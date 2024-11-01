# Finace-WebApp-Mern-Stack


# Projekt-Dokumentation



Filip Mitrovic, Cedric Tuma, Raul Gilardoni und Kenan Bajramovic

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|   23.08.2024    | 0.0.1   |  Wir haben uns für ein Finance Webapp entschieden zu implementieren mit Mern Stack und uns darüber informiert. Wir haben begonnen Visual Studio zu Einrichten für unser Projekt. Bei der Einrichtung sind wir auf viele Problemen zugestossen, aber haben auch viel dazugelernt. Die Konfiguartion ist bis jetzt ohne Erfolg. Die Projektdokumentation und das Layout wurden erstellt.|
|   30.08.2024   | 0.0.2   | Wir haben es nun geschafft Visual Studio richtig einzurichten und haben schon etwas programmieren begonnen. Wir konnten somit schon mal die Grundstruktur erstellen und sehen, wie es etwa aussieht. Die Projektdokumentation wurde Angefangen. |
|  13.09.2024    | 0.0.3   | Wir haben nun die Optionen für die Eingaben erstellt. Zudem haben wir wieder an der Projektdokummentation gearbeitet. |
|   20.09.2024    | 0.0.4   | Wir haben das Kreisdiagramm erstellt und wir konnten es zum ersten mal austesten. Zudem wurde die Projektdokumentation einmal komplett überarbeitet und Fehler wurden behoben. |
|   27.09.2024   | 1.0.0   | Wir haben nun die Speicherung erstellt und alles restliche inkl. Feinschliff entwickelt. Die Projektdokumentation wurde erweitert.  |
|   01.11.2024    | 1.0.1   | Wir haben die Projektdokumentation fertiggestellt und die Portfolios gemacht.  |


## 1 Informieren



### 1.1 Ihr Projekt

Personal Finance Web App mit Mern Stack
Beschreibung: Eine App zur Verwaltung von Finanzen, die Benutzern hilft, ihre Ausgaben zu verfolgen, Budgets festzulegen und Sparziele zu erreichen.
Funktionen:
Benutzerregistrierung und -authentifizierung
Verfolgen von Einnahmen und Ausgaben (mit Kategorien wie Essen, Miete, Unterhaltung)
Monatliche Budgetierung und Zielverfolgung
Sparziele setzen und den Fortschritt visualisieren
Berichte und Diagramme zur finanziellen Analyse
Erinnerungen für Rechnungen und Zahlungstermine (Push-Benachrichtigungen)
Technologien: MongoDB, Express.js, React Native, Node.js, Chart.js für Diagramme, Firebase für Benachrichtigungen.








### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ          | Beschreibung                                                                 |
| ---- | --------------- | ------------ | ---------------------------------------------------------------------------- |
| 1    | Muss            | funktional   | Als Benutzer möchte ich meine Ausgaben und Einnahmen schnell und einfach hinzufügen können, um einen Überblick über mein Geld zu behalten. |
| 2    | Muss            | funktional   | Als Benutzer möchte ich meine Ausgaben in Kategorien wie "Essen", "Miete" und "Unterhaltung" aufteilen, damit ich sehe, wofür mein Geld ausgegeben wird. |
| 3    | Muss            | funktional   | Als Benutzer möchte ich ein monatliches Budget festlegen können, um meine Ausgaben besser zu kontrollieren. |
| 4    | Muss            | funktional   | Als Benutzer möchte ich Ziele für das Sparen festlegen können, damit ich für grössere Anschaffungen oder Notfälle planen kann. |
| 5    | Muss            | funktional   | Als Benutzer möchte ich Benachrichtigungen für Rechnungen erhalten, damit ich keine Zahlungen vergesse. |
| 6    | Muss            | funktional   | Als Benutzer möchte ich Diagramme sehen können, die meine Einnahmen und Ausgaben darstellen, um meine Finanzen besser zu verstehen. |
| 7    | Muss            | funktional   | Als Benutzer möchte ich regelmässig wiederkehrende Zahlungen (wie Miete) automatisch hinzufügen lassen, damit ich nicht jedes Mal daran denken muss. |
| 8    | Muss            | funktional   | Als Benutzer möchte ich benutzerdefinierte Kategorien erstellen können, damit die App auf meine Bedürfnisse passt. |
| 9    | Soll            | funktional   | Als Benutzer möchte ich eine Nachricht bekommen, sobald meine eingegebenen Rechnungen bezahlt werden müssen. |










### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  |      Programm wird geöffnet        |    Einnahmen    |        Detaillierte Ansicht der Einnahmen.          |
| 1.2  |      Programm wird geöffnet        |    Ausgaben     |        Detaillierte Ansicht der Ausgaben.           |
| 1.3  |      Programm wird geöffnet        |    Einnahmen & Ausgaben    |    Einnahmen und Ausgaben werden zusammen angezeigt, so dass man ein budget sieht.             |
| 2.1  |      Programm wird geöffnet        |    Kategorie Essen und Menge an Geld    |    Das Programm zeigt mir an, wie viel ich für Essen ausgegeben habe.              |
| 2.2  |      Programm wird geöffnet        |    Verschiedene Kategorien und Mengen an Geld    |   Das Programm zeigt mir im Kreisdiagramm an, wie viel ich für was ausgebe.               |
| 3.1  |      Programm wird geöffnet        |    Alle Einkommens und Ausgabens Daten    |   Es wird angezeigt, wie viel man für was ausgibt und woher das Geld kommt.               |
| 3.2  |      Programm wird geöffnet        |    (bezogen auf 3.1) Daten ändern    |    Die Daten wurden geändert und ich habe nun ein eigenes Budget erstellt.              |
| 4.1  |      Programm wird geöffnet        |    Menge die gespaart werden soll    |    Die gespaarte Menge wird in das Budget einberechnet.              |
| 5.1  |      Programm wird geöffnet        |    Rechnungsdatum eingeben    |   Benachrichtigung wenn die Rechnung fällig ist.               |
| 6.1  |      Programm wird geöffnet        |    Beträge    |   Das Diagramm zeigt an, für wsa ich geld ausgebe und von wo ich es einnehme.               |
| 7.1  |      Programm wird geöffnet        |    Miete    |    Die Miete wird nun automatisch jeden Monat hinzugefügt.             |
| 8.1  |      Programm wird geöffnet        |    Kategorie    |   Neue Kategorie wurde erstellt.               |
| 8.2  |      Programm wird geöffnet        |    Geld in die neue Kategorie    |  Es wird nun bei den anderen Ausgaben/Einnahmen mit dem richtigen Namen angezeigt.                |
| 9.1  |      Programm wird geöffnet        |    Rechnung eintragen    |  Es wird eine Nachricht gesendet, sobald ich meine Rechnung bezahlen muss.               |

### 1.4 Diagramme


![FinanceWebapp_Usecase](https://github.com/user-attachments/assets/d559da99-57a4-4909-bc5e-7e69baf2ddcb)


## 2 Planen

| AP-№ | Zuständig | Geplante Zeit | Beschreibung |
|------|-----------|---------------|--------------|
| 1    | Cedric    | 120 Minuten   | Grundstruktur der App erstellen (Initiale MongoDB-Datenbank, Express.js Setup, Node.js Servereinrichtung) |
| 2    | Cedric    | 90 Minuten    | Benutzerregistrierung und -authentifizierung (Backend-Implementierung mit JWT für Sicherheit) |
| 3    | Raul      | 120 Minuten   | Frontend-Setup mit React Native, Layout und Navigationsstruktur der App erstellen |
| 4    | Filip     | 90 Minuten    | Kategorien für Einnahmen und Ausgaben erstellen, API für das Hinzufügen und Abrufen von Transaktionen |
| 5    | Kenan     | 120 Minuten   | Monatsbudgetierung und Zielverfolgung, Endpunkte für Budget und Ziele hinzufügen |
| 6    | Cedric    | 60 Minuten    | Frontend-Komponenten für das Hinzufügen von Ausgaben und Einnahmen implementieren |
| 7    | Cedric    | 90 Minuten    | Backend für Kategorienverwaltung und Benutzerdefinierte Kategorien entwickeln |
| 8    | Raul      | 90 Minuten    | Frontend für Budget- und Zielsetzung mit Progress-Tracking erstellen |
| 9    | Filip     | 120 Minuten   | Push-Benachrichtigungen für Rechnungen und Zahlungstermine (Integration mit Firebase) |
| 10   | Kenan/Filip     | 120 Minuten   | Kreisdiagramm zur Darstellung der Finanzen (Integration von Chart.js und Frontend-Visualisierung) |
| 11   | Cedric    | 60 Minuten    | Funktion für automatische, regelmässig wiederkehrende Zahlungen (wie Miete) entwickeln |
| 12   | Cedric    | 60 Minuten    | Testing und Validierung der API und Endpunkte |
| 13   | Raul      | 90 Minuten    | Testing und Validierung der Benutzeroberfläche und Funktionalität |
| 14   | Filip     | 90 Minuten    | Dokumentation des Codes und API-Beschreibungen für die Entwickler und zukünftige Wartung |
| 15   | Kenan     | 60 Minuten    | Finaler Testlauf, Debugging und Vorbereitungen für die Präsentation |




## 3 Entscheiden

Für das Projekt "Personal Finance Web App" haben wir den MERN Stack gewählt, da er optimal auf die Anforderungen passt. MongoDB als NoSQL-Datenbank ermöglicht die flexible Speicherung von Finanzdaten wie Einnahmen, Ausgaben und Sparzielen. Express.js unterstützt die effiziente Kommunikation zwischen Frontend und Backend, was schnelle Ladezeiten ermöglicht. React Native erlaubt es uns, eine plattformübergreifende App für iOS und Android zu entwickeln und so eine breite Nutzerschaft anzusprechen. Node.js sorgt dafür, dass die Anwendung auch bei vielen gleichzeitigen Anfragen performant bleibt. Zudem lassen sich mit Chart.js Diagramme und Analysen visuell darstellen, und Firebase ermöglicht Push-Benachrichtigungen für Zahlungserinnerungen. Der MERN Stack bietet uns somit eine ideale Kombination aus Flexibilität, Skalierbarkeit und Benutzerfreundlichkeit für diese Finanz-App.


## 4 Realisieren


| AP-№ | Datum       | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----------- | --------- | ------------- | ----------------- |
| 1.A  | 30.08.2024  | Cedric    | 120           | 150               |
| 2.A  | 13.09.2024  | Cedric    | 90            | 60                |
| 3.A  | 20.09.2024  | Raul      | 120           | 90                |
| 4.A  | 27.09.2024  | Filip     | 90            | 120               |
| 5.A  | 01.11.2024  | Kenan     | 120           | 150               |
| 6.A  | 23.08.2024  | Cedric    | 60            | 90                |
| 7.A  | 13.09.2024  | Cedric    | 90            | 120               |
| 8.A  | 20.09.2024  | Raul      | 90            | 60                |
| 9.A  | 27.09.2024  | Filip     | 120           | 90                |
| 10.A | 01.11.2024  | Kenan     | 120           | 90                |
| 11.A | 23.08.2024  | Cedric    | 60            | 30                |
| 12.A | 13.09.2024  | Cedric    | 60            | 90                |
| 13.A | 20.09.2024  | Raul      | 90            | 120               |
| 14.A | 27.09.2024  | Filip     | 90            | 60                |
| 15.A | 01.11.2024  | Kenan     | 60            | 90                |






## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |   01.11.24   |   Funktioniert  |   Kenan Bajramovic   |
| 1.2  |  01.11.24    |   Funktioniert  |   Kenan Bajramovic   |
| 1.3  |   01.11.24   |   Funktioniert  |   Kenan Bajramovic   |
| 2.1  |   01.11.24   |   Funktioniert  |   Kenan Bajramovic   |
| 2.2  |   01.11.24   |   Funktioniert  |   Kenan Bajramovic   |
| 3.1  |   01.11.24   |   Funktioniert  |    Filip Mitrovic    |
| 3.2  |   01.11.24   |   Funktioniert  |    Filip Mitrovic    |
| 4.1  |   01.11.24   |   Funktioniert  |    Filip Mitrovic    |
| 5.1  |   01.11.24   |   Funktioniert  |    Filip Mitrovic    |
| 6.1  |   01.11.24   |   Funktioniert  |    Filip Mitrovic    |
| 7.1  |   01.11.24   |   Funktioniert  |    Filip Mitrovic    |
| 8.1  |   01.11.24   |   Funktioniert  |    Filip Mitrovic    |
| 8.2  |   01.11.24   |   Funktioniert  |   Kenan Bajramovic   |
| 9.1  |   01.11.24   |   Funktioniert nicht |   Kenan Bajramovic   |


`Fazit:`
Das Projekt ist äusserst erfolgreich verlaufen, alle Ziele wurden erreicht. Das Programm funktioniert einwandfrei und ermöglicht es den Benutzern, sowohl Text als auch Bilder zu verschlüsseln und wieder zu entschlüsseln.
