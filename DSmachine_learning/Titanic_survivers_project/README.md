# Titanic Survival Prediction

## Project Overview

This project predicts whether a passenger survived the Titanic disaster using machine learning algorithms. It focuses on feature engineering and improving model performance.

## Dataset
* Source: Titanic dataset on Kaggle

The dataset contains passenger information such as:
- PassengerID
- Survived (0 = Did not survive, 1 = survived)
- Ticket Class (Pclass): 1 = 1st class, 2 = 2nd class, 3 = 3rd class
- Name
- Sex
- Age
- Number of siblings/spouses (SibSp)
- Number of parents/children (Parch)
- Ticket
- Fare

## Problem Statement 

Predict passenger survival (0 = Did not survive, 1 = Survived).

## Tech Stack

* Python
* Pandas
* Scikit-learn (LogisticRegression,StandardScaler,RandomForestClassifier, train_test_split, accuracy_score, classification_report, confusion_matrix)
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

- But they both performed slightly different from their precision, recall and f1-score results. The Logistic Regression model performed slitly better than the Random Forest Classifier
  - The results were highly influenced by the sex feature. The sex highly determined the survival of the passengers on the titanic.

## **Insights**
* People who did not survive are more than those that survived the disaster.
* More female passengers likely survived than male passengers
* People in higher class were more priotized than people in other classes

## How to run

1. Clone the repository 
2. Navigate to the folder ensure that `Titanic-Dataset.csv` is in the same folder as the notebook `Titanic_Survivers.ipynb`
3. Open `Titanic_Survivers.ipynb` in your Jupyter Nootebook or JupyterLab.
4. Run all cells to preprocess the data, train the model and view predictions and visualisations