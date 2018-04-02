---
url: "/manuals/driving-2000-3000-4000-series"
title: "Driving manual – Barcelona Metro 2000/3000/4000 Series"
image: '/images/manuals/3000/portada.png'
---
The 3000 and 4000 series train sets were ordered in the mid-1980s to improve service on L3 and L1, respectively, both of which had very old cars in service that needed replacement. Technically, the two series are the same, but the 4000 series trains are wider to run on Iberian gauge. Many years after entering service, both series were fitted with ATP/ATO systems.

The 2000 series, in contrast, was ordered to start commercial service on L2 during the 1992 Olympics. Although L2 did not open until 1995, the trains entered into service temporarily on L3. These trains were very similar to those of the 3000 series, but they had built-in ATP/ATO systems and their cars were connected by gangways.

All the information in this manual applies to the three series unless otherwise specified.

<center><h1>Driver’s cab</h1></center>

<table>
<tr><td rowspan=11><img src="/images/manuals/3000/Cabina.png" alt="Cabina"></td><td>1. Power-brake handle</td></tr>
<tr><td>2. Emergency brakes</td></tr>
<tr><td>3. Reverser</td></tr>
<tr><td>4. Brake pressure gauge</td></tr>
<tr><td>5. Door status indicators</td></tr>
<tr><td>6. ATC panel</td></tr>
<tr><td>7. SAC display</td></tr>
<tr><td>8. Slope brake</td></tr>
<tr><td>9. Headlights</td></tr>
<tr><td>10. Door closing signal</td></tr>
<tr><td>11. Horn pedal</td></tr>
</table>

<center><h1>ATC Panel (2000 series)</h1></center>

<table>
<tr><td rowspan=6><img src="/images/manuals/3000/ATC2000.png" alt="ATC2000"></td><td>A. Speedometer</td></tr>
<tr><td>B. Target speed indicators</td></tr>
<tr><td>C. Driving mode selector/indicator</td></tr>
<tr><td>D. ATO startup buttons</td></tr>
<tr><td>E. Overspeed indicator</td></tr>
<tr><td>F. ATP code indicator</td></tr>
</table>

<center><h1>ATC Panel (3000/4000 series)</h1></center>

<table>
<tr><td rowspan=6><img src="/images/manuals/3000/ATC3000.png" alt="ATC3000"></td><td>A. Speedometer</td></tr>
<tr><td>B. Target speed indicator</td></tr>
<tr><td>C. Driving mode selector/indicator</td></tr>
<tr><td>D. ATO startup buttons</td></tr>
<tr><td>E. Brake activation indicator</td></tr>
<tr><td>F. Target distance indicator</td></tr>
</table>

<center><h1>Keyboard</h1></center>

| Key | Default assignment | Function |
| ------------ | ------------- | ------------- |
| SECURITY_S | Space bar | Dead man switch |
| SECURITY_D | 2 | Changes to Manual+25 mode |
| SECURITY_E | 3 | Changes to Manual+ATP mode |
| SECURITY_F | 4 | Changes to ATO mode |
| SECURITY_I | 7 | Disables the slope brake |
| SECURITY_J + SECURITY_L | 8 + 0 | Starts up the train in ATO mode |
| SECURITY_C2 | Page Down | Turns on or off the headlights |
| RAISE_PANTOGRAPH | P | Raises the pantographs and disconnects the contact shoes |
| LOWER_PANTOGRAPH | Ctrl + P | Lowers the pantographs and connnects the contact shoes |
| HORN_PRIMARY | Enter | Plays the horn |
| HORN_SECONDARY | Add (numpad) | Plays the door closing signal |
| SECURITY_B2 | End | Enables or disables the safety systems (special mode) |

<center><h1>Driving the train</h1></center>

The 2000, 3000 and 4000 series trains have a power-brake handle (1) with 7 brake notches, 4 power notches and 1 neutral notch. Although the controls are the same as for any other openBVE train with a single handle, the so-called ***Dead man*** device must be taken into account. It is very important to keep the button (space bar) pressed at all times while the train is in motion. If for any reason the button is not pressed for more than 3 seconds, the emergency brakes will be applied and the train will not move again until it has fully stopped.

## Driving modes

The 2000, 3000 and 4000 series trains have three driving modes: Manual+25, Manual+ATP and ATO. The Manual+25 mode is always available, while Manual+ATP and ATO will only be active if ATP codes and stop position beacons are found in the route.

### Manual+25 Mode

The Manual+25 mode is the default mode in the train and the most basic one. It is used for train reversing at the end of the line and to drive the train through sections with no ATP protection. In this mode, the train speed is permanently limited to 25kmph, and the service brakes are automatically applied at higher speeds. If ATP codes are detected in the track, it is possible to change to the Manual+ATP mode, even with the train in motion.

### Manual+ATP Mode

The Manual+ATP mode is the normal train driving mode in track sections fitted with ATP protection. In this mode, the train speed is limited to the section’s target speed (B), which is displayed in the driver’s cab using LEDs (2000 series) or a display (3000 and 4000 series). The service brakes will be automatically applied at higher speeds.

### ATO Mode

El mode ATO és el mode de conducció més habitual actualment. En aquest mode, el tren circula de manera autònoma a la velocitat màxima permesa fins a la següent estació The ATO mode is the most usual driving mode currently. In this mode, the train automatically drives itself at the maximum permitted speed to the next station and stops at the stop marker. This means that the driver only has to operate the doors and press the ATO startup buttons (keys 8 and 0). The train may stop between two stations due to line traffic, but in this case it will begin to move again after a few seconds without the need for the driver to do anything.

The power-brake handle (1) must be place at neutral (N) in order to start up the train. However, it is possible to activate the brakes manually between stations if it were necessary. It is also possible to change to Manual+ATP mode at any time.

## Disabling the safety systems (special mode)

The 2000, 3000 and 4000 series trains have a ***Special Mode*** available to drive on track sections without ATP protection and override the Manual+25 mode speed limit. Even though it is forbidden to use it during normal service, it may be useful for openBVE routes without ATP features. It can be turned on or off (Page Down) at any time the train is stopped.

## Starting up the train on slopes

The 2000, 3000 and 4000 series trains have a slope brake (8) that prevents the train from slipping in slopes after releasing the brakes. To start up the train under these conditions (at stations placed on slopes, for example), the slope brake button (key 7) must be pressed to release the brakes and allow the train to move.

## Tips

* It is advised to use the headlights in the tunnels, but they must be turned off at stations or if an oncoming train is near.
* The status of the doors can be checked at all times in the SAC display (7).
* It is completely forbidden to drive the train backwards. Doing so will trigger a warning sound signal.

<center>***Have a nice trip!***</center>
