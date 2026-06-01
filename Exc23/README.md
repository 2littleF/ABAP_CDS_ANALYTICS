# ABAP CDS Fortgeschrittene Konzepte

**Filter bei Assoziationen**<br>
<br>
Erstelle einen View ZI_Flug_Route_Asso_Text[xx] als Kopie von ZI_Flug_Route[xx]<br>
<br>
Assoziiere den neuen View mit den Texten zur Währung in der Tabellen TCURT über das Währungsfeld<br>
<br>
Zeige aus der Tabelle TCURT den Kurztext im CDS-View mit an, der für den aktuellen Sprachschlüssel in $session gilt<br>
Filtere dazu das Feld KTEXT aus TCURT direkt über die Systemvariable $session.system_language<br>
<br>
Prüfe den View im Data Preview<br>
Nutze auch die Pfadnavigation<br>
