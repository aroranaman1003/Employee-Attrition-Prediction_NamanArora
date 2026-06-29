# Project Journal

## Day 1

### Completed

- Project setup completed.
- GitHub repository created and connected.
- README.md created.
- requirements.txt created.
- Dataset loaded successfully.
- Displayed first 10 rows.
- Identified target variable.
- Calculated attrition rate.
- Identified numerical and categorical columns.
- Completed Task 1.

## Day 2

### Completed

* Verified there were no missing values in the dataset.
* Removed irrelevant columns after analyzing their usefulness.
* Converted the target variable into numerical format.
* Performed One-Hot Encoding on categorical features.
* Standardized continuous numerical features using StandardScaler.
* Completed Task 2 - Data Cleaning & Preprocessing.

### Next Goal

Begin Exploratory Data Analysis (EDA) to identify patterns in employee attrition and generate business insights.

# Project Journal

## Exploratory Data Analysis (Task 3)

### Completed

* Performed department-wise attrition analysis.
* Analyzed attrition across different job roles.
* Investigated the relationship between monthly income and employee attrition using salary ranges.
* Analyzed work-life balance ratings and their relationship with attrition.
* Examined attrition across years at the company using experience ranges.
* Documented observations for every analysis.
* Derived business insights from exploratory data analysis.

### Challenges Faced

* Initially grouped `MonthlyIncome` directly, which produced misleading results due to many unique salary values.
* Improved the analysis by creating salary ranges using `pd.cut()`.
* Learned the importance of choosing the appropriate analysis based on the type of feature.

### Key Takeaways

* EDA is about extracting meaningful business insights rather than only generating visualizations.
* Understanding the data is as important as building predictive models.
* Feature type (continuous, ordinal, categorical) determines the appropriate analysis technique.


# Task 4 and 5 - Model Building & Evaluation

## Completed
- Split the dataset into training and testing sets.
- Trained Logistic Regression, Random Forest, and Gradient Boosting models.
- Evaluated each model using Precision, Recall, F1-Score, ROC-AUC, and Confusion Matrix.
- Compared all models using a comparison table.
- Identified Logistic Regression as the best-performing model.
- Extracted and ranked the top features influencing employee attrition.

## Challenges Faced
- Understood why Accuracy is not an ideal metric for imbalanced datasets.
- Learned when to use Logistic Regression coefficients instead of tree-based feature importance.

## Key Takeaways
- Model evaluation should consider multiple metrics rather than Accuracy alone.
- Different algorithms explain feature influence differently.
- Business interpretation is an essential part of a machine learning project.



# Session 4 - Data Visualization

## Completed

- Visualized attrition rates by department.
- Visualized attrition rates by job role.
- Compared salary distributions using a box plot.
- Generated a confusion matrix for the best-performing model.
- Visualized the Top 10 most influential features.
- Compared all trained models using an ROC Curve.

## Key Learnings

- Different visualizations communicate different aspects of the data.
- ROC Curves provide a comprehensive comparison of classification models.
- Logistic Regression coefficients explain both the strength and direction of feature influence.
- Proper visualization improves the interpretability of machine learning models.

