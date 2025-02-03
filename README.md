# Sales Forecasting for a Bakery Branch

## Repository Link

https://github.com/manuelboehm/MA-bakery-sales-prediction

**(NOTE: The branch *production* contains the current code. The branch *main* is not up to date.)**

## Description

This project focuses on sales forecasting for a bakery branch, utilizing historical sales data spanning from July 1, 2013, to July 30, 2018, to inform inventory and staffing decisions. We aim to predict future sales for six specific product categories: Bread, Rolls, Croissants, Confectionery, Cakes, and Seasonal Bread. Our methodology integrates statistical and machine learning techniques, beginning with a baseline linear regression model to identify fundamental trends, and progressing to a sophisticated neural network designed to discern more nuanced patterns and enhance forecast precision. The initiative encompasses data preparation, crafting bar charts with confidence intervals for visualization, and fine-tuning models to assess their performance on test data from August 1, 2018, to July 30, 2019, using the Mean Absolute Percentage Error (MAPE) metric for each product category.

### Task Type

Regression

### Results Summary

-   **Best Model:** neuronales_modell_v2 ([see NeuronalesModell_v2.ipynb](3_Model/NeuronalesModell_v2.ipynb))
-   **Evaluation Metric:** MAPE (Validation Data)
-   **Result by Category** (Identifier):
    -   **Bread** (1): 29.75 %
    -   **Rolls** (2): 22.96 %
    -   **Croissant** (3): 22.04 %
    -   **Confectionery** (4): 28.32 %
    -   **Cake** (5): 18.24 %
    -   **Seasonal Bread** (6): 158.56 %

## Documentation

1.  [**Data Import and Preparation**](0_DataPreparation/)
3.  [**Dataset Characteristics (Barcharts)**](1_DatasetCharacteristics/)
4.  [**Baseline Model**](2_BaselineModel/)
5.  [**Model Definition and Evaluation**](3_Model/)
6.  [**Presentation**](4_Presentation/README.md)

## Cover Image

![](CoverImage/Image_Presentation_Group_1.PNG)
