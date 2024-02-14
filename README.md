# Classifying Credit Risk utilizing Logistic Regression

## Project Purpose
The main goal of this project is to build a logistic regression model to assess the creditworthiness of borrowers using a dataset containing historical lending information. The analysis involves splitting the data into training and testing sets, creating a logistic regression model with the original data, and providing a comprehensive analysis of the model's performance.

## Getting Started
1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. The notebook script (credit_risk_classification.ipynb) is located in the forefront of this repo
3. The raw dataset (lending_data.csv) is located in the Resources directory

### Methods Used
* Logistic Regression
* Train-Test Split
* Confusion Matrix
* Classification Report

### Technologies
* Python
* Pandas, scikit-learn

# Project Overview

## Summary
The project begins by reading the lending_data.csv from the Resources folder into a Pandas DataFrame. The dataset is then divided into labels (y) and features (X), with the "loan_status" column indicating 0 for a healthy loan and 1 for a high-risk loan. Subsequently, the data is split into training and testing sets using the train_test_split function. The logistic regression model is then fitted with the training data (X_train and y_train), and predictions are generated for the testing data labels (X_test). The model's performance is evaluated through the generation of a confusion matrix and a classification report. The analysis includes an examination of how well the model predicts both healthy (0) and high-risk (1) loans. 

## Results
The model performs exceedingly well both in the initial prediction as well as the resampled predictions. The balanced accuracy of the resampled data yields a 99% which is better than our initial sampling of 96% accurate, yet both are still significant. In particular, we see a consistent precision score of 1.0 for both datasets and corresponding 0.99 in recall for predicting whether a loan is safe. One consistent concern of the model comes in the accuracy of correctly classifying the risky loans, in other words, the lower precision of risky loans. Both the resampled and original have a high recall for predicting risky loans (0.99); however, the precision drops to 0.84. This puts the model at an increased risk of predicting falsely the risky loans to be safe ones. Overall, I would recommend this model to my employer, but it would be important to focus optimization efforts in increasing precision of predicting risky loans correctly. 
