# ABAP CDS

**Konvertierungen**<br>
<br>
Erweitere den View ZI_Flug[xx]<br>
<br>
Annotiere Price und Currency als Währungsfelder über die Domäne Semantics<br>
Füge ein neues Feld hinzu Preis_in_Euro mit entsprechender Konvertierung nach Flugdatum<br>
Nutze für die Zielwährung ein Cast auf abap.cuky<br>
<br>
<br>


Erweitere den View ZI_FLugplan[xx]<br>
<br>
Annotiere Distance und Distid als Distanzfelder für die Domäne Semantics<br>
Für ein neues Feld hinzu Distanz_in_KM mit entsprechender Konvertierung <br>
Nutze als Zielformat ein Cast auf abap.unit<br>
Caste das Ergebnis in das gleiche Datenelement wie Distance<br>
