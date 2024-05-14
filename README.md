<h1 align="center">DU - University of Denver<br/>
Data Analysis & Visualization Bootcamp<br/></h1>

--------------------------------

<h2 align="center">Credit Risk Classification<br/>
Module 20 Challenge
<br/>
By Laura Vara</h2><br/>

## Overview of the Analysis
The purpose of this analysis was to build a machine learning model to predict the likelihood of loan default based on financial information. The dataset contains various financial attributes of borrowers, such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, and derogatory marks. The target variable, "loan_status," indicates whether a loan is healthy (0) or high-risk (1).

Basic information about the variables:

* **loan_status (Target Variable):**
  * 0: Healthy loan
  * 1: High-risk loan
  * Value counts:
    * Healthy loan (0): 56,277 instances
    * High-risk loan (1): 1,875 instances

Stages of the machine learning process:

1. Data preprocessing: The dataset was loaded, and features and target variables were separated. The data was split into training and testing sets.
2. Model training: Logistic Regression model was instantiated and trained using the training data.
3. Model evaluation: The model was evaluated using confusion matrices, classification reports, and accuracy scores.

Methods used:
The Logistic Regression Model was used to predict the likelihood of loan default based on the given financial attributes.

## Results
* **Logistic Regression:**
  * **Testing Set:**
    * Accuracy: 99%
    * Precision (Label 0 - Healthy Loan): 100%
    * Recall (Label 0 - Healthy Loan): 100%
    * Precision (Label 1 - High-risk Loan): 87%
    * Recall (Label 1 - High-risk Loan): 95%

  * **Training Set:**
    * Accuracy: 99%
    * Precision (Label 0 - Healthy Loan): 100%
    * Recall (Label 0 - Healthy Loan): 99%
    * Precision (Label 1 - High-risk Loan): 85%
    * Recall (Label 1 - High-risk Loan): 94%


## Summary
The logistic regression model performed exceptionally well in predicting both healthy loans and high-risk loans. It achieved high accuracy, precision, and recall scores for both classes.

* **Performance Comparison:**
  * The logistic regression model's accuracy, precision, and recall scores were consistently high for both healthy loans (label 0) and high-risk loans (label 1).
  * The model predicts healthy loans with almost perfect precision and recall, indicating that it correctly identifies nearly all healthy loans.
  * Although the precision and recall scores for high-risk loans are slightly lower, they are still quite high, indicating effective identification of high-risk loans.

* **Impact on Business Goals:**
  * The performance of the model does not seem to depend significantly on the problem we are trying to solve. However, given the nature of loan predictions, it might be more important to correctly predict high-risk loans (label 1) to prevent financial losses for the lender. In this aspect, the model performs well, with high precision and recall scores for high-risk loans.

* **Recommendation:**
  * Based on the results, the logistic regression model seems to be a great best choice for predicting loan default risk. It achieves high accuracy and effectively identifies both healthy and high-risk loans. However, trialing other models might result in a higher performance for the precision and recall on the high-risk loans.


---------------------------------
INDEX
---------------------------------
1. Overview of the Analysis, Results, and Summary (Above)
2. Content of the repository
3. Instructions for the Project
4. References

---------------------------------
Content of the repository
---------------------------------
- Credit_Risk Directory:
  - credit_risk_classification.ipynb
  - lending_data.csv

----------------------------------
Instructions
----------------------------------

The instructions for this Challenge are divided into the following subsections:
* Split the Data into Training and Testing Sets
* Create a Logistic Regression Model with the Original Data
* Write a Credit Risk Analysis Report

### Split the Data into Training and Testing Sets
Open the starter code notebook and use it to complete the following steps:
1. Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
2. Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
**NOTE**
A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.
3. Split the data into training and testing datasets by using train_test_split.

### Create a Logistic Regression Model with the Original Data
Use your knowledge of logistic regression to complete the following steps:
1. Fit a logistic regression model by using the training data (X_train and y_train).
2. Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
3. Evaluate the model’s performance by doing the following:
    * Generate a confusion matrix.
    * Print the classification report.
4. Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

### Write a Credit Risk Analysis Report (Refer to the top of this ReadMe)
- Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. You should write this report as the README.md file included in your GitHub repository.
- Structure your report by using the report template that Starter_Code.zip includes, ensuring that it contains the following:
1. **An overview of the analysis:** Explain the purpose of this analysis.
2. **The results:** Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.
3. **A summary:** Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.

------------------------------------
References
------------------------------------
Everything included in this project was covered in class. Regardless, these two resources were used to complete the challenge.

https://scikit-learn.org/stable/index.html 





