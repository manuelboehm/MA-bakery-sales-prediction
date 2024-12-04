# Dokumentation Lineares Baseline Model 
Diese lineare Regressionsmodell zielt darauf ab, die abhängige Variable `Umsatz` (Verkäufe) unter Verwendung verschiedener unabhängiger Variablen vorherzusagen. Das Modell berücksichtigt die folgenden Variablen:

1. **Produktkategorien**:
   - `Brot`: Verkäufe von Brot.
   - `Broetchen`: Verkäufe von Brötchen.
   - `Croissant`: Verkäufe von Croissants.
   - `Konditorei`: Verkäufe von Konditoreiwaren.
   - `Kuchen`: Verkäufe von Kuchen.
   - `Saisonbrot`: Verkäufe von saisonalem Brot.

2. **Ereignisse und Feiertage**:
   - `national_holiday`: Indikator für nationale Feiertage.
   - `christmas_market`: Indikator für das Vorhandensein eines Weihnachtsmarktes.
   - `KielerWoche`: Indikator für das Ereignis Kieler Woche.

3. **Wetterbedingungen**:
   - `Schifffahrt`: Indikator für Schifffahrtsaktivitäten.
   - `bewoelkt_bins_bewoelkt_1mäßig_3_5`: Indikator für mäßige Bewölkung.
   - `bewoelkt_bins_bewoelkt_2stark_6_8`: Indikator für starke Bewölkung.
   - `temp_bins_kalt`: Indikator für kalte Temperaturen.
   - `temp_bins_mild`: Indikator für milde Temperaturen.
   - `temp_bins_warm`: Indikator für warme Temperaturen.
   - `temp_bins_heiß`: Indikator für heiße Temperaturen.
   - `wind_bins_Wind`: Indikator für windige Bedingungen.
   - `wind_bins_Sturm`: Indikator für stürmische Bedingungen.
   - `Wettercode_2_leichter_niederschlag`: Indikator für leichten Niederschlag.
   - `Wettercode_3_starker_niederschlag`: Indikator für starken Niederschlag.
   - `Wettercode_4_gewitter`: Indikator für Gewitter.

4. **Zeitvariablen**:
   - `Monat`: Monat des Jahres.
   - `Wochentag_Di`: Indikator für Dienstag.
   - `Wochentag_Mi`: Indikator für Mittwoch.
   - `Wochentag_Do`: Indikator für Donnerstag.
   - `Wochentag_Fr`: Indikator für Freitag.
   - `Wochentag_Sa`: Indikator für Samstag.
   - `Wochentag_So`: Indikator für Sonntag.

Diese Variablen werden verwendet, um ein lineares Regressionsmodell zu erstellen, das den `Umsatz` (Verkäufe) der Bäckerei vorhersagt. Die Zusammenfassung des angepassten Modells liefert wichtige Kennzahlen wie R-Quadrat, Koeffizienten und p-Werte, die helfen, die Bedeutung und den Einfluss jeder Variablen auf die Zielvariable `Umsatz` zu verstehen.