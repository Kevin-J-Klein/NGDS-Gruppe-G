# Gruppenarbeit Projekt

## Einleitung

Wir führen eine projektbasierte Gruppenarbeit durch. Es wird in 3er-Gruppen gearbeitet, die zufällig zugeteilt wurden, siehe Moodle-Kurs. Die Bewertung erfolgt pro Gruppe und geht mit einem Gewicht von 40% in die Modulnote ein.

Im Projekt geht es um Wetterdaten und jeder Gruppe wird eine Wetterstation zugeteilt. Die Daten werden als CSV-Dateien im Verzeichnis `Projekt/Daten` im GitHub Repo zur Verfügung gestellt werden. Sie beinhalten folgende Messwerte über ein ganzes Jahr:

|  Header   |        Bedeutung        |  Einheit   |
| :-------: | :---------------------: | :--------: |
|    stn    |      Wetterstation      |     -      |
|   time    |       Zeitstempel       | `datetime` |
| prestah0  |        Luftdruck        |    hPa     |
| tre200h0  |       Temperatur        |     °C     |
| rre150h0  |       Regenmenge        |     mm     |
| su2000h0  |      Sonnenstunden      |     %      |
| time_diff | Stunden seit Messbeginn |     h      |

Die Zuordnung der Wetterstationen auf die Gruppen findet ihr in der Datei `Gruppen_Stationen.csv`.

## Auftrag

Im Projekt sollt ihr folgende Punkte abarbeiten:

1. Import der Daten
   - Beschreibt die Datenstruktur.
   - Zeigt auf, wie viele Messungen es sind.

2. Da einige Datenpunkte fehlen, müsst ihr diese interpolieren.
   - Wählt dazu eine geeignete Methode und begründet eure Wahl.
   - Führt die Methode durch, um eine interpolierte Version der Daten mit mindestens doppelt so vielen Punkten zu erzeugen.

3. Ihr sollt alle Variablen (Luftdruck, Temperatur, Regenmenge und Sonnenstunden) über einen selbstgewählten Zeitraum darstellen. 
   - Basisvariante: Wähle einen interessanten Zeitraum von 1-2 Wochen.
   - Schwierigere Variante (mehr Punkte): Errechne tageweise Durchschnitte, um die Variablen in einem grösseren Zeitraum (mehrere Monate/Quartal) darzustellen.

4. Für die folgenden Punkte sollt ihr eine der Variablen auswählen.
   - Entweder Luftdruck, Temperatur, Regenmenge oder Sonnenstunden

5. Vergleicht die ursprünglichen Daten mit den interpolierten Daten und zeigt eure Erkenntnisse auf. 
   - Hier könnt ihr euch z.B. fragen, wie sich unterschiedliche Interpolationsmethoden verhalten.

6. Berechnet Nullstellen bzw. Schnittpunkte mit einem Schwellenwert und überlegt euch, welche Aussagen ihr daraus ableiten könnt.
   - Ihr könntet z.B. sagen: "In Davos hatten wir im Winter X-mal weniger als Null Grad." oder "An welchen Tagen wurde die Regenmenge XY erreicht?".

7. Mithilfe der Ableitung soll nach grossen Änderungen in den Daten gesucht werden. 
   - So könnt ihr z.B. sagen: "Am Tag X hatten wir die grösste Änderungsrate des Luftdrucks".

8. Benutze die Integration, um gewisse Durchschnittswerte über einen definierten Zeitraum zu berechnen.
   - So könnt ihr z.B. die durchschnittlichen Sonnenstunden über den Sommer aufzeigen.

Die gegebenen Beispiele sollen als Anhaltspunkte dienen.

## Abgabe

- Die Abgabe erfolgt über Moodle: [Abgabe Projekt](https://moodle.zhaw.ch/mod/assign/view.php?id=829823).
- Es sollen die PowerPoint-Präsentation in PDF-Form und ein gut dokumentiertes Jupyter-Notebook abgegeben werden.
- Der Zeitraum zur Abgabe ist Mittwoch, 17. Mai 2023, 00:00 bis Mittwoch, 24. Mai 2023, 23:59.

## Präsentation

- Die Präsentationen finden Donnerstag, 25. Mai 2023, und Freitag, 26. Mai 2023, statt.
- Die Präsentation sollte maximal 10 Minuten dauern und die wichtigsten Erkenntnisse und Ergebnisse eures Projekts darstellen.
- Alle Gruppenmitglieder sollen gleichwertig zur Präsentation beitragen.
- Verwendet ansprechende Visualisierungen, um eure Ergebnisse zu präsentieren. Diese sollten leicht verständlich sein und eure Erkenntnisse veranschaulichen.
- Zeigt nur Code, wenn es wirklich der Erklärung hilft.
- Verwendet eine klare und verständliche Sprache, um eure Ergebnisse zu erklären.
- Nutzt die Möglichkeit, Fragen des Publikums zu beantworten und geht auf Feedback ein.

## Jupyter-Notebook

- Achtet darauf, dass euer Code gut strukturiert und kommentiert ist, um anderen Personen ein einfaches Verstehen zu ermöglichen.
- Erklärt in Markdown Zellen euer Vorgehen und interpretiert die Ergebnisse.
- Das Notebook soll in dem Ordner `Projekt` laufen und relativ dazu die CSV-Dateien importieren.
- Achtet darauf, dass eure Visualisierungen ansprechend und leicht verständlich sind. 
- Fügt am Ende des Notebooks eine Zusammenfassung eurer wichtigsten Ergebnisse und Erkenntnisse ein.
- Die Gruppenarbeit soll abschliessend hinsichtlich Zusammenarbeit, Rollenverteilung und Einschätzung der individuellen Beiträge reflektiert werden (am Ende des Jupyter Notebooks).

Wir hoffen, diese Anweisungen sind hilfreich. Bei Fragen oder Problemen stehen wir euch gerne zur Verfügung.
