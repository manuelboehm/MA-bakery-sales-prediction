# Model Definition and Evaluation


## Model Definition and Evaluation
This folder contains the scripts and notebooks used for building and evaluating the neural network model for the bakery sales forecast project. The tasks include importing the dataset, defining the neural network architecture, training the model, making predictions, and preparing the results for Kaggle submission. The following notes describe what was done in each file:

### INSTRUCTIONS.md
The file INSTRUCTIONS.md provides an overview and guidelines for building the neural network model. It describes the key steps to focus on, including model selection, feature engineering, hyperparameter tuning, implementation, and evaluation metrics.

### Installation and Setup
#### INSTALLATION NUMPY.ipynb
1. **Install Dependencies**:
   - Installs specific versions of `numpy` and `tensorflow`.
   - Verifies the installation by printing the versions of the installed packages.

Overall, this folder ensures that a neural network model is correctly built, evaluated, and the predictions are prepared for submission to Kaggle.

### Neural Network Model Notebooks
#### NEURONALES MODELL.ipynb (NOT USED)
1. **Data Preparation**:
   - Imports necessary libraries such as `pandas` and `numpy`.
   - Reads the training, validation, and test datasets (`df_training_neural_network.csv`, `df_validation_neural_network.csv`, `df_test_neural_network.csv`).
   - Separates features and labels for training, validation, and test datasets.
   - Exports the prepared data as pickle files for later use.

2. **Model Definition**:
   - Defines a neural network using Keras with batch normalization and dense layers.
   - Compiles the model using Mean Squared Error (MSE) as the loss function and Adam optimizer.
   - Trains the model using the training data and evaluates it using the validation data.

3. **Model Evaluation**:
   - Saves the trained model.
   - Plots the training and validation loss over epochs.
   - Makes predictions on the training and validation sets.
   - Evaluates the model's performance using Mean Absolute Percentage Error (MAPE).

4. **Visualization**:
   - Visualizes the predicted versus actual values for training and validation data.

#### NEURONALES MODELL_v2.ipynb
1. **Data Preparation**:
   - Similar steps as NEURONALES MODELL.ipynb for importing and preparing the data.

2. **Model Definition**:
   - Defines a neural network with additional preprocessing steps such as scaling the features using `StandardScaler`.
   - Adds dropout layers to the model for regularization.
   - Compiles and trains the model with learning rate scheduling and early stopping callbacks.

3. **Model Evaluation**:
   - Saves the trained model.
   - Plots the training and validation loss over epochs.
   - Makes predictions and evaluates the model's performance using MAPE.

4. **Visualization**:
   - Visualizes the predicted versus actual values for training and validation data.

### Kaggle Submission Preparation
#### _prep_kaggle_upload_neural_network.ipynb

1. **Prepare Data for Kaggle Upload**:
   - Loads the predictions file (`df_predictions_neuralNetwork.csv`).
   - Merges the predictions with the sample submission file.
   - Saves the final dataframe as `df_kaggle_upload_neuralNetwork.csv` for submission.

### Variables Used in the Neural Network Model
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