# Loan-Repayment-Assessment-in-Banking
Task is to build and train a model that identifies a customer will repay or default from the loan dataset

# Data Preprocessing
emp_length column is converted into numerical.

emp_title column missing values are imputed by creating a new category 'Not Specified'.

Missing values were handled by imputation or filling with a placeholder case being median and modes

Skewness of the features checked and Outliers were treated by clipping based on the interquartile range (IQR) method.

# Feature Engineering
New features created :

region : Grouped the address states by region they belong.

credit history : To record days since the borrower's earliest reported credit line was opened and present.

fico_score_average : The average of high FICO and low FICO range.

# Class Imbalance Management

Using SMOTE(Synthetic Minority Over-sampling Technique)

# Models
1 LogisticRegression classifier

2 Gaussian Naive Bayes classifier

3 Linear SVM classifier

4 BaggingClassifier

5 AdaBoostClassifier

6 Random Forest classifier

7 XGBoost classifier

# Performed stratified cross-validation , GridSearchCV and hyperparameter tuning

# Feature Importance Analysis

Analysis by feature importance produced by Random Forest classifier and XGBoost classifier

# Outcome

Based on the metrics, the XGBoost classifier outperformed the other models in terms of accuracy, precision, recall, and F1-score. Achieving F1 score of 0.87.
Choose XGBoost as the primary model for prediction.
further hyperparameter tuning can be done for XGBoost to potentially improve performance.


