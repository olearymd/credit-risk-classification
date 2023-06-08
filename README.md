# credit-risk-classification

In this repo, we have code to test the ability of two logistic regression models to accurately predict healthy vs. high-risk loans based on the following features for 75,036 healthy and 2,500 high risk loans

- Loan Size
- Interest Rate
- Borrower Income
- Debt to Income Ratio
- Number of Accounts
- Derogatory Marks
- Total Debt

The first model utilized the original data set and returned the following:

              precision    recall  f1-score   support

     Healthy       1.00      1.00      1.00     18759
   High-Risk       0.87      0.89      0.88       625

    accuracy                           0.99     19384
   macro avg       0.94      0.94      0.94     19384
weighted avg       0.99      0.99      0.99     19384

The second model utilized a RandomOverSampler module for imbalanced datasets, and returned the following:

              precision    recall  f1-score   support

     Healthy       0.99      0.99      0.99     56277
   High-Risk       0.99      0.99      0.99     56277

    accuracy                           0.99    112554
   macro avg       0.99      0.99      0.99    112554
weighted avg       0.99      0.99      0.99    112554

# Summary

Given the imalanced nature of our data set and the outsized importance of predicting high-risk loans, the second model utilizing the RandomOverSampler module is recommended.   
