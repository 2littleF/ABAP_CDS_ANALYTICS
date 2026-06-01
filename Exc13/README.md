# ABAP CDS

**Aggregationen und View on View**<br>
<br>
Erstelle einen View ZI_Umsatz_pro_Flug[xx] basiernd auf dem View ZI_Flug[xx]<br>
<br>
Aggregiere auf die Summe des Preises in Euro<br>
Nur Gesellschaft und Verbindung sind interessant<br>
![alt text](image.png)
<br>
<br>
Basieren auf ZI_BUCHUNG[xx]<br>
Aggregiere in einem Hilfsview ZP_Kundenbuchung[xx] die durchschnittliche Anzahl der Tage die ein Kunde im Voraus gebucht hat<br>
Runde das Ergebnis in ZI_Kundenbuchung basieren auf dem Hilfsview in auf den nächsten vollen Tag<br>
<br>
Achtung: View Entity würden auch ohne Hilfsview auskommen, die obsoleten View nicht<br>
<br>
Für die Verdichtung ist nur der Kunde interessant<br>
![alt text](image-1.png)
<br>
<br>
<br>
Hilfe: avg(Buchung_im_voraus as abap.dec(12,2))<br>
AVG wirft eine Fehlermeldung bei VIEW Entity, wenn kein Casting erfolgt AVG(Field as ...)<br>
https://help.sap.com/doc/abapdocu_cp_index_htm/CLOUD/en-US/ABENCDS_AVG_AS_V1.html

