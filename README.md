# Predictive Modeling for Consumer Purchase and Spending

## Overview
This project focuses on building predictive models to analyze consumer behavior in response to a test mailing of a catalog. The dataset, provided in the customers.xlsx file, contains information about whether consumers made a purchase and, in case of a purchase, the amount spent. The primary objective is to predict consumer spending based on various customer attributes while exploring multiple numeric prediction techniques.

## Dataset (customers.xlsx)
The dataset consists of consumer information, including whether a purchase was made (Purchase: 0/1) and the spending amount (Spending: numeric value).

## Project Structure
### For task (a) use full dataset, for task (b) use restricted dataset (Purchase = 1)

1. Data Preprocessing: The data is loaded from an Excel file and split into a feature matrix (X) and target variable (y). Min-Max scaling (Normalization) is applied to the feature matrix to ensure all features are on a similar scale.

2. Model Selection: Various predictive modeling techniques are employed, including Linear Regression, k-NN (K-Nearest Neighbors), Decision Tree, SVM Regression (Support Vector Machine), Random Forest, Neural Network, and XGBoost.

3. Hyperparameter Tuning: Hyperparameter tuning is performed for each model using RandomizedSearchCV to find the best combination of hyperparameters.

4. Cross-Validation: Nested cross-validation with KFold is utilized, with an outer loop for model evaluation and an inner loop for hyperparameter tuning.

5. Performance Metric: A custom scoring function for RMSE (Root Mean Squared Error) is defined and used to evaluate models. Lower RMSE values indicate better predictive performance.

## Result
|Model Name | (a) Average RMSE | (a) Model Rank | (b) Average RMSE | (b) Model Rank |
|-----------|------------------|----------------|------------------|----------------|
|Linear Regression|  127.73 | 1 | 165.25 | 2 |
|K-NN Regression | 169.76 | 7 | 208.50 | 7 |
|Decision Tree Regression | 133.37 | 4 | 189.88 | 5 |
|SVM Regression | 167.60 | 6 | 206.79 | 6 |
|Random Forest | 128.07 | 2 | 160.84 | 1 |
|XGBoost | 132.00 | 3 | 175.15 | 3 |

## How to Run:
- Clone the repository.
- Install the required dependencies using pip install packages.
- Execute the main script to run the predictive modeling analysis.

Feel free to explore and contribute to the project for further enhancements and insights.
