# Heart Disease Prediction Using Machine Learning
Course project for Machine Learning for Data Science (DS2401) at Umm Al-Qura University. Team of 4.

## Overview
A supervised binary classification project predicting the presence of heart disease from clinical attributes, comparing Logistic Regression and Decision Tree models.

## Dataset
[Heart Failure Prediction Dataset (Kaggle)](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction): 918 records, 12 features.

## Methodology
1. Exploratory data analysis
2. Preprocessing: found 172 zero Cholesterol values and 1 zero RestingBP value (biologically impossible), treated them as hidden missing values and replaced them with the median; encoded categorical variables; scaled features with StandardScaler
3. 80/20 train-test split with a fixed random state
4. Models: Logistic Regression and Decision Tree
5. Evaluation: accuracy, precision, recall, F1-score, ROC-AUC, and confusion matrices

## Results
| Model | Recall | Notes |
|---|---|---|
| Logistic Regression | 88.2% | ROC-AUC 92.51% |
| Decision Tree | 82.4% | Signs of mild overfitting |

Logistic Regression outperformed the Decision Tree on the test set.

## My Contribution
Checked missing values and duplicates, handled biologically implausible zero values using median imputation, and encoded categorical variables with LabelEncoder.

## Tools
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

## Limitations
Small dataset; hyperparameter tuning and ensemble methods were not explored.
