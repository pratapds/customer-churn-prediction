# Customer Churn Prediction

## Overview

Customer churn is a critical business problem for subscription-based companies because retaining existing customers is often more cost-effective than acquiring new ones.

This project uses the IBM Telco Customer Churn dataset to predict whether a customer is likely to leave the company. The project follows the complete data science workflow, including data cleaning, exploratory data analysis (EDA), feature engineering, machine learning, model evaluation, and business recommendations.

---

## Project Workflow

1. Data Understanding
2. Data Cleaning
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. Train-Test Split
6. Logistic Regression
7. Random Forest
8. Model Comparison
9. ROC-AUC Analysis
10. Feature Importance Analysis
11. Business Recommendations
12. Conclusion

---

## Dataset

**Dataset:** IBM Telco Customer Churn Dataset

**Records:** 7,043 customers

**Target Variable:** Churn

* Yes = Customer left the company
* No = Customer stayed with the company

---

## Tools and Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

---

## Data Cleaning

The following preprocessing steps were performed:

* Checked for missing values
* Converted TotalCharges from object to numeric format
* Replaced blank TotalCharges values with 0 for customers having zero tenure
* Verified data types
* Prepared data for machine learning

---

## Exploratory Data Analysis

### Key Findings

#### Contract Type

Customers with month-to-month contracts exhibited significantly higher churn rates compared to customers with one-year and two-year contracts.

#### Customer Tenure

Customers who churned had substantially lower tenure than retained customers. Long-term customers were considerably less likely to leave the company.

#### Monthly Charges

Customers paying higher monthly charges were more likely to churn in this dataset.

---

## Feature Engineering

The following feature engineering steps were performed:

* One-Hot Encoding of categorical variables
* Conversion of the target variable (Churn) into binary format
* Preparation of the final machine learning dataset

### Final Dataset

* 7,043 observations
* 30 input features
* 1 target variable (Churn)

---

## Models Used

### Logistic Regression

Used as the baseline classification model.

### Logistic Regression with Feature Scaling

StandardScaler was applied before training.

### Random Forest Classifier

Used for model comparison and feature importance analysis.

---

## Model Performance

| Model                        | Accuracy |
| ---------------------------- | -------- |
| Logistic Regression          | 80.4%    |
| Logistic Regression (Scaled) | 80.7%    |
| Random Forest                | 78.5%    |

### Selected Model

Logistic Regression with feature scaling achieved the best overall performance and was selected as the final model.

---

## ROC-AUC Analysis

**ROC-AUC Score: 0.8418**

A ROC-AUC score of 0.8418 indicates excellent discriminatory power and demonstrates that the model can effectively distinguish between customers who churn and customers who remain with the company.

---

## Important Features

The Random Forest model identified the following features as the most influential predictors of churn:

1. TotalCharges
2. tenure
3. MonthlyCharges
4. PaymentMethod_Electronic check
5. InternetService_Fiber optic
6. Contract_Two year
7. OnlineSecurity_Yes
8. PaperlessBilling_Yes
9. TechSupport_Yes
10. Contract_One year

These findings are consistent with the insights obtained during exploratory data analysis.

---

## Business Recommendations

1. Focus retention efforts on customers during their first year.
2. Encourage customers to move from month-to-month contracts to longer-term contracts.
3. Monitor customers with high monthly charges and provide personalized retention offers.
4. Promote value-added services such as Online Security and Technical Support.
5. Identify high-risk customers early and engage them proactively.

---

## Conclusion

This project successfully developed machine learning models to predict customer churn using the IBM Telco Customer Churn dataset.

Among the evaluated models, Logistic Regression with feature scaling achieved the best overall performance, with an accuracy of approximately 80.7% and a ROC-AUC score of 0.8418.

The analysis revealed that customer tenure, monthly charges, total charges, contract type, and service-related factors are strong indicators of churn. These insights can help businesses improve customer retention strategies and reduce revenue loss.

---

## Repository Structure

Customer-Churn-Prediction/

├── Customer_Churn_Prediction.ipynb

├── README.md

├── data/

│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv

└── images/

    ├── churn_distribution.png

    ├── contract_vs_churn.png

    ├── tenure_vs_churn.png

    ├── monthly_charges_vs_churn.png

    ├── feature_importance.png

    └── roc_curve.png

---

## Author

Pratap N

Certified IBM Data Science Professional(V3)

