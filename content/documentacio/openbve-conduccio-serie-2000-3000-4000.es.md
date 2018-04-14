---
url: "/documentation/openbve-conduccion-serie-2000-3000-4000"
title: "Manual de conducción – Serie 2000/3000/4000 del Ferrocarril Metropolitano de Barcelona"
image: '/images/manuals/3000/portada.png'
---
Los trenes de las series 3000 y 4000 fueron encargados a mediados de los años 80 para modernizar el servicio en la L3 y la L1, respectivamente. A nivel técnico las dos series son idénticas, con la única diferencia que los trenes de la serie 4000 son más anchos y circulan en ancho ibérico. Posteriormente, se instalaron los sistemas ATP/ATO en los trenes de ambas series.

La serie 2000, en cambio, fue encargada para inaugurar la L2 en motivo de los Juegos Olímpicos del año 1992. Aunque la L2 no se inauguró hasta el 1995, entró en servicio 
provisionalmente en la L3. Estos trenes eran muy parecidos a los de la serie 3000, pero llevaban los sistemas ATP/ATO instalados de fábrica y los coches estaban comunicados por pasillos.

Toda la información de este manual se aplica a los tres trenes a no ser que se indique lo contrario.

## Cabina de conducción

<table>
<tr><td rowspan=11><img src="/images/manuals/3000/Cabina.png" alt="Cabina"></td><td>1. Manipulador marcha-freno</td></tr>
<tr><td>2. Freno de emergencia</td></tr>
<tr><td>3. Selector de marcha</td></tr>
<tr><td>4. Indicador de presión de los frenos</td></tr>
<tr><td>5. Indicadores de les puertas</td></tr>
<tr><td>6. Panel ATC</td></tr>
<tr><td>7. Monitor SAC</td></tr>
<tr><td>8. Freno de retención</td></tr>
<tr><td>9. Faros</td></tr>
<tr><td>10. Silbato de cierre de puertas</td></tr>
<tr><td>11. Silbato de vía</td></tr>
</table>

## Panel ATC (Serie 2000)

<table>
<tr><td rowspan=6><img src="/images/manuals/3000/ATC2000.png" alt="ATC2000"></td><td>A. Velocímetro</td></tr>
<tr><td>B. Indicadores de velocidad objetivo</td></tr>
<tr><td>C. Selector/indicador del modo de conducción</td></tr>
<tr><td>D. Pulsadores de arranque ATO</td></tr>
<tr><td>E. Indicador de exceso de velocidad</td></tr>
<tr><td>F. Indicador de presencia de códigos ATP</td></tr>
</table>

## Panel ATC (Serie 3000/4000)

<table>
<tr><td rowspan=6><img src="/images/manuals/3000/ATC3000.png" alt="ATC3000"></td><td>A. Velocímetro</td></tr>
<tr><td>B. Indicador de velocidad objetivo</td></tr>
<tr><td>C. Selector/indicador del modo de conducción</td></tr>
<tr><td>D. Pulsadores de arranque ATO</td></tr>
<tr><td>E. Indicador de activación de los frenos</td></tr>
<tr><td>F. Indicador de distancia objetivo</td></tr>
</table>

## Teclado

| Teclado | Assignación por defecto | Función |
| ------------ | ------------- | ------------- |
| SECURITY_S | Barra de espacio | Desactiva el hombre muerto |
| SECURITY_D | 2 | Cambia a modo Manual+25 |
| SECURITY_E | 3 | Cambia a modo Manual+ATP |
| SECURITY_F | 4 | Cambia a modo ATO |
| SECURITY_I | 7 | Desactiva el freno de retención |
| SECURITY_J + SECURITY_L | 8 + 0 | Arranca el tren en modo ATO |
| SECURITY_C2 | Av Pág | Enciende o apaga los faros delanteros |
| RAISE_PANTOGRAPH | P | Sube los pantógrafos y desconecta los patines |
| LOWER_PANTOGRAPH | Ctrl + P | Baja los pantógrafos y conecta los patines |
| HORN_PRIMARY | Intro | Activa el silbato de vía |
| HORN_SECONDARY | Sumar (teclado numérico) | Activa el silbato de cierre de puertas |
| SECURITY_B2 | Fin | Activa o desactiva los sistemas de seguridad (modo especial) |

## Conducción del tren

Los trenes de las series 2000, 3000 y 4000 disponen de un manipulador marcha-freno (1) con 7 posiciones de freno de servicio, 4 posiciones de tracción y 1 posición de deriva. Aunque los controles son los estándar para cualquier tren de control simple en openBVE, hay que tener en cuenta el llamado ***Hombre muerto***. Es muy importante mantener activado el pulsador (barra de espacio) durante la tracción, la deriva y el frenado. Si por cualquier motivo no se activa el pulsador durante más de 3 segundos, el tren aplicará el freno de emergencia y no se podrá retomar la marcha hasta que esté parado por completo.

### Modos de conducción

Los trenes de las series 2000, 3000 y 4000 disponen de tres modos de conducción: Manual+25, Manual+ATP y ATO. El modo Manual+25 siempre está disponible, y los modos Manual+ATP y ATO solo se activarán si se detectan códigos ATP y códigos de parada en la ruta.

#### Modo Manual+25

El modo Manual+25 es el modo por defecto del tren y el más básico. Se utiliza para realizar manioras al final de la línea y para circular en tramos de vía sin protección ATP. En este modo, la velocidad del tren está limitada permanentemente a 25 km/h, y se aplica automáticamente el freno de servicio si la velocidad es superior. Si se detectan códigos ATP en la vía, es posible cambiar a modo Manual+ATP, incluso durante la marcha.

#### Modo Manual+ATP

El modo Manual+ATP es el modo de conducción normal del tren en tramos de vía con protección ATP. En este modo, la velocidad del tren queda limitada por la velocidad objetivo (B) del tramo, que se indica en la cabina mediante luces LED (serie 2000) o una pantalla (series 3000 y 4000). Se aplicará automáticamente el freno de servicio si la velocidad es superior a la permitida en el tramo.

#### Modo ATO

El modo ATO es el modo de conducción más habitual actualmente. En este modo, el tren circula de manera autónoma a la velocidad máxima permitida hasta la siguiente estación y para en el punto de parada. Por lo tanto, el conductor se limita a abrir y cerrar las puertas y a pulsar los botones de arranque ATO (teclas 8 y 0). Es posible que el tren se pare entre dos estaciones si hay problemas de tráfico en la línea, pero en este caso retomará la marcha después de unos segundos sin que el conductor tenga que actuar.

El manipulador marcha-freno (1) tiene que estar en posición de deriva (N) para que el tren pueda arrancar. de todas formas, es posible activar el freno manualmente durante la circulación si fuera necesario. También se puede cambiar a modo Manual+ATP en cualquier momento.

### Desactivar los sistemas de seguridad (modo especial)

Los trenes de las series 2000, 3000 y 4000 disponen de un ***Modo especial*** para circular por vías sin protección ATP sin la limitación de velocidad del modo Manual+25. Aunque está prohibido utilizarlo durante la circulación normal, puede ser útil para rutas de openBVE sin características ATP. Se puede activar o desactivar (Av Pág) siempre que el tren se encuentre parado.

### Arranque en pendiente

Los trenes de las series 2000, 3000 y 4000 disponen de un freno de retención (8) que impide que el tren se desplace cuando se sueltan los frenos en un tramo en pendiente. Para arrancar en estas condiciones (por ejemplo, en una estación en pendiente), hay que pulsar brevemente el pulsador del freno de retención (tecla 7) para soltar los frenos y permitir que el tren arranque.

### Consejos

* Se recomienda circular en túnel con los faros encendidos, pero se deben apagar en las estaciones o si hay un tren en dirección opuesta.
* Se puede comprobar el estado de las puertas en cualquier momento en el monitor SAC (7).
* Está totalmente prohibido usar la marcha atrás durante la circulación. Si se activa la marcha atrás, sonará un aviso acústico.

<center>***¡Buen viaje!***</center>
