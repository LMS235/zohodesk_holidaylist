# Custom Function für externe Ticketnummern

Eine Custom Function um jedes Jahr die Holiday List zu pflegen

## Vorbereitung
 
### OAuth Verbindung

1. Click on Setup > Developer Space > Connections 
2. Click on Create Connection
3. Choose Zoho OAuth
4. Name Connection and connection link as "holidayup"
5. In Scope Choose Desk.settings.UPDATE
6. Click on Create and Connect
7. Click on Connect
8. Click on Accept and proceed

### Anpassungen im Code

  - Die Feiertage die man benötigt entsprechend definieren und die API erstellen (im Code sind es aktuell DEUTSCHLAND und BAYERN (BY)) - Siehe api-feiertage.de
  - im `posttext = '] , "name" : "Feiertage_Deutschland"}';` entsprechend den Namen der Holiday List hinterlegen
  - im `url :"https://desk.zoho.eu/api/v1/holidayList/<HOLIDAYLISTID>"` entsprechend die ID der Holiday List hinterlegen

# Einbau als Schedule

Den Code kann man jetzt einmal im Jahr laufen lassen um die Holiday List aktuell zu haben.

Code wird "as is" zu Verfügung gestellt. Keinerlei Haftung oder Support.

