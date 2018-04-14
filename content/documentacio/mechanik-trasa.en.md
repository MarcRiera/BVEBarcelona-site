---
url: "/documentation/mechanik-trasa"
title: "Format especification – Route files (Trasa.dat)"
draft: true
---
## General specifications

Mechanik routes are plain text files containing a list of commands. Each command is placed in a new line and comprises a name followed by several values separated by either a space or a tab. These commands can be of three types:

* 3D objects
* 2D objects (scaled objects)
* Control objects


### 3D considerations

Unlike most modern 3D software, the unit of measurement in Mechanik is the pixel. Conversion to meters is achieved by dividing any size by 200; that is, 200 pixels in Mechanik equal 1 meter in real life. X/Y/Z coordinates work mostly the same as any other 3D software, except that the Y axis is inverted (objects above the ground have a negative Y coordinate).

In addition to this, the position of the objects in the world (except the Z axis, which corresponds to the train's direction) is not absolute, but relative to the driver's point of view. By default, the driver's eyes are 2 meters above the track (which means that the ground or track is in Y -2.0), and 0.75 meters to the right, but there is at least one route (Prague Metro) known to use slightly different values (there is no X axis offset).

Vertices must always be declared in clockwise order.


## List of commands

This is a list of all the available commands in Mechanik. 3D and 2D objects are visible in the world, and control objects are invisible.


### 3D objects


#### #t (3D textured object)

```#t km ile x1 y1 z1 x2 y2 z2 x3 y3 z3 x4 y4 z4 x5 y5 z5 x6 y6 z6 x7 y7 z7 nr_0 m_v m_u dlugosz nr_t jakosc nr_konca```

The #t command defines a 3D object with a texture. It takes the following arguments:

km: The distance from the beginning of the route.

ile: The number of vertices (3, 4 or 5).

x1, y1, z1: The 3D coordinates for the first vertex.

x2, y2, z2: The 3D coordinates for the second vertex.

x3, y3, z3: The 3D coordinates for the third vertex.

x4, y4, z4: The 3D coordinates for the fourth vertex.

x5, y5, z5: The 3D coordinates for the fifth vertex.

x6, y6, z6: The 3D coordinates for the sixth vertex (currently not used, should be 0, 0, 0).

x7, y7, z7: The 3D coordinates for the seventh vertex (currently not used, should be 0, 0, 0).

nr_0:

m_v:

m_u:

dlugosz: The scale of the texture.

nr_t: The texture index.

jakosc: 

nr_konca: 


#### #t_prz (3D transparent textured object)

```#t_prz km ile x1 y1 z1 x2 y2 z2 x3 y3 z3 x4 y4 z4 x5 y5 z5 x6 y6 z6 x7 y7 z7 nr_0 m_v m_u dlugosz nr_t jakosc nr_konca```

The #t_prz command defines a 3D object with a transparent texture. It is identical to the #t command, but pure black is used as the alpha colour. It takes the following arguments:

km: The distance from the beginning of the route.

ile: The number of vertices (3, 4 or 5).

x1, y1, z1: The 3D coordinates for the first vertex.

x2, y2, z2: The 3D coordinates for the second vertex.

x3, y3, z3: The 3D coordinates for the third vertex.

x4, y4, z4: The 3D coordinates for the fourth vertex.

x5, y5, z5: The 3D coordinates for the fifth vertex.

x6, y6, z6: The 3D coordinates for the sixth vertex (currently not used, should be 0, 0, 0).

x7, y7, z7: The 3D coordinates for the seventh vertex (currently not used, should be 0, 0, 0).

nr_0:

m_v:

m_u:

dlugosz: The scale of the texture.

nr_t: The texture index.

jakosc: 

nr_konca: 


#### #t_p (3D horizontal textured object)

```#t_p km ile x1 y1 z1 x2 y2 z2 x3 y3 z3 x4 y4 z4 x5 y5 z5 x6 y6 z6 x7 y7 z7 nr_0 m_v m_u dlugosz nr_t nr_konca```

The #t_prz command defines a 3D object with a texture. Objects must be horizontal in the Z axis. It takes the following arguments:

km: The distance from the beginning of the route.

ile: The number of vertices (3, 4 or 5).

x1, y1, z1: The 3D coordinates for the first vertex.

x2, y2, z2: The 3D coordinates for the second vertex.

x3, y3, z3: The 3D coordinates for the third vertex.

x4, y4, z4: The 3D coordinates for the fourth vertex.

x5, y5, z5: The 3D coordinates for the fifth vertex.

x6, y6, z6: The 3D coordinates for the sixth vertex (currently not used, should be 0, 0, 0).

x7, y7, z7: The 3D coordinates for the seventh vertex (currently not used, should be 0, 0, 0).

nr_0:

m_v:

m_u:

dlugosz: The scale of the texture.

nr_t: The texture index.

nr_konca: 


### 2D objects


### Control objects


#### 'z_d (Sound marker)

```'z_d km x z nr_d k petla hz_v glosnosc```

The 'z_d command starts or stops playing a sound. It takes the following arguments:

km: The distance from the beginning of the route.

x: The X coordinate of the sound.

z: The Z coordinate of the sound.

nr_d: The sound index.

k:

petla: Whether the sound plays in a loop (1) or not (0).

hz_v: Whether the sound is affected by the train's speed (1) or not (0).

glosnosc: The volume at which the sound is played (0-128)


#### 'z_p (Speed marker)

```'z_p km x z pr```

The 'z_p command sets a speed limit. It takes the following arguments:

km: The distance from the beginning of the route.

x: The X coordinate of the limit.

z: The Z coordinate of the limit.

pr: The speed limit.


#### 'z_s (Whistle marker)

```'z_s km x z status```

The 'z_s command sets a whistle marker. Two must be placed to define a section, one at the beginning and another at the end. It takes the following arguments:

km: The distance from the beginning of the route.

x: The X coordinate of the marker.

z: The Z coordinate of the marker.

status: Whether the section during which the whistle must be played starts (1) or ends (0).


#### 'z_z (Stop marker)

```'z_z km x z status```

The 'z_z command sets a stop marker. Two must be placed to define a section, one at the beginning and another at the end. It takes the following arguments:

km: The distance from the beginning of the route.

x: The X coordinate of the marker.

z: The Z coordinate of the marker.

status: Whether the section in which the train must stop starts (1) or ends (0).


#### 'z_shp (Indusi/PZB marker)

```'z_shp km x z status```

The 'z_shp command places an Indusi/PZB beacon in the track. It takes the following arguments:

km: The distance from the beginning of the route.

x: The X coordinate of the marker.

z: The Z coordinate of the marker.

status: Must be always 1.


#### 'z_jb (Current break marker)

```'z_jb km x z status```

The 'z_jb command sets a current break marker. Two must be placed to define a currentless section, one at the beginning and another at the end. It takes the following arguments:

km: The distance from the beginning of the route.

x: The X coordinate of the marker.

z: The Z coordinate of the marker.

status: Whether the currentless section starts (1) or ends (0).
