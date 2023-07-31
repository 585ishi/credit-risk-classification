# Module 12 Report Template

## Overview of the Analysis

Purpose of the analysis - The goal of this analysis was to determine if the Logistic Regression machine learning model can more accurately predict healthy loans versus high-risk loans using the original dataset or a dataset that is resampled to increase the size of the minority class.


The Dataset - The dataset used to perform the analysis consists of information on 77,536 loans. The data includes columns for  loan_size, interest_rate, borrower_income, debt_to_income ratio, number_of_accounts, derotatory_marks, total_debt, and loan_status. The category that we are attempting to predict with our analysis is loan_status. The data provided in the remaining columns will be used as features to train the data and inform the predictions.


Stages of the Machine Learning Process - The stages of the machine learning process are very scripted. If followed in order, they provide you with an accurate assessment of the model's ability to make predictions. The stages of the machine learning process are as follows:


 1. Prepare the data - Import the file, establish the DataFrame, evaluate the columns and features.


 2. Separate the data into features and labels - The labels are what you are attempting to predict, is the status of the loan     healthy (0) or high-risk (1). The features are all of the remaining data you will use to train and test the model.


 3. Use the train_test_split function to separate the features and labels data into training and testing datasets.


 4. Import the machine learning model from the library - In this instance, we will be importing LogisticRegression from SKLearn.


 5. Instantiate the model.


 6. Fit the model using the training data.


 7. Use the model to make predictions using the features test data.


 8. Evaluate the predictions - Evaluations are done by calculating and comparing metrics like accuracy score, a confusion matrix, and a classification report.




Machine Learning Methods Utilized -
 1. The primary model used in this analysis is:

 2. LogisticRegression model from SKLearn

 3. Supporting functions used in this analysis are:

 4. train_test_split from SKLearn

 5. Models are evaluated using the following functions:

 6. confustion_matrix from SKLearn

 7. classification_report from SKLearn

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1: Logistic Regression:

 *Accuracy score: 0.99
  Precision: Class 0: 1.00 Class 1: 0.85
  Recall: Class 0: 0.99 Class 1: 0.91



* Machine Learning Model 2: Logistic Regression Model with Resampled Training Data
  * Accuracy score: 0.99
    Precision: Class 0: 1.00 Class 1: 0.84
    Recall: Class 0: 0.99 Class 1: 0.99

## Summary

Overall, both the models performed well, especially regarding predicting the outcomes for Class 0 (healthy loans). For the 0 class, both the precision and the recall were extremely close to perfect.
For the 1 class (high-risk loans), both the models precision is 0.8 (rounded to one decimal) the recall is 0.9 (rounded to one decimal). This indicates that the models more often gives false positives than false negatives.
Given this information, it appears that both the models do a great job at predicting both healthy and high-risk loans, given the features that are used to train the data.


