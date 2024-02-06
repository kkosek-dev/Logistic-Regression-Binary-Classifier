# credit-risk-classification
This project is a part of the Module 20 challenge in the Vanderbilt University Data Analytics BootCamp and is written entirely by the author of the repository. This README template is from the Data Science Working Group.

#### -- Project Status: [Completed]

## Project Overview
The main goal of this project is to build a logistic regression model to assess the creditworthiness of borrowers using a dataset containing historical lending information. The analysis involves splitting the data into training and testing sets, creating a logistic regression model with the original data, and providing a comprehensive analysis of the model's performance.

### Methods Used
* Logistic Regression
* Train-Test Split
* Confusion Matrix
* Classification Report

### Technologies
* Python
* Pandas, scikit-learn

## Project Description
The project begins by reading the lending_data.csv from the Resources folder into a Pandas DataFrame. The dataset is then divided into labels (y) and features (X), with the "loan_status" column indicating 0 for a healthy loan and 1 for a high-risk loan. Subsequently, the data is split into training and testing sets using the train_test_split function. The logistic regression model is then fitted with the training data (X_train and y_train), and predictions are generated for the testing data labels (X_test). The model's performance is evaluated through the generation of a confusion matrix and a classification report. The analysis includes an examination of how well the model predicts both healthy (0) and high-risk (1) loans.

## Getting Started

1. Clone this repository (for help see this tutorial).
2. The Jupyter Notebook script (credit_risk_classification.ipynb) and the dataset (lending_data.csv) are located in the "Credit_Risk" folder.
3. Raw data is stored in the Resources directory.   
