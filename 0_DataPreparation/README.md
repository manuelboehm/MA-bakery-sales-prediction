# Data Preparation
This folder contains the scripts and notebooks used for data preparation of the bakery sales forecast project. The tasks include importing the dataset, cleaning the data, and creating new variables relevant for sales forecasting. The following notes describe what was done in each file:

## INSTRUCTIONS.md
The file [`INSTRUCTIONS.md`](0_DataPreparation/INSTRUCTIONS.md) provides an overview and guidelines for the data preparation process. It describes the key topics to focus on, including data import, merging data from different sources, data cleaning, handling missing values, creating new variables, and data transformation.

## Data Import and Preparation Notebooks
1. **DATA_IMPORT.ipynb**
   - Imports data from external sources and saves them as CSV files.
2. **DATA_PREP_WETTER.ipynb**
   - Prepares the weather data, creates bins for cloud cover and temperature, converts boolean dummy variables to integers, and categorizes weather codes.
3. **DATA_PREP_UMSATZ_WARENGRUPPE.ipynb**
   - Prepares the product group sales data by creating dummy variables for different product groups.
4. **DATA_PREP_SCHIFFAHRTSDATEN.ipynb**
   - Prepares the shipping data by testing different encodings, filtering relevant columns, and renaming columns.
5. **DATA_PREP_MERGE.ipynb**
   - Merges various prepared datasets, including sales data, Kiel Week, shipping data, weather data, and weekday data, and saves the merged dataset.
6. **DATA_PREP_MERGE_v2.ipynb (NOT USED)**
   - Update of data_prep_merge_v2. However, it is not used.
7. **DATA_PREP_EVENTS.ipynb**
   - Integrates holidays and other relevant events into the dataset and saves the cleaned data.
8. **DATA_PREP_KIWO.ipynb**
   - Prepares data related to Kiel Week, creates a complete date series, and replaces missing values.
9. **DATA_PREP_WOCHENTAGE.ipynb**
   - Extracts weekday information and saves the cleaned data.
10. **DATA_PREP_NEURAL_NETWORK.ipynb**
    - Prepares the data for use in a neural network by removing irrelevant columns.

Overall, this folder ensures that all relevant data for sales forecasting is correctly imported, cleaned, and prepared to create a solid foundation for modeling.