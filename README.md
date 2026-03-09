# Loan Default Prediction

Binary classification model to predict whether a borrower will default on a loan.

## Dataset
LendingClub Loans (2007–2018) from Kaggle — ~2.2M accepted loan records, 151 features.

## Approach
1. Engineer binary target from `loan_status` (Fully Paid = 0, Charged Off = 1)
2. Drop data leakage columns (post-disbursement payment info)
3. Impute missing values, encode categoricals
4. Train Logistic Regression → Random Forest → XGBoost
5. Evaluate with AUC-ROC and F1; explain predictions with SHAP

## Stack
Python · Pandas · Scikit-learn · XGBoost · SHAP

## Status
🔄 In progress — EDA and preprocessing phase
