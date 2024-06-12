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
Die Kunden können Feedback über das Unternehmen geben und die Daten werden gespeichert.
✍️ Beschreiben Sie Ihr Projekt in einem griffigen Satz.

✍️ Erklären Sie genauer in 50 bis 100 Wörtern, was genau Sie in diesem Projekt erreichen möchten, und was Sie dabei zu lernen hoffen.
In diesem Projekt geht es darum, das ich eine fikitive Unternehmenswebsite erstelle. Danach können die Kunden ihre Bewertung hinterlassen. Diese Bewertung/Daten werden in MongoDB gepspeichert. Ich werde also den MongoDB kennenlernen.


### 1.2 Anforderungen

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1 | muss | Qualität | Es muss einen Unternehmens Website erstellt werden. |
| 2  | muss | Qualität | Die Website muss schön dargestellt werden. |
| 3  | muss | Funktionalität | Die Website soll Informationen des Unternehmen zur verfügung stellen. |
| 4  | muss | Funktionalität | Es muss eine Bewertungmöglichkeit haben. |
| 5  | muss | Funktionalität | Es muss eine Möglichkeit geben, mit Sterne zu bewerten.|
| 6  | muss | Funktionalität | Ich kann für dieses Website Feedback schreiben und senden. |
| 7  | muss | Funktionalität | Ich kann für dieses Website ein Feedback Löschen bzw. auch das "Löschen" bestätigen. |
| 8  | muss | Randbedingung | Für diese entwicklung soll in C# geschrieben werden. |
| 9  | muss | Funktionalität | Wenn ich etwas falsches eingebe beim Email/Name oder etwas nicht hingeschrieben habe, soll angezeigt werden, was ich wirklich eingeben soll. |
| 10  | muss | Funktionalität | Es sollen zwei Buttons geben, um Feedback-seite oder Startseite zu gelangen. |

✍️ Jede User Story hat eine ganzzahlige Nummer (1, 2, 3 etc.), eine Verbindlichkeit (Muss oder Kann?), und einen Typ (Funktional, Qualität, Rand). Die User Story selber hat folgende Form: *Als ein 🤷‍♂️ möchte ich 🤷‍♂️, damit 🤷‍♂️*.

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
| ...  |              |         |                   |


✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, die der Testfall abdeckt, und `m` von `1` an nach oben gezählt. Beispiel: Der dritte Testfall, der die zweite User Story abdeckt, hat also die Nummer `2.3`.

### 1.4 Diagramme

✍️Fügen Sie hier ein Use Case-Diagramm mit mindestens 10 Anwendungsfällen ein; und einen PAP.

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


Total: 

✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, auf die sich das Arbeitspaket bezieht, und `m` von `A` an nach oben buchstabiert. Beispiel: Das dritte Arbeitspaket, das die zweite User Story betrifft, hat also die Nummer `2.C`.

✍️ Ein Arbeitspaket sollte etwa 45' für eine Person in Anspruch nehmen. Die totale Anzahl Arbeitspakete sollte etwa Folgendem entsprechen: `Anzahl R-Sitzungen` ╳ `Anzahl Gruppenmitglieder` ╳ `4`. Wenn Sie also zu dritt an einem Projekt arbeiten, für welches zwei R-Sitzungen geplant sind, sollten Sie auf `2` ╳ `3` ╳`4` = `24` Arbeitspakete kommen. Sollten Sie merken, dass Sie hier nicht genügend Arbeitspakte haben, denken Sie sich weitere "Kann"-User Stories für Kapitel 1.2 aus.

## 3 Entscheiden

✍️ Dokumentieren Sie hier Ihre Entscheidungen und Annahmen, die Sie im Bezug auf Ihre User Stories und die Implementierung getroffen haben.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  | 22.05.2024 | Sathana | 45min | 60min |
| 2.A  | 05.06.2024 | Sathana | 3 x 45min | 3 x 45min |
| 3.A  | 05.06.2024 | Sathana | 2 x 45min | 2 x 45min |
| 4.A  | 22.05.2024 | Sathana | 2 x 45min | 60min |
| 5.A  | 29.05.2024 | Sathana | 45min | - |
| 6.A  | 22.05.2024 | Sathana | 2 x 45min | 2 x 45min |
| 7.A  | 29.05.2024 | Sathana | 45min | 2 x 45min |
| 9.A  | 29.05.2024 | Sathana | 45min | 2 x 45min |
| 10.A | 05.06.2024 | Sathana | 45min | 55min |



✍️ Tragen Sie jedes Mal, wenn Sie ein Arbeitspaket abschließen, hier ein, wie lang Sie effektiv dafür hatten.

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
| ...  |       |          |        |

Das Programm wurde auf einem HP Windows 11 Pro getestet. Alle Tests wurden bestanden. Es gibt eine Anforderung "5", welche nicht implemenitert wurde, jedoch kann man das ohne diese implementierung diese Website nutzen. 
