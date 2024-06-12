# Real-Estate-Houses-in-Argentina-Predicting-Apartment-Prices
This project aims to create a model that predicts the price of apartments in Buenos Aires, Argentina, focusing on those priced below $400,000. The project involves building multiple models with increasing complexity to improve prediction accuracy.

## Models Implemented

## 1. Linear Regression with Single Dataset
Description: The first model employs a simple Linear Regression on a single dataset of Buenos Aires apartment prices.

## Performance:
Baseline MAE: 59231.71
Training MAE: 36489.06

## 2. Enhanced Linear Regression with Additional Features
Description: Building on the initial model, this version includes a more complex data wrangling function to clean additional data and incorporate more features for predicting apartment prices.

## Performance:
Baseline MAE: 59231.71
Training MAE: 59216.41
Model Coefficients: [7156.35]
Intercept: 23488.49

## 3. Ridge Regression with Combined Datasets
Description: This model uses Ridge Regression and combines multiple datasets using the glob library to handle more data and improve prediction accuracy.

## Performance:
Baseline MAE: 66154.97
Training MAE: 62799.16
Model Coefficients: [-26760.5, 32548.75, 2654.72, 33414.91, 18621.18]
Intercept: 115282.94

## 4. Ridge Regression with Combined Datasets and Imputation
Description: The final model improves upon the previous Ridge Regression by adding a SimpleImputer to handle missing values.

## Performance:
Baseline MAE: 66154.97
Training MAE: 66154.97
Model Coefficients: [1893.61, -1818.4, 956.51, 16316.06, 9685.38]
Intercept: 15065.22

## Data Source
The dataset contains real estate data for Buenos Aires apartments, focusing on those priced below $400,000. The data includes various features such as location, size, and amenities.

## Methodology
Data Collection: Gathered datasets using the glob library to combine multiple CSV files.
Data Preprocessing: Cleaned and imputed missing values, applied one-hot encoding for categorical variables.

## Model Building:
Implemented Linear Regression for initial modeling.
Enhanced the model by including more features and cleaning more data.
Used Ridge Regression to handle multicollinearity and combined datasets for better predictions.
Model Evaluation: Evaluated models using Mean Absolute Error (MAE) to measure prediction accuracy.
Visualization: Used matplotlib and plotly to visualize data and model performance.

## Results
The initial Linear Regression model provided a baseline MAE.
Enhancing the data wrangling and including more features slightly improved the MAE.
Combining datasets and applying Ridge Regression further improved the model's performance.
The final model, with added imputation, provided the most robust predictions.

## Conclusion
This project demonstrates the process of building and improving predictive models for real estate prices in Buenos Aires. By iteratively refining data preprocessing and employing more sophisticated models, we achieved better prediction accuracy.
