# Module 12: Credit Risk Analysis Report

Purpose of the analysis: The analysis aims to build and evaluate machine learning models for predicting loan default status based on financial information, assisting a lending institution in risk assessment.

Financial Information and Prediction: The data contains financial information for loans, with the target variable "loan_status" indicating loan default (1) or non-default (0).

Variables: The target variable "loan_status" has two classes (0 and 1). Other variables represent financial features used for prediction.

# Process Summary

Data Loading: Load the loan data from a CSV file into a DataFrame.

Data Preprocessing: Split the data into features (X) and the target variable (y) representing loan status (default or non-default).

Train-Test Split: Split the data into training and testing sets to train and evaluate the machine learning models.

Model Training and Evaluation (Model 1 - Logistic Regression): Train a logistic regression model on the original training data and evaluate its performance using accuracy, precision, recall, and a confusion matrix.

Resampling, Model Training and Evaluation (Model 2): Address class imbalance by applying random oversampling to the training data, creating synthetic samples of the minority class. Train another logistic regression model on the resampled data. Evaluate the second model's performance on the testing set using the same metrics as Model 1.

# Methods Used

Model 1: Logistic Regression: Used for binary classification, predicting loan default or non-default.

Model 2: Random Oversampling: Applied to address class imbalance by creating synthetic samples of the minority class.

# Summary Results

Model 1:

Balanced Accuracy Score: The balanced accuracy score for Model 1 is approximately 0.95.

Precision and Recall Scores:

Precision for class 0 (non-default): 1.00
Precision for class 1 (default): 0.85
Recall for class 0 (non-default): 0.99
Recall for class 1 (default): 0.91

Model 2:

Balanced Accuracy Score: The balanced accuracy score for Model 2 is approximately 0.99.

Precision and Recall Scores:

Precision for class 0 (non-default): 1.00
Precision for class 1 (default): 0.84
Recall for class 0 (non-default): 0.99
Recall for class 1 (default): 0.99
Summary:

Comparing the performance of the two machine learning models:

Model 1 has a balanced accuracy score of approximately 0.95, which means it correctly classifies both the default and non-default cases with high accuracy.

Model 2 has a higher balanced accuracy score of approximately 0.99, indicating even better overall performance in classifying both classes.

Recommendation:

Based on the evaluation metrics, Model 2 outperforms Model 1 in terms of balanced accuracy, precision, and recall for both classes. It shows better classification performance on the testing data and is more suitable for the given problem.

The performance of the models may depend on the specific problem we are trying to solve. In this case, since the data is related to loan status (default or non-default), correctly predicting the defaults (class 1) is crucial for risk assessment and decision-making in the lending industry. Model 2 has a significantly higher recall score for class 1, meaning it is better at identifying true positives (default cases) compared to Model 1. Therefore, if the main goal is to predict defaults accurately, Model 2 is the preferred choice.

