# **California Housing Price Prediction**

## Overview

This project builds a machine learning model to predict housing prices in California using demographic and geographical data. The focus is on feature engineering, model comparison and extracting key insights.

## Problem Statement
Predict the house price based on available features and understand what drives housing prices.

## Dataset
**Source:** Built-in dataset from `scikit-learn (fetch_california_housing)`
- Includes features such as income, population, housing characteristics and location.

Features in the dataset:
 - MedInc (Median Income)
 - HouseAge (Median House age)
 - AveRooms (Average rooms per house)
 - AveBedrms (Average bedrooms)
 - Population (Area Population)
 - AveOccup (Average occupancy)
 - Latitude/Longitude (Location)

## Tech Stack

* Python
* Pandas
* Numpy
* Scikit-learn
* Matplotlib
* Seaborn

## Feature Engineering
Created new features to capture deeper relationships with price:

- RoomsPerHousehold
- BedroomRatio 
- PeoplePerHouse

## Models used:
- Linear Regression model
- Random Forest Regressor model

## Model Performance
1. Linear Regression model
- Before feature engineering:
   - MAE: 0.53
   - R2: 0.57
- After feature engineering:
   - MAE: 0.48
   - R2: 0.65 

2. Random Forest Regressor model
- MAE: 0.33
- R2: 0.80

## Results
 - Feature engineering improved the performanc of the Linear Regression model.
 - Random Forest Regressor model performed better on the data than the Linear Regression model.
 - The Random Forest Regressor model mean_absolute_error results dropped and the ratio score increased to 80% (0.80)

## **Insights**
- Random Forest provided the best performance for the data. 
- Median income is the dominant factor in predicting house prices.
- Feature engineering provided small but meaningful improvements to the model performances.

## How to run

1. Clone the repository 
2. Open `CalforniaHousing_prediction.ipynb` in your Jupyter Nootebook or JupyterLab.
3. Run all cells to preprocess the data, train the model and view predictions and visualisations