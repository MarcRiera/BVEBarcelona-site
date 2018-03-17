---
title: "Manual de conducció – Sèrie 2000/3000/4000 del Ferrocarril Metropolità de Barcelona"
image: '/images/manuals/3000/portada.png'
---
Els trens de les sèries 3000 i 4000 van ser encarregats a mitjans dels anys 80 per modernitzar el servei a la L3 i la L1, respectivament. A nivell tècnic les dues sèries són idèntiques, amb l’única diferència que els trens de la sèrie 4000 són més amples i circulen en ample ibèric. Posteriorment, a totes dues sèries se’ls va instal·lar els sistemes ATP/ATO.

La sèrie 2000, en canvi, va ser encarregada per inaugurar la L2 en motiu dels Jocs Olímpics de l’any 1992. Tot i que la L2 no es va inaugurar fins l’any 1995, va entrar en servei provisionalment a la L3. Aquests trens eren molt semblants als de la sèrie 3000, però tenien els sistemes ATP/ATO instal·lats de fàbrica i els cotxes estaven comunicats per passadissos.

Tota la informació d’aquest manual s’aplica als tres trens a no ser que s’indiqui el contrari.

<center><h1>Cabina de conducció</h1></center>

<table>
<tr><td rowspan=11><img src="/images/manuals/3000/Cabina.png" alt="Cabina"></td><td>1. Manipulador marxa-fre</td></tr>
<tr><td>2. Fre d'emergència</td></tr>
<tr><td>3. Selector de marxa</td></tr>
<tr><td>4. Indicador de pressió dels frens</td></tr>
<tr><td>5. Indicadors de les portes</td></tr>
<tr><td>6. Panell ATC</td></tr>
<tr><td>7. Monitor SAC</td></tr>
<tr><td>8. Fre de retenció</td></tr>
<tr><td>9. Fars</td></tr>
<tr><td>10. Xiulet de tancament de portes</td></tr>
<tr><td>11. Xiulet</td></tr>
</table>

<center><h1>Panell ATC (Sèrie 2000)</h1></center>

<table>
<tr><td rowspan=6><img src="/images/manuals/3000/ATC2000.png" alt="ATC2000"></td><td>A. Velocímetre</td></tr>
<tr><td>B. Indicadors de velocitat objectiu</td></tr>
<tr><td>C. Selector/indicador del mode de conducció</td></tr>
<tr><td>D. Polsadors d'arrencada ATO</td></tr>
<tr><td>E. Indicador d'excés de velocitat</td></tr>
<tr><td>F. Indicador de presència de codis ATP</td></tr>
</table>

<center><h1>Panell ATC (Sèrie 3000/4000)</h1></center>

<table>
<tr><td rowspan=6><img src="/images/manuals/3000/ATC3000.png" alt="ATC3000"></td><td>A. Velocímetre</td></tr>
<tr><td>B. Indicador de velocitat objectiu</td></tr>
<tr><td>C. Selector/indicador del mode de conducció</td></tr>
<tr><td>D. Polsadors d'arrencada ATO</td></tr>
<tr><td>E. Indicador d'activació dels frens</td></tr>
<tr><td>F. Indicador de distància objectiu</td></tr>
</table>

<center><h1>Teclat</h1></center>

| Teclat | Assignació per defecte | Funció |
| ------------ | ------------- | ------------- |
| SECURITY_S | Barra d'espai | Desactiva l'home mort |
| SECURITY_D | 2 | Canvia a mode Manual+25 |
| SECURITY_E | 3 | Canvia a mode Manual+ATP |
| SECURITY_F | 4 | Canvia a mode ATO |
| SECURITY_I | 7 | Desactiva el fre de retenció |
| SECURITY_J + SECURITY_L | 8 + 0 | Arrenca el tren en mode ATO |
| SECURITY_C2 | Av Pàg | Encén o apaga els fars davanters |
| RAISE_PANTOGRAPH | P | Aixeca els pantògrafs i desconnecta els patins |
| LOWER_PANTOGRAPH | Ctrl + P | Abaixa els pantògrafs i connecta els patins |
| HORN_PRIMARY | Enter | Activa el xiulet |
| HORN_SECONDARY | Suma (teclat numèric) | Activa el xiulet de tancament de portes |
| SECURITY_B2 | Fi | Activa o desactiva els sistemes de seguretat (mode especial) |

<center><h1>Conducció del tren</h1></center>

Els trens de les sèries 2000, 3000 i 4000 disposen d’un manipulador marxa-fre (1) amb 7 posicions de fre de servei, 4 posicions de tracció i 1 posició de deriva. Tot i que els controls són els estàndard per a qualsevol tren de control simple a OpenBVE, cal tenir en compte l’anomenat ***Home mort***. És molt important mantenir activat el polsador (barra d’espai) durant la tracció, la deriva i la frenada. Si per qualsevol raó no s’activa el polsador durant més de 3 segons, el tren aplicarà el fre d’emergència i no es podrà reprendre la marxa fins que s’hagi aturat completament.

## Modes de conducció

Els trens de les sèries 2000, 3000 i 4000 disposen de tres modes de conducció: Manual+25, Manual+ATP i ATO. El mode Manual+25 sempre està disponible, i els modes Manual+ATP i ATO només s’activaran si es detecten codis ATP i codis de parada a la ruta.

### Mode Manual+25

El mode Manual+25 és el mode per defecte del tren i el més bàsic. S’utilitza per realitzar maniobres al final de la línia i per circular per trams de via sense protecció ATP. En aquest mode, la velocitat del tren està limitada permanentment a 25 km/h, i s’aplica automàticament el fre de servei si la velocitat és superior. Si es detecten codis ATP a la via, és possible canviar a mode Manual+ATP, fins i tot durant la marxa.

### Mode Manual+ATP

El mode Manual+ATP és el mode de conducció normal del tren en trams de via amb protecció ATP. En aquest mode, la velocitat del tren queda limitada per la velocitat objectiu (B) del tram, que s’indica a la cabina mitjançant llums LED (sèrie 2000) o una pantalla (sèries 3000 i 4000). S’aplicarà automàticament el fre de servei si la velocitat és superior a la permesa al tram.

### Mode ATO

El mode ATO és el mode de conducció més habitual actualment. En aquest mode, el tren circula de manera autònoma a la velocitat màxima permesa fins a la següent estació i s’atura al punt de parada. Per tant, el conductor es limita a obrir i tancar les portes i prémer els polsadors d’arrencada ATO (tecles 8 i 0). És possible que el tren s’aturi entre dues estacions si hi ha problemes de trànsit a la línia, però en aquest cas reprendrà la marxa al cap d’uns segons sense que el conductor hagi d’actuar.

El manipulador marxa-fre (1) ha d’estar en posició de deriva (N) perquè el tren pugui arrencar. De totes maneres, és possible activar el fre manualment durant la circulació si fos necessari. També es pot canviar a mode Manual+ATP en qualsevol moment.

## Desactivar els sistemes de seguretat (mode especial)

Els trens de les sèries 2000, 3000 i 4000 disposen d’un ***Mode especial*** per circular per vies sense protecció ATP sense la limitació de velocitat del mode Manual+25. Tot i que està prohibit utilitzar-lo durant la circulació normal, pot ser útil per a rutes d’OpenBVE sense característiques ATP. Es pot activar o desactivar (Av Pàg) sempre que el tren estigui aturat.

## Arrencada en pendent

Els trens de les sèries 2000, 3000 i 4000 disposen d’un fre de retenció (8) que impedeix que el tren es desplaci quan s’alliberen els frens en un tram en pendent. Per arrencar en aquestes condicions (per exemple, en una estació en pendent), cal prémer breument el polsador del fre de retenció (tecla 7) per alliberar els frens i permetre que el tren arrenqui.

## Consells

* Es recomana circular en túnel amb els fars encesos, però s’han d’apagar a les estacions o si hi ha un tren en direcció contrària.
* Es pot comprovar l’estat de les portes en qualsevol moment al monitor SAC (7).
* Està totalment prohibit utilitzar la marxa enrere durant la circulació. Si s’activa la marxa enrere sonarà un avís acústic.

<center>***Bon viatge!***</center>
