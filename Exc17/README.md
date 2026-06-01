# ABAP CDS

**Annotationen anlegen**<br>
<br>
Annotiere den View ZI_Umsatz_Kundenverhalten[xx]<br>
<br>
Gib jedem Feld eine passende Bezeichnung Label aus der Domäne EndUser<br>
<br>
Schalte die volle Pufferung für den CDS View an, geht dies bei Entity Views?<br>
@AbapCatalog.buffering.status: #ACTIVE<br>
https://help.sap.com/docs/abap-cloud/abap-data-models/cds-view-entity-buffers?locale=en-US<br>
Erlaube die Pufferung mit @AbapCatalog.entityBuffer.definitionAllowed<br>
und passe alle erforderlichen Entitäten an<br>
Erzeuge eine Pufferung ZB_Buffer_Umsatz_KundenXX für den Layer Partner für alle Daten
<br>
<br>
Prüfe die aktiven Annotationen über das Werkzeug Active Annotations<br>
