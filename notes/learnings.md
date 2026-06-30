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


## Task 3 - Exploratory Data Analysis (EDA)

### Exploratory Data Analysis

* Understood that EDA is performed to identify patterns, relationships, and trends before building machine learning models.
* Learned to separate business analysis (EDA) from model preprocessing by using a separate `df_eda` dataframe.

### GroupBy and Lambda Functions

* Used `groupby()` to analyze attrition across categorical features.
* Used `lambda x: (x == "Yes").mean() * 100` to calculate attrition percentages.

### Choosing the Right Analysis

* Learned that not every numerical feature should be grouped directly.
* For continuous variables such as `MonthlyIncome`, creating ranges (bins) produces more meaningful business insights than grouping every unique value.
* For ordinal features such as `WorkLifeBalance`, no binning is required because the values already represent categories.

### Binning Numerical Features

* Used `pd.cut()` to create salary and experience ranges.
* Learned how `bins`, `labels`, and `include_lowest=True` work.

### Business Insights

* Learned that EDA should answer business questions instead of simply displaying statistics.
* Observations should describe relationships and trends without claiming causation.

### Data Analysis Best Practices

* Always check the number of unique values (`nunique()`) before deciding whether to create bins.
* Consider sample size before interpreting percentages, especially when groups contain very few observations.


# Task 4 & Task 5 - Model Building and Evaluation

## Model Building
- Learned how to split the dataset into training and testing sets using an 80/20 ratio.
- Understood the importance of `stratify=y` for maintaining class distribution.
- Learned why `class_weight="balanced"` helps handle imbalanced datasets without modifying the original data.
- Trained three classification models:
  - Logistic Regression
  - Random Forest Classifier
  - Gradient Boosting Classifier

## Model Evaluation
- Evaluated models using Precision, Recall, F1-Score, ROC-AUC, and Confusion Matrix.
- Learned why Accuracy is not sufficient for imbalanced classification problems.
- Compared multiple models using a single comparison table.
- Selected the best model based on a balance of evaluation metrics instead of relying on one metric.

## Model Interpretation
- Learned the difference between Feature Importance and Logistic Regression Coefficients.
- Understood why tree-based models use `feature_importances_` while Logistic Regression uses `coef_`.
- Ranked the Top 10 most influential features affecting employee attrition.


# Task 6 - Data Visualization

## Charts Created

- Created a bar chart to visualize attrition rates across different departments.
- Created a bar chart to compare attrition rates among different job roles.
- Created a box plot to compare the monthly income distribution of employees who stayed versus those who left.
- Visualized the confusion matrix of the best-performing model (Logistic Regression).
- Ranked and visualized the Top 10 most influential features using the absolute values of Logistic Regression coefficients.
- Created an ROC Curve comparing Logistic Regression, Random Forest, and Gradient Boosting models.

## Concepts Learned

- Difference between bar charts, box plots, and horizontal bar charts.
- Why box plots are suitable for comparing data distributions.
- Interpretation of a confusion matrix heatmap.
- ROC Curve and AUC as evaluation tools for binary classification.
- Why ROC curves require predicted probabilities (`predict_proba()`) instead of predicted classes (`predict()`).
- Importance of comparing models visually using ROC curves.
- Purpose of `plt.legend()`, `plt.tight_layout()`, `plt.savefig()`, `plt.xticks()`, and `ha="right"` in Matplotlib.

# Task 7 - HR Insights & Business Recommendations

## Business Learnings

- Learned that machine learning should support HR decision-making rather than replace human judgment.
- Understood how to translate technical model results into business-friendly recommendations for non-technical stakeholders.
- Identified that employee attrition is influenced by multiple factors rather than salary alone.
- Learned how data-driven insights can help HR identify employees who may require additional support before they decide to leave.
- Understood the importance of balancing employee well-being with organizational productivity through smart work and effective workload management.

## Communication Learnings

- Learned how to write an executive summary for a non-technical HR audience.
- Improved my ability to explain machine learning results using business language instead of technical terminology.
- Learned that presenting actionable recommendations is as important as building accurate machine learning models.
