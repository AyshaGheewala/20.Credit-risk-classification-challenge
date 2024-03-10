# 20.Credit-risk-classification-challenge
Module 20 Challenge - Loan Risk Machine Learning Model

## Overview of the Analysis
The purpose of this analysis was to create a model and evaluate its effectiveness in identifying the creditworthiness of borrowers. 

The analysis aims to assess how well the model distinguishes between "Healthy Loans" and "High-risk Loans."

The dataset used to build the model included several pieces of financial information:
- size of the loan
- interest rate
- income of the borrower
- debt to income rate
- number of accounts
- total derogatory marks
- total debt of the borrower 

I began the analysis by preprocessing the data. After defining the labels and features, I split the data into subsets for training and testing using `train_test_split`.
Then I created a Logistic Regression Model. I fit the model with the training data and used it to predict outcomes for the testing data. Finally, I assessed the model's effectiveness by generating a confusion matrix and a classification report. 

## Results
- Accuracy: 99%
    - The high level of accuracy indicates that the model is making correct predictions for the vast majority of instances.

- Precision: 
    - Healthy Loan: 100% - indicates that all instances predicted as "Healthy Loan" were correct
    - High-Risk Loan: 85% - indicates that the majority of instances predicted as "High-risk Loan" were correct

- Recall:
    - Healthy Loan: 99% - suggests that the model effectively captured almost all instances of "Healthy Loans"
    - High-Risk Loan: 91% - suggests that the model captured a significant portion of "High-risk Loans"

## Summary
Overall, this model has very high accuracy and performance, especially in identifying "Healthy Loans". 

It has slightly lower performance in identifying "High-risk Loans", as reflected in the slightly lower precision and recall score for that class. Whilst there may be some falsely identified high-risk loans, the model effectively captures a significant portion of the actual high-risk loans.

Since the consequences of misclassifying high-risk loans could be serious, further refinement to improve precision for the "High-risk Loan" class could be considered. This might involve exploring additional features to enhance the model's predictive capability. Nevertheless, considering the overall strong performance, the current model is valuable for identifying loan risk. Thus I would recommend its use by the company, as it will contribute to effective risk management in lending practices.