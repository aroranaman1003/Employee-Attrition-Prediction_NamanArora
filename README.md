# Employee Attrition Prediction

A Machine Learning project that predicts employee attrition and provides HR-focused business insights using the IBM HR Analytics dataset.

## Project Overview

This project uses Machine Learning to predict whether an employee is likely to leave an organization based on HR analytics data. The objective is to help HR teams identify employees at risk of attrition, understand the factors contributing to employee turnover, and support better retention strategies through data-driven insights.

---

## Features

- Employee Attrition Prediction using Machine Learning
- Comprehensive Data Preprocessing Pipeline
- Exploratory Data Analysis (EDA)
- Multiple Classification Models
- Model Performance Comparison
- Business-Oriented HR Insights
- Professional Data Visualizations
- Executive Summary for HR Decision Makers

## Problem Statement

Employee attrition can lead to increased recruitment costs, loss of experienced talent, and reduced organizational productivity. This project analyzes employee data to identify patterns associated with attrition and builds predictive models that assist HR in making informed retention decisions.

---

## Dataset

**Dataset:** IBM HR Analytics Employee Attrition Dataset

The dataset contains employee information such as:

- Age
- Department
- Job Role
- Monthly Income
- Business Travel
- Work-Life Balance
- Overtime
- Years at Company
- Marital Status
- Education
- Attrition (Target Variable)

---

## Project Workflow

### Task 1 - Data Loading & Exploration
- Loaded the dataset
- Explored dataset dimensions and features
- Identified target variable
- Checked missing values

### Task 2 - Data Cleaning & Preprocessing
- Removed irrelevant columns
- Encoded categorical variables
- Standardized numerical features
- Prepared training and testing datasets

### Task 3 - Exploratory Data Analysis (EDA)
- Department-wise attrition analysis
- Job role-wise attrition analysis
- Salary vs attrition analysis
- Work-Life Balance vs attrition
- Years at Company vs attrition
- Business insights from EDA

### Task 4 - Model Building
Built and trained the following classification models:

- Logistic Regression
- Random Forest Classifier
- Gradient Boosting Classifier

### Task 5 - Model Evaluation
Evaluated all models using:

- Precision
- Recall
- F1 Score
- ROC-AUC Score
- Confusion Matrix

Compared model performance and identified the best-performing model.

### Task 6 - Data Visualization
Created visualizations including:

- Attrition by Department
- Attrition by Job Role
- Monthly Income Box Plot
- Confusion Matrix
- Top 10 Feature Importance
- ROC Curve Comparison

### Task 7 - HR Insights & Business Recommendations
Generated business-focused insights including:

- Strongest predictors of employee attrition
- High-risk departments and job roles
- Salary impact analysis
- HR recommendations
- Model limitations
- Executive Summary for HR Director

---

## Models Used

- Logistic Regression
- Random Forest Classifier
- Gradient Boosting Classifier

---

## Key Findings

- Employees working overtime were more likely to leave the organization.
- Frequent business travel increased the likelihood of employee attrition.
- Sales Representatives experienced the highest attrition rate among all job roles.
- The Sales department recorded the highest employee attrition.
- Employee attrition is influenced by multiple factors rather than salary alone.

---

## Visualizations

The project includes:

- Department-wise Attrition
- Job Role-wise Attrition
- Monthly Income Box Plot
- Confusion Matrix
- ROC Curve Comparison
- Top 10 Feature Importance

---

## Project Structure

```text
Employee-Attrition-Prediction/
│
├── charts/
├── notebooks/
│   └── analysis.ipynb
│
├── notes/
│   ├── learnings.md
│   └── project_journal.md
│
├── reports/
│   └── summary.docx
│
├── README.md
├── requirements.txt
└── WA_Fn-UseC_-HR-Employee-Attrition.csv
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/aroranaman1003/Employee-Attrition-Prediction_NamanArora
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
notebooks/analysis.ipynb
```

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## Future Improvements

- Hyperparameter tuning
- Cross-validation
- Explainable AI using SHAP or LIME
- Deployment as a web application
- Real-time employee attrition prediction

---

## Author

**Naman Arora**

B.Tech Computer Science Engineering

Machine Learning | Cybersecurity | Software Development

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.