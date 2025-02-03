# Dataset Characteristics
# Dataset Characteristics
This folder contains the scripts and notebooks used for analyzing the characteristics of the bakery sales dataset. The tasks include examining missing values, generating histograms, and performing descriptive statistics on various aspects of the data. The following notes describe what was done in each file:

## INSTRUCTIONS.md
The file [INSTRUCTIONS.md](1_DatasetCharacteristics/INSTRUCTIONS.md) provides an overview and guidelines for analyzing the dataset characteristics. It describes the key topics to focus on, including handling missing values, generating histograms, and performing descriptive statistics on different variables.

## Dataset Characteristics Notebooks
1. **MISSING_VALUES.ipynb**
   - Analyzes missing values in the dataset, identifies columns with missing data, and displays rows with missing values for specific columns.
2. **HISTOGRAMME_UMSATZ.ipynb**
   - Generates histograms for sales data (`Umsatz`) and performs dummy encoding for product groups (`Warengruppe`).
3. **DESCR_STATISTICS_WOCHENTAGE.ipynb**
   - Analyzes sales data by weekdays, creates one-hot encoding for weekdays, and visualizes average sales per weekday.
4. **DESCR_STATISTICS_WETTER.ipynb**
   - Provides descriptive statistics for weather-related columns (`Bewoelkung`, `Temperatur`, `Windgeschwindigkeit`, `Wettercode`) and generates appropriate graphs.
5. **DESCR_STATISTICS_WARENGRUPPE.ipynb**
   - Analyzes sales data by product groups (`Warengruppe`), calculates summary statistics, and visualizes average and total sales per product group.
6. **DESCR_STATISTICS_OTHER.ipynb**
   - Analyzes sales data during the Kiel Week and other events, calculates average sales per product group during these events, and visualizes the results.
7. **DESCR_STATISTICS_EVENTS.ipynb**
   - Examines the impact of various events (e.g., national holidays, Christmas market) on sales, merges event data with sales data, and visualizes the influence of events on sales.

Overall, this folder ensures that all relevant characteristics of the dataset are thoroughly analyzed, providing valuable insights for further modeling and forecasting.