# credit-risk-classification
I used various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

# Overview of the Analysis

Factors considered in the analysis included data on:

* the size of the loan
* its interest rate
* the borrower's income
* the debt to income ratio
* the number of accounts the borrower held
* derogatory marks against the borrower
* the total debt

![image](https://github.com/zquiroga/credit-risk-classification/assets/118328051/3f09f046-7bef-40ac-83e8-9e9580b58e3a)

 first, I Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns that had 75,036 low-risk loan data points and 2,500 high-risk data points. The dataset (77,536 data points) was Split the data into training and testing datasets by using train_test_split. The training set was used to build an initial logistic regression model (Logistic Regression Model 1) using the LogisticRegression module from scikit-learn. Logistic Regression Model 1 was then applied to the testing dataset. The purpose of the model was to determine whether a loan to the borrower in the testing set would be low- or high-risk. Also I evaluate e model’s performance by doing the following: Generate a confusion matrix with 0.9442676901753825 and Print the classification report :
 
![image](https://github.com/zquiroga/credit-risk-classification/assets/118328051/278fceb4-4339-4ed9-bdc5-43549bb8a5ee)

# Results

Machine Learning Model 

Model Accuracy: 94%.
Model Precision: for healthy loans the precision is 100%, for high-risk loans the precision is 87%.
Model Recall: for healthy loans the recall score is 100%, for high-risk loans the recall score is 89%.

# Summary

When predicting healthy loans, the logistic regression model applied to the original dataset yields superior results, as evidenced by a classification report showing a precision and recall both at 100%. However, for forecasting high-risk loans, I recommend Predict a Logistic Regression Model with Resampled Training Data with RandomOverSampler module probaly we can get a better prediction high-risk loans.

