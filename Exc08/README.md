# ABAP CDS

**Typkonvertierungen**<br>
<br>
Erweitere den View ZI_FlugSitzplatz[xx]<br>
<br>
Füge ein Feld für den 1,5 fachen Preis hinzu mit Casting<br>
<br>
Füge ein Initial-Datum ein (‚00000000‘) und caste es nach dem Typ von FLDATE<br>
<br>
Prüfe die aktiven Annotationen für das Initial-Datum<br>
Von wo wurden die Annotationen übernommen?<br>
<br>
<br>
Erweitere den View ZI_Kunde[xx]<br>
<br>
Das dort enthaltene Feld Discount gibt den Rabatt an, allerdings als 3-stellige Ganzzahl (020 statt 0,2)<br>
Lege ein Feld Rabatt_Faktor an für die Berechnung von Discount / 100<br>
Caste die Felder ein passendes Format (abap.fltp)<br>
