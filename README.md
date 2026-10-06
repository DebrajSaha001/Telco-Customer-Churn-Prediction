# Telco Customer Churn Prediction

Predicts which telecom customers are likely to leave, using Python.

## Problem
Customer churn costs telecom companies revenue. This project identifies the customers most at risk so retention efforts can be targeted.

## Data
- Telco Customer Churn dataset: [7,043] customers, [21] columns
- Target: whether the customer churned (Yes/No)

## Method
1. Data cleaning: [
   1 .Converted TotalCharges from text to numeric
   2. Filled 11 blank records (tenure = 0) with 0
   3. Dropped the non-predictive customerID column
   4. Encoded the Churn target as binary 0 / 1]
2. Exploratory analysis: churn compared across [Contract Type, Tenure, Monthly Charges, Internet Type]
3. Encoding of categorical features
4. Classification model:
     1. Linear Regression
     2. Random Forest
     3. XGBoost

## Results
- Model: Logistic Regression, ROC-AUC: [0.835], F1-Score: [0.611] 
- Key finding: [Customers with Electronic Check Payment, Fiber Optic Internet, Short Tenure, High Monthly Charges increases the Churned Probability with respect to those customers with Two Years Contract have less Churned Probability]

## Tools
Python, Pandas, Matplotlib, [scikit-learn]

## How to run
Download the notebook and the CSV into the same folder, then open the notebook in Jupyter or Google Colab and run all cells.
