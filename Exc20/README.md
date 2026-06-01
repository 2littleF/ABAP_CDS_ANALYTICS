# ABAP CDS Fortgeschrittene Konzepte

**Input Parameter**<br>
<br>
Kopiere den View ZI_Flug[xx] nach ZI_Flug_Datum[xx]<br>
<br>
Führe einen Input Parameter für das Datum P_Rate_Date des Währungswechsels ein vom Typ Abap Datum<br>
Dieser wird mit dem Systemdatum vorbelegt aus der Domöne Environment<br>
<br>
Führe einen Input Parameter P_Target_Curr für die Zielwährung ein vom Typ der Währung<br>
<br>
Passe die Konvertierung im View auf die Input-Felder an, benenne das Feld entsprechend um<br>
Prüfe den View im Data Preview<br>
<br>
<br>
Kopiere den View ZI_Umsatz_pro_Flug[xx] nach ZI_Umsatz_pro_Flug_Input[xx]<br>
<br>
Ändere die Quelle in ZI_Flug_Datum[xx] für einen View on View mit Input Parameter und versorge die Parameter<br>
Die neue Zielwährung ist JPY<br>
Das Datum ist das Systemdatum über die Systemvariable $session.system_date<br>
<br>
Gebe zusätzlich die Buchungswährung und die Summe des Buchungspreises an<br>
Gebe zusätzlich die gewählte Zielwährung aus dem Input-Parameter mit aus<br>
 