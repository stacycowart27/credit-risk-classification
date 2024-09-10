# Module 20 Report 

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* **Explain the purpose of the analysis.** The goal of this analysis is to determine if the Logistic Regression machine learning model can more accurately predict healthy loans versus high risk loans using the original dataset or a dataset that is resampled to increase the size of the minority class. 
**Explain what financial information the data was on, and what you needed to predict.** The dataset used to perform the analysis consists of inofrmation on 77,536 loans. The data inclused columns for loan_size, interest_rate, borrower_income, debt_to_income_ratio, number_of_accounts, derogatory_marks, total_debt, and loan_status. The category we are attempting to predict with our analysis is "loan_status". The data provided in the remaining columns will be used as features to train the data and inform the predictions.
***Describe the stages of the machine learning process you went through as part of this analysis.** The stages of the machine learning process are very scripted. If followed in order, they provide you with an accurate assessment of the model's ability to make predictions. The stages of the machine learning process are as follows:
    -Prepare the data- Import the file, establish the DataFrame, evaluate the columns and features
    -Separate the data into features and labels. The labels are what you are attempting to predict, is the status of the loan healthy(0) or high risk (1). The features are all of the reamining data you will use to train and test the model.
    -Use the train_test_split function to separate the features and labels data into training and testing datasets.
    -Import the machine learning model from the library - In this instance we will be importing LogisticRegression from SKLearn.
    -Instantiate the model.
    -Fit the model using the training data
    -Use the model to make predictions using the features test data
    -Evaluate the predictions - Evaluations are done by calculating and comparing metrics like accuracy score, a confusion matrix, and a classification report.
    -
**Briefly touch on any methods you used** The primary model used in this analysis is: LogisticRegression Model from SKLearn. Supporting functions used in this model are: train_test_split from SKLearn. Models are evaluated using the following functions: confusion_matrix from SKLearn and classification_report from SKLearn.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model - Logistic Regression
  **Accuracy Score** 99%
  **Precision Scores**
  Class 0 (Healthy Loans): 100%
  Class 1 (High Risk Loans): 85%
  **Recall Scores**
  Class 0 (Healthy Loans): 99%
  Class 1 (High Risk Loans): 91%


## Summary

The model does a great job in using the original data to predict the values of the healthy loans. Precision was 100% and recall was 99%. The model is pretty good at predicting the values of high risk loans, but not as good as the healthy loans. Precision was 85% and recall was 91%. Given this information, it appears the Logistic Regression model does a great job at predicting both healthy and high risk loans, given the features that are used to train the data. 

