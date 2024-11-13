# Credit Risk Classification

## An overview of the analysis

* Explain the purpose of the analysis.

  The purpose of this analysis was to create a supervised machine learning model that would predict if a loan is healthy or high-risk.

* Explain what financial information the data was on, and what you needed to predict.

  The data contained columns of various data about the loan amount, interest rate and the borrower's income, debt and accounts, as well as a column classifying the loan as healthy or high-risk.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

  For the target values of loan_status there are two variables. The first set of variables have a value of '0' which indicates that the loan is healthy. The second set of variables have a value of '1'which means that the loan has a high risk of defaulting.

* Describe the stages of the machine learning process you went through as part of this analysis.

  To preform the machine learning process the data was:
  1. Split into labels and features, with the loan status (healthy or high-risk) being the label and the remaining seven columns as features.
  2. The data was then split into training and testing data sets.
  3. A Logistic Regression model was created using ('lbfgs') solver.
  4. Logistic Regression was chosen as we are classifying loans as healthy OR high-risk and only those two options.
  5. The model was then fit with the training data.
  6. Predictions were made with the test data.
  7. The model was evaluated by generating a confusion matrix & printing classification report.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

  The logistic regression module was used to aid predictions throughout the analysis.

## The results

* Using a bulleted list, describe the accuracy, precision, and recall scores of the machine learning model.

- Accuracy: **0.99**
- Precision
  - Healthy: **1.00**
  - High-Risk: **0.84**
- Recall
  - Healthy: **0.99**
  - High-Risk: **0.94**
 
## A summary

* The Logistic Regression Model has performed well to predict the Loan Status with an accuracy score of 0.99 as reported in the classification report.
* The precision and recall score for Loan Status '0' are both 1, which means the model was able to correctly predict 'Healty Loan' labels.
* The precision and recall score for Loan Status '1' are .87 & .89 respectievely so the model was not able to predict 'High-Risk Loan' as accurate as 'healthy loan' but it still has a good success rate.

It would be recommended to use the Logistics Regression Model for predicting credit worthiness of borrowers.








