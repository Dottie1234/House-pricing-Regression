# House-pricing-Regression

## Table of Contents
Project Overview
Dataset
Data Preprocessing
Feature Engineering
Feature Selection
Modeling
Hyperparameter Tuning
Results and Evaluation
Usage
Acknowledgments
Contributors

## Project Overview
This project is a beginner friendly project that predicts the prices of houses based on the features available. The aim of this project is to aid beginners in exploring the different steps involved in building machine learning projects. Have fun!

## Dataset
The dataset is the train.csv and test.csv file available in the repository. or you can get the dataset from kaggle
(http://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)

## Data Preprocessing
The data Preprocessing steps include: 

* Handling missing values: The features with missing values more than 50 percent of the values in each feature is dropped and the ones with null values less than 50% is filled with pandas `.fillna()` method.
* The numerical features with interesting outliers were scaled with scikit-learn `StandardScaler()`.
* Dealing with high correlation in numerical features: Numerical features with high correlation of 0.9 was also dropped.
* Handling low cardinality in categorical features: Categorical features with low cardinality of 5 was dropped.


## Feature Engineering
Feature engineering process:
* Categorical feature encoding: using (label encoding, one-hot encoding).
* Feature scaling: Scaling of Numerical features.

## Feature Selection
`sklearn.feature_selection.SelectPercentile()` is used with score_function of f_regression and percentile of 20.

