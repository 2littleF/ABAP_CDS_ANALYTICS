# ABAP CDS Verwendung

**Embedded Analytics**<br>
<br>
Lege eine Dimension ZI_FLUG_DIMXX für ZI_FLUGXX an <br>
<br>VDM-View-Type Basic / Analtics-Data-Category Dimension
    key Carrid,<br>
    key Connid,<br>
    key Fldate,<br>
    Planetype,<br>
    Seatsmax,<br>
    Seatsocc,<br>
    SeatsmaxB,<br>
    SeatsoccB,<br>
    SeatsmaxF,<br>
    SeatsoccF<br>
<br>
Lege einen Cube ZI_BUCHUNG_CUBEXX als Würfel an für ZI_BuchungXX mit<br>
Left-Outer-Join auf die Dimension, als Composite mit Category Cube.<br>
    key ZI_Buchung00.Carrid,<br>
    key ZI_Buchung00.Connid,<br>
    key ZI_Buchung00.Fldate,<br>
    key ZI_Buchung00.Bookid,<br>
    @Aggregation.default: #SUM<br>
    ZI_Buchung00.Luggweight,<br>
    ZI_Buchung00.Wunit,<br>
    ZI_Buchung00.Class_Text,<br>
    @Aggregation.default: #MAX<br>
    ZI_Buchung00.Buchung_im_Voraus,<br>
    _Flug_Dim00.Planetype as Planetype<br>
<br>
Lege eine Query ZC_BUCHUNG_QUERYXX für den Cube an als Consumption mit Analytics.Query True.<br>
Beachte die Freigabe des API Status<br>
Benenne den Enduser-Label mit einem sprechenden Namen<br>
    key Carrid,<br>
    key Connid,<br>
    key Fldate,<br>
    key Bookid,<br>
    Luggweight,<br>
    Wunit,<br>
    Class_Text,<br>
    Buchung_im_Voraus,<br>
    Planetype<br>
<br>
Prüfe die Query in der RSRT (Name ist der Enduser-Label<br>
<br>
Prüfe die Query im View-Browser (/UI2/FLP)<br>
