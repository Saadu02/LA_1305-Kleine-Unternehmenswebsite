# LA_1305-Fiktives-Unternehmen

fiktives Unternehmen von Sathana Suganthasri

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
| 15.05.2024 | 0.0.1 | Über das Projekt informiert.|
| 15.05.2024 | 0.0.2   | Anforderungen, Skizze und Planung erstellt. |
| 29.05.2024 | 0.0.3   | Testfälle erstellt. |
| 05.06 2024 | 0.0.4   | Das Projekt fertig programmiert. |
| 12.06.2024 | 0.0.5   | Dokumentation fertig erstellt. |



## 1 Informieren

### 1.1 Ihr Projekt
Die Kunden können Feedback zum Unternehmen geben, und die Daten werden gespeichert.


In diesem Projekt möchte ich eine fiktive Unternehmenswebsite erstellen, auf der Kunden ihre Bewertungen hinterlassen können. Diese Bewertungen werden dann in einer MongoDB-Datenbank gespeichert. Ziel ist es, mehr über den Umgang mit MongoDB zu lernen. Zusätzlich uach meine Kenntnisse in den Programmiersprachen C# und JavaScript zu erweitern und zu vertiefen. Durch die Integration dieser Technologien möchte ich mein Verständnis für die Webentwicklung verbessern und lernen, wie man eine funktionale und benutzerfreundliche Website erstellt.

### 1.2 Anforderungen

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1 | muss | Qualität | Es muss eine Unternehmenswebsite erstellt werden. |
| 2  | muss | Qualität | Die Website muss ansprechend gestaltet sein. |
| 3  | muss | Funktionalität | Die Website soll Informationen über das Unternehmen zur Verfügung stellen. |
| 4  | muss | Funktionalität | Es muss eine Bewertungsmöglichkeit geben. |
| 5  | muss | Funktionalität | Es muss die Möglichkeit geben, mit Sternen zu bewerten. |
| 6  | muss | Funktionalität | Ich kann auf dieser Website Feedback schreiben und senden. |
| 7  | muss | Funktionalität | Ich kann auf dieser Website ein Feedback löschen und das Löschen bestätigen. |
| 8  | muss | Randbedingung | Für diese Entwicklung soll in C# programmiert werden. |
| 9  | muss | Funktionalität | Wenn ich etwas Falsches beim E-Mail/Name eingebe oder etwas nicht ausgefüllt habe, soll angezeigt werden, was ich wirklich eingeben soll. |
| 10  | muss | Funktionalität | Es sollen zwei Buttons vorhanden sein, um zur Feedback-Seite oder zur Startseite zu gelangen. |
| 11  | kann | Funktionalität | Die Website muss auch in einer mobilen Version nutzbar sein. |


### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 3.1  | Website wird gestartet | klickt auf "Startseite" | Unternehmungs informationen |
| 4.1  | Feedback-Seite | Name: Petra, E-Mail: petra@gmail.com, Nachricht: Gutes Unternehmung | Bedankens-Seite|
| 6.1  | Feedback-Seite | Name: Sandra, E-Mail: sandra@hotmail.com, Nachricht: Tolle Mitarbeiter --> "Feedback absenden" | Bedankens-Seite|
| 7.1  | Feedback-Seite | klickt auf "Löschen" | Möchten Sie dieses Feedback wirklich löschen? |
| 7.2  | Dialog mit "Möchten Sie dieses Feedback wirklich löschen?" | klickt auf das Button "OK ". | Feedback wird gelöscht. |
| 7.3  | Dialog mit "Möchten Sie dieses Feedback wirklich löschen?" | klickt auf das Button "Abbrechen ". | Feedback wird nicht gelöscht. |
| 9.1  | Feedback-Seite | Name:  , E-Mail: meier@hotmail.com, Nachricht: schönes Website --> "Feedback absenden" | Fülle dieses Feld aus.|
| 9.2  | Feedback-Seite | Name: Meier, E-Mail: meierhotmail.com, Nachricht: schönes Website --> "Feedback absenden" | Fie E-Mail-Adresse muss ein @-Zeichen enthalten. In der Angabe "meierhotmail.com" fehlt ein @-Zeichen.|
| 9.3  | Feedback-Seite | Name: Meier, E-Mail: meierhotmail.com, Nachricht: schönes Website --> "Feedback absenden" | Nach dem @-Zeichen darf das Zeichen "#" nicht verwendet werden.|
| 10.1  | Startseite | klickt auf das Button  "Feedback"| Feedback-Seite wird angezeigt. |
| 10.2  | Feedback-Seite | klickt auf das Button  "Startseite"| Startseite wird angezeigt. |


### 1.4 Diagramme

Startseite:
![Startseite](https://github.com/Saadu02/LA_1305-Kleine-Unternehmenswebsite/assets/111046257/c05ee56c-4f1e-402c-a834-72e40435aaf8)


Feedback-Seite:
![Feedback](https://github.com/Saadu02/LA_1305-Kleine-Unternehmenswebsite/assets/111046257/834c4a35-f5ac-4d92-9b27-011c4b3a711d)


Bedanken-Seite:
![BedankenSeite](https://github.com/Saadu02/LA_1305-Kleine-Unternehmenswebsite/assets/111046257/b277bf27-cf0d-4324-8543-7b66bd95e48f)


## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  | 22.05.2024 | Sathana | Website erstellen | 45min |
| 2.A  | 05.06.2024 | Sathana | Design | 3 x 45min |
| 3.A  | 05.06.2024 | Sathana | Information der Unternehmen | 2 x 45min|
| 4.A  | 22.05.2024 | Sathana | Feedback erstellen | 2 x 45min |
| 5.A  | 29.05.2024 | Sathana | Sterne bewertung | 45min|
| 6.A  | 22.05.2024 | Sathana | Feedback schreiben & senden (DB) | 2 x 45min |
| 7.A  | 29.05.2024 | Sathana | Feedback Löschen | 45min |
| 9.A  | 29.05.2024 | Sathana | Fehlermeldung-Box | 45 min|
| 10.A | 29.05.2024 | Sathana | Buttons | 45 min|
| 11.A | 05.06.2024 | Sathana | Mobile-Version | 45 min|


## 3 Entscheiden

Ich habe mich entschieden, Visual Studio Code zu nutzen, da es eine ausgezeichnete Anwendung zur Erstellung von Websites bietet. Zudem habe ich mich für die Programmiersprachen C# und JavaScript entschieden. Als Datenbank habe ich MongoDB ausgewählt. Ich habe auch geplant meine Website auch auf Mobile-Version nutzbar zu machen.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  | 22.05.2024 | Sathana | 45min | 60min |
| 2.A  | 05.06.2024 | Sathana | 3 x 45min | 2 x 45min |
| 3.A  | 05.06.2024 | Sathana | 2 x 45min | 2 x 45min |
| 4.A  | 22.05.2024 | Sathana | 2 x 45min | 60min |
| 5.A  | 29.05.2024 | Sathana | 45min | - |
| 6.A  | 22.05.2024 | Sathana | 2 x 45min | 2 x 45min |
| 7.A  | 29.05.2024 | Sathana | 45min | 2 x 45min |
| 9.A  | 29.05.2024 | Sathana | 45min | 2 x 45min |
| 10.A | 05.06.2024 | Sathana | 45min | 55min |
| 11.A | 05.06.2024 | Sathana | 45min | 25min |


## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 3.1  | 12.06.2024 | OK | Sathana Suganthasri |
| 4.1  | 12.06.2024 | OK | Sathana Suganthasri |
| 6.1  | 12.06.2024 | OK | Sathana Suganthasri |
| 7.1  | 12.06.2024 | OK | Sathana Suganthasri |
| 7.2  | 12.06.2024 | OK | Sathana Suganthasri |
| 7.3  | 12.06.2024 | OK | Sathana Suganthasri |
| 9.1  | 12.06.2024 | OK | Sathana Suganthasri |
| 9.2  | 12.06.2024 | OK | Sathana Suganthasri |
| 9.3  | 12.06.2024 | OK | Sathana Suganthasri |
| 10.1 | 12.06.2024 | OK | Sathana Suganthasri |
| 10.2 | 12.06.2024 | OK | Sathana Suganthasri |

Das Programm wurde auf einem HP Windows 11 Pro getestet und hat alle Tests bestanden. Es gibt eine Anforderung, 
nämlich Anforderung nr."5", die nicht implementiert wurde. Dennoch ist die Website auch ohne diese Implementierung 
nutzbar.
