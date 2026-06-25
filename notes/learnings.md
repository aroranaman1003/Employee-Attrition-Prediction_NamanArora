# Learnings

## Week 2

### Employee Attrition Prediction

This project focuses on predicting whether an employee is likely to leave a company using Machine Learning classification techniques.

Concepts to learn:

* Classification
* Logistic Regression
* Random Forest Classifier
* Gradient Boosting Classifier
* Precision
* Recall
* F1 Score
* ROC-AUC
* Confusion Matrix
* Feature Importance

## Task 1 - Data Loading & Exploration

### Concepts Learned

- How to load datasets using Pandas.
- Difference between rows and columns in a dataset.
- How to identify the target variable.
- How to calculate attrition rate.
- Difference between numerical and categorical features.
- Understanding class imbalance in classification problems.

### Key Findings

- Dataset contains 1470 employee records.
- Dataset contains 35 columns.
- Target column: Attrition.
- The dataset is imbalanced because employees who stayed significantly outnumber employees who left.


## Task 2 - Data Cleaning & Preprocessing

### Concepts Learned

* Checked the dataset for missing values using `isnull().sum()`.
* Understood that missing values can be handled by dropping rows/columns or by imputing values depending on the dataset.
* Identified and removed constant columns and identifier columns that do not contribute to prediction.
* Converted the target variable (`Attrition`) from categorical values (`Yes`/`No`) to numerical values (`1`/`0`).
* Applied One-Hot Encoding to convert categorical features into numerical features.
* Standardized continuous numerical features using `StandardScaler`.

### Key Takeaways

* Machine Learning models require numerical data.
* Constant and identifier columns add no predictive value.
* One-Hot Encoding prevents introducing artificial ordering into categorical variables.
* Feature scaling helps algorithms treat numerical features fairly by bringing them to a common scale.
