# Data Preparation

In diesem Ordner befinden sich die Skripte und Notebooks, die für die Datenvorbereitung des Bäckerei-Umsatzprognoseprojekts verwendet wurden. Eine effiziente und genaue Datenvorbereitung ist grundlegend für erfolgreiche Prognosemodelle. Die Aufgaben umfassen das Importieren des Datensatzes, das Bereinigen der Daten und das Erstellen neuer Variablen, die für die Umsatzprognose relevant sind. Im Folgenden wird beschrieben, was in den einzelnen Dateien gemacht wurde:

## INSTRUCTIONS.md

Die Datei [`INSTRUCTIONS.md`](0_DataPreparation/INSTRUCTIONS.md) bietet eine Übersicht und Richtlinien für den Datenvorbereitungsprozess. Sie beschreibt die wichtigsten Themen, auf die man sich konzentrieren sollte, einschließlich Datenimport, Zusammenführen von Daten aus verschiedenen Quellen, Datenbereinigung, Umgang mit fehlenden Werten, Erstellen neuer Variablen und Datentransformation.

## Datenimport und Vorbereitung Notebooks

1. **DATA_IMPORT.ipynb**
   - Dieses Notebook importiert Daten von externen Quellen und speichert sie als CSV-Dateien. Es führt eine erste Datenexploration und Visualisierung durch und führt die Umsatzdaten mit den Daten der Kieler Woche und den Wetterdaten zusammen.

2. **DATA_PREP_WETTER.ipynb**
   - Dieses Notebook konzentriert sich auf die Vorbereitung der Wetterdaten. Es umfasst Schritte zum Einlesen der Wetterdaten, Umgang mit fehlenden Werten, Erstellen von Bins für Bewölkung und Temperatur sowie das Konvertieren von booleschen Dummy-Variablen in Ganzzahlen. Es kategorisiert auch Wettercodes in beschreibende Kategorien.

3. **DATA_PREP_WARENGRUPPEN.ipynb**
   - Dieses Notebook bereitet die Daten der Warengruppen vor, indem es Dummy-Variablen für verschiedene Warengruppen erstellt und die bereinigten Daten speichert.

4. **DATA_PREP_SCHIFFAHRTSDATEN.ipynb**
   - Dieses Notebook behandelt die Vorbereitung der Schifffahrtsdaten. Es umfasst Schritte zum Einlesen der Daten mit verschiedenen Kodierungen, Filtern relevanter Spalten und Umbenennen von Spalten zur Konsistenz.

5. **DATA_PREP_MERGE.ipynb**
   - Dieses Notebook führt verschiedene vorbereitete Datensätze zusammen, einschließlich Umsatzdaten, Kieler Woche, Schifffahrtsdaten, Wetterdaten und Wochentagsdaten. Es speichert den zusammengeführten Datensatz und teilt ihn in Trainings- und Testdatensätze auf.

6. **DATA_PREP_KIWO_WOCHENTAGE.ipynb**
   - Dieses Notebook bereitet Daten im Zusammenhang mit der Kieler Woche und den Wochentagen vor. Es extrahiert relevante Spalten und speichert die bereinigten Daten.

7. **DATA_PREP_EVENTS.ipynb**
   - Dieses Notebook bereitet Ereignisdaten vor, indem es Feiertage und andere relevante Ereignisse in den Datensatz integriert und die bereinigten Daten speichert.

Insgesamt stellt dieser Ordner sicher, dass alle relevanten Daten für die Umsatzprognose korrekt importiert, bereinigt und vorbereitet werden, um eine solide Grundlage für die Modellierung zu schaffen.