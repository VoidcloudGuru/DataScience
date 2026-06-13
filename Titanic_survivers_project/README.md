# Titanic Survival Prediction

## Project Overview

This project predicts whether a passenger survived the Titanic disaster using machine learning algorithms. It focuses on feature engineering and improving model performance.

## Dataset
* **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset)

The dataset contains passenger information such as:
- PassengerID
- Survived (0 = Did not survive, 1 = survived)
- Ticket Class (Pclass): 1 = 1st class, 2 = 2nd class, 3 = 3rd class
- Name
- Sex
- Age
- SibSp (siblings/spouses) 
- Parch (parents/children) 
- Ticket
- Fare

## Problem Statement 

Predict passenger survival (0 = `Did not survive`, 1 = `Survived`).

## Tech Stack

* Python
* Pandas
* Scikit-learn
* Matplotlib
* Seaborn

## Feature Engineering
Created new features to improve performance:

- FamilySize (based on number of siblings/spouses and number of parents/children) 
- IsAlone (based on family size)
- Title (extracted from passenger names)

### Models used

* Logistic Regression 
* Random Forest Classifier

## Results

- Both the models acquired the same accuracy 0.81 (81%)
- Both models performed slightly different from their precision, recall and f1-score results. 
- The Logistic Regression model performed slightly better overall.
- Model predictions were strongly influenced by the Sex feature. 

## **Insights**
* More people died than survived.
* Female passengers had higher survival rates than male passengers.
* Passengers in higher class were more likely to survive than passengers in other classes.

## How to run

1. Clone the repository 
2. Navigate to the folder ensure that `Titanic-Dataset.csv` is in the same folder as the notebook `Titanic_Survivers.ipynb`
3. Open `Titanic_Survivers.ipynb` in your Jupyter Nootebook or JupyterLab.
4. Run all cells to preprocess the data, train the model and view predictions and visualisations
