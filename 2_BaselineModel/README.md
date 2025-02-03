## Baseline Model
This folder contains the scripts and notebooks used for building and evaluating the baseline linear model for the bakery sales forecast project. The tasks include importing the dataset, fitting a linear regression model, making predictions, and preparing the results for Kaggle submission. The following notes describe what was done in each file:

### INSTRUCTIONS.md
The file INSTRUCTIONS.md provides an overview and guidelines for building the baseline model. It describes the key steps to focus on, including data import, model fitting, making predictions, and preparing the results for submission.

### Linear Model Notebook
#### LINEAR_MODEL.ipynb
1. **Preparation**:
   - Imports necessary libraries such as `pandas` and `statsmodels`.
   - Reads the training dataset (`df_training_neural_network.csv`) for model building.

2. **Building the Linear Model**:
   - Fits a linear regression model using `statsmodels` with `Umsatz` as the dependent variable and various features (e.g., product groups, months, holidays, weather conditions) as independent variables.
   - Outputs the summary of the fitted model, including key metrics such as R-squared, coefficients, and p-values.

3. **Create Predictions**:
   - Loads the test dataset (`df_test_neural_network.csv`).
   - Uses the fitted model to predict `Umsatz` for the test dataset.
   - Saves the predictions in a CSV file (`df_predictions_linearModel.csv`).

4. **Prepare Kaggle-Upload**:
   - Loads the predictions file.
   - Replaces any NaN values in the `Umsatz` column with 0.
   - Keeps only the `id` and `Umsatz` columns for submission.
   - Saves the final dataframe as `df_kaggle_upload_linearModel.csv`.

Overall, this folder ensures that a baseline linear model is correctly built, evaluated, and the predictions are prepared for submission to Kaggle.

### Variables Used in the Linear Model
1. **Product Categories**:
   - `Brot`: Sales of bread.
   - `Broetchen`: Sales of rolls.
   - `Croissant`: Sales of croissants.
   - `Konditorei`: Sales of confectionery products.
   - `Kuchen`: Sales of cakes.

2. **Events and Holidays**:
   - `national_holiday`: Indicator for national holidays.
   - `christmas_market`: Indicator for the presence of a Christmas market.
   - `KielerWoche`: Indicator for the Kiel Week event.

3. **Weather Conditions**:
   - `temp_bins_kalt`: Indicator for cold temperatures.
   - `temp_bins_mild`: Indicator for mild temperatures.
   - `temp_bins_warm`: Indicator for warm temperatures.
   - `temp_bins_heiß`: Indicator for hot temperatures.

4. **Time Variables**:
   - `Monat_2`: February.
   - `Monat_3`: March.
   - `Monat_4`: April.
   - `Monat_5`: May.
   - `Monat_6`: June.
   - `Monat_7`: July.
   - `Monat_8`: August.
   - `Monat_9`: September.
   - `Monat_10`: October.
   - `Monat_11`: November.
   - `Monat_12`: December.
   - `Wochentag_Di`: Indicator for Tuesday.
   - `Wochentag_Mi`: Indicator for Wednesday.
   - `Wochentag_Do`: Indicator for Thursday.
   - `Wochentag_Fr`: Indicator for Friday.
   - `Wochentag_Sa`: Indicator for Saturday.
   - `Wochentag_So`: Indicator for Sunday.