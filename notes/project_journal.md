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

