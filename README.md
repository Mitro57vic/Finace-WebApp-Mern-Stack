# Finace-WebApp-Mern-Stack


# Projekt-Dokumentation



Filip Mitrovic, Cedric Tuma, Raul Gilardoni und Kenan Bajramovic

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|   23.08.2024    | 0.0.1   |  Wir haben uns für ein Finance Webapp entschieden zu implementieren mit Mern Stack und uns darüber informiert. Wir haben begonnen Visual Studio zu Einrichten für unser Projekt. Bei der Einrichtung sind wir auf viele Problemen zugestossen, aber haben auch viel dazugelernt. Die Konfiguartion ist bis jetzt ohne Erfolg.|
|   30.08.2024   | 0.0.2   | Wir haben es nun geschafft Visual Studio richtig einzurichten und haben schon etwas programmieren begonnen. Wir konnten somit schon mal die Grundstruktur erstellen und sehen, wie es etwa aussieht. |
|  13.09.2024    | 0.0.3   |   |
|   20.09.2024    | 0.0.4   |  |
|   27.09.2024   | 0.0.5   |   |
|   01.11.2024    | 1.0.0   |  |


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


### 1.4 Diagramme


![FinanceWebapp_Usecase](https://github.com/user-attachments/assets/d559da99-57a4-4909-bc5e-7e69baf2ddcb)


## 2 Planen

| AP-№ | Zuständig | geplante Zeit | Beschreibung |
| ---- |  --------- | ------------ | ------------- |
| 1.A  |               | 60           |             |
| 2.A  |                  |  60            |                 |
| 3.A  |                  |   30         |           |
| 4.A  |                  |  60            |                  |



## 3 Entscheiden

Für das Projekt "Personal Finance Web App" haben wir den MERN Stack gewählt, da er optimal auf die Anforderungen passt. MongoDB als NoSQL-Datenbank ermöglicht die flexible Speicherung von Finanzdaten wie Einnahmen, Ausgaben und Sparzielen. Express.js unterstützt die effiziente Kommunikation zwischen Frontend und Backend, was schnelle Ladezeiten ermöglicht. React Native erlaubt es uns, eine plattformübergreifende App für iOS und Android zu entwickeln und so eine breite Nutzerschaft anzusprechen. Node.js sorgt dafür, dass die Anwendung auch bei vielen gleichzeitigen Anfragen performant bleibt. Zudem lassen sich mit Chart.js Diagramme und Analysen visuell darstellen, und Firebase ermöglicht Push-Benachrichtigungen für Zahlungserinnerungen. Der MERN Stack bietet uns somit eine ideale Kombination aus Flexibilität, Skalierbarkeit und Benutzerfreundlichkeit für diese Finanz-App.


## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A   |        |                |  60          |       60       |





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


`Fazit:`
Das Projekt ist äusserst erfolgreich verlaufen, alle Ziele wurden erreicht. Das Programm funktioniert einwandfrei und ermöglicht es den Benutzern, sowohl Text als auch Bilder zu verschlüsseln und wieder zu entschlüsseln.
