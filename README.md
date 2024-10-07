Project Overview
This project aims to predict the prices of 22 different commodities using historical data sourced from gov.in. The dataset has been augmented with additional features to improve predictions. Two models, Random Forest and ARIMA, are used to train and forecast future prices based on this dataset.

Commodities Included
The dataset includes price data for the following 22 commodities:

Wheat
Rice
Maize
Barley
Soybean
Pulses
Sugarcane
Cotton
Tea
Coffee
Rubber
Jute
Groundnut
Sunflower Oil
Mustard
Onion
Potato
Tomato
Garlic
Pepper
Coconut
Milk
Files in this Repository
1. Commodities Prices Dataset
The dataset contains historical price data for the above-listed 22 commodities, gathered from government sources.
Features:
Date: The time the price data was recorded.
Commodity Type: The specific commodity (e.g., Wheat, Rice, etc.).
Region: The geographical area where prices were collected.
Price: The price per unit of the commodity.
Augmented Features: Additional derived variables such as moving averages, price trends, seasonal indices, and lag variables for more accurate predictions.
2. Model Files
Random Forest Model: This machine learning model is used to predict prices based on the feature-rich data, focusing on both short-term and medium-term predictions.
Training: The model was trained on the historical price data of the 22 commodities, incorporating augmented features like price trends and seasonal effects.
Evaluation: Model performance was evaluated using test data, with metrics like Root Mean Squared Error (RMSE) used to gauge accuracy.
ARIMA Model: A time series forecasting model suitable for predicting trends over time.
Training: ARIMA was trained on individual commodity time series data to capture long-term price movements and seasonal trends.
Evaluation: ARIMA’s accuracy was assessed using AIC/BIC criteria and test data.
Data Preprocessing
Data Cleaning: Missing data points were handled through interpolation, and any outliers were carefully analyzed.
Feature Engineering: Custom features like moving averages, lagged prices, seasonal adjustments, and trend indicators were generated to provide more meaningful inputs for the models.
Train-Test Split: Data was split into training and testing sets to evaluate the models' performance accurately.
Model Usage
Load the Dataset: Ensure the commodity price dataset is loaded and processed as per the preprocessing steps.
Model Training:
Train the Random Forest model to predict short-term price changes using all features.
Train the ARIMA model for each commodity to capture long-term trends.
Prediction: Once trained, the models can be used to predict future prices for any of the 22 commodities.
Evaluation: The models' performance is evaluated on unseen test data to assess their generalization ability.
Dependencies
Python (3.x or higher)
Pandas (For data manipulation)
Scikit-learn (For Random Forest)
Statsmodels (For ARIMA)
Matplotlib / Seaborn (For visualizing price trends and predictions)
Results
The Random Forest model demonstrates strong predictive accuracy for short-term commodity prices, handling nonlinear relationships and multiple features.
The ARIMA model provides robust long-term trend forecasts, especially for commodities with significant seasonality.
