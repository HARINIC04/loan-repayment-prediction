Loan Repayment Prediction
Project Overview

This project aims to predict the likelihood of a borrower repaying a loan using machine learning techniques. By analyzing various borrower attributes, the model assists financial institutions in assessing credit risk and making informed lending decisions.

Objective

The primary objective is to develop a predictive model that classifies loan applicants into two categories:

Fully Paid: The borrower repaid the loan on time.

Charged Off: The borrower defaulted on the loan.

Dataset

The dataset utilized in this project is sourced from Kaggle's LendingClub dataset
, which contains information about loan applicants, including:

Credit Policy: Whether the borrower meets the credit underwriting criteria.

Annual Income: The borrower's annual income.

FICO Score: A measure of the borrower's creditworthiness.

Loan Amount: The total loan amount requested.

Interest Rate: The interest rate charged on the loan.

Debt-to-Income Ratio: The borrower's debt relative to their income.

Delinquencies: The number of past due payments.

Credit History Length: The length of the borrower's credit history.

Purpose: The purpose of the loan (e.g., debt consolidation, credit card refinancing).

Methodology
1. Data Preprocessing

Handling Missing Values: Imputed missing values using appropriate strategies.

Feature Engineering: Created new features to enhance model performance.

Encoding Categorical Variables: Applied one-hot encoding to categorical variables.

Feature Scaling: Standardized numerical features to bring them to a common scale.

2. Model Development

Implemented and evaluated several machine learning models:

Logistic Regression

Decision Tree Classifier

Random Forest Classifier

Gradient Boosting Classifier

AdaBoost Classifier

Each model's performance was assessed using accuracy, precision, recall, and F1-score metrics.

3. Model Evaluation

The models were evaluated using:

Cross-Validation: To ensure the model's performance is consistent across different subsets of the data.

Hyperparameter Tuning: Employed grid search to find the optimal hyperparameters for each model.

Results

The Gradient Boosting Classifier achieved the highest performance metrics, with an accuracy of 85%, precision of 83%, recall of 87%, and an F1-score of 85%.

Deployment

For deployment, the trained model was saved using joblib and integrated into a Flask web application. The application allows users to input borrower details and receive a prediction on loan repayment.

Technologies Used

Python Libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

Web Framework: Flask

Model Serialization: Joblib
