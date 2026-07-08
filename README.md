### Customer Churn Prediction using Machine Learning

#### Project Overview

Customer churn prediction is one of the most important applications of machine learning in customer relationship management. Identifying customers who are likely to discontinue a service enables organizations to implement targeted retention strategies, improve customer satisfaction, and reduce revenue loss.

This project develops an end-to-end supervised machine learning pipeline using the IBM Telco Customer Churn dataset. The workflow covers data preprocessing, exploratory data analysis (EDA), feature engineering, model development, model evaluation, hyperparameter tuning, feature interpretation, and model persistence.

---

#### Business Problem

Customer acquisition is often more expensive than customer retention. Organizations need the ability to identify customers who are at risk of leaving so that proactive retention strategies can be implemented.

The objective of this project is to build a machine learning model capable of predicting whether a customer is likely to churn based on demographic information, service subscriptions, account details, and billing history.

---

#### Objectives

* Perform comprehensive data exploration and preprocessing.
* Analyze customer behavior using exploratory data analysis (EDA).
* Build multiple machine learning classification models.
* Compare model performance using multiple evaluation metrics.
* Select the best-performing model.
* Optimize the selected model using hyperparameter tuning.
* Interpret the model to identify important business factors associated with customer churn.
* Save the final model for future inference and deployment.

---

#### Dataset

**Dataset:** IBM Telco Customer Churn Dataset

**Number of Records:** 7,043

**Number of Features:** 21

**Target Variable:** Churn

The dataset contains customer demographic information, subscribed services, billing details, contract information, and whether the customer discontinued the service.

---

#### Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Joblib
* Jupyter Notebook

---

#### Project Workflow

1. Import Libraries
2. Load the Dataset
3. Explore the Dataset
4. Data Cleaning and Preprocessing
5. Exploratory Data Analysis (EDA)
6. Feature Engineering
7. Train-Test Split
8. Feature Scaling
9. Machine Learning Model Development
10. Model Performance Comparison
11. Best Model Selection
12. Hyperparameter Tuning
13. Feature Interpretation
14. Save the Final Model
15. Project Summary
16. Conclusion

---

#### Machine Learning Models Evaluated

* Logistic Regression
* Decision Tree Classifier
* Random Forest Classifier
* K-Nearest Neighbors (KNN)
* Support Vector Machine (SVM)
* Gaussian Naive Bayes
* XGBoost Classifier

---

#### Model Performance Summary

| Model                |   Accuracy |  Precision |     Recall |   F1-Score |
| -------------------- | ---------: | ---------: | ---------: | ---------: |
| Logistic Regression  | **80.38%** | **64.76%** | **57.49%** | **60.91%** |
| Random Forest        |     78.96% |     62.58% |     51.87% |     56.73% |
| XGBoost              |     77.83% |     58.91% |     54.81% |     56.79% |
| Gaussian Naive Bayes |     64.46% |     41.84% | **86.36%** |     56.37% |
| K-Nearest Neighbors  |     75.41% |     53.74% |     53.74% |     53.74% |
| Decision Tree        |     71.86% |     47.01% |     46.26% |     46.63% |

**Best Model:** Logistic Regression

Although hyperparameter tuning was performed using GridSearchCV, the baseline Logistic Regression model achieved the best performance on the test dataset and was selected as the final model.

---

#### Key Business Insights

* Customers with Fiber Optic Internet Service showed a higher likelihood of churn.
* Electronic Check payment method was associated with increased churn.
* Customers with longer tenure were significantly less likely to churn.
* One-year and two-year contracts were associated with better customer retention.
* Online Security and Tech Support services were linked to lower churn rates.

These findings can support customer retention initiatives by helping organizations identify high-risk customers and implement targeted intervention strategies.

---

#### Project Structure

```text
Customer_Churn_Prediction/
│
├── data/
│   └── Telco-Customer-Churn.csv
│
├── notebook/
│   └── Customer_Churn_Prediction.ipynb
│
├── images/
│
├── models/
│   ├── customer_churn_logistic_regression_model.pkl
│   └── customer_churn_standard_scaler.pkl
│
├── results/
│   └── model_comparison.csv
│
├── requirements.txt
├── README.md
├── LICENSE
└── .gitignore
```

---

#### Installation

Clone the repository:

```bash
git clone <repository-url>
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the notebook and execute all cells sequentially.

---

#### Future Enhancements

* Apply advanced feature engineering techniques.
* Investigate class imbalance methods such as SMOTE.
* Perform broader hyperparameter optimization.
* Explore ensemble and stacking methods.
* Deploy the model using Flask, FastAPI, or Streamlit.
* Monitor model performance using real-world customer data.

---

#### Author

**Pratap N**

Data Science | Machine Learning | Deep Learning Enthusiast

---
