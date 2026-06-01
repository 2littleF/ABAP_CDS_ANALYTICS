# ABAP CDS

**Union**<br>
<br>
Erstelle einen View ZI_Buchung_Rabatt[xx] basierend auf ZI_Kunde[xx], ZI_Flug[xx] und ZI_Buchung[xx]<br>
<br>
Geschäftskunden vom Typ B (Custtype) bekommen einen Rabatt von 10%<br>
<br>
Verknüpfe die Kunde mit den Buchungen per Join <br>
Rückgabe sind die Schlüsselfelder der Buchung, der Kunde mit Name und der Preis des Fluges und der Preis in Euro mit neuem Rabatt_Feld<br>
<br>
Führe diesen Join getrennt für die Typen P und B durch<br>
<br>
Führe Kunden vom Typ P und Typ B dann in der Ergebnismenge zusammen per Union<br>
<br>
![alt text](image.png)
