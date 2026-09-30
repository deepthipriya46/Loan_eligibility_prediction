# 🏦 Loan Eligibility Prediction Using Machine Learning

A machine learning project that predicts whether a loan applicant is **Eligible** or **Not Eligible** based on demographic, financial, employment, credit history, and property-related information.

The project performs data preprocessing, exploratory data analysis, feature encoding, model comparison, and classification using multiple machine learning algorithms, with **Logistic Regression selected as the final model**.

---

## 📊 Overview

### Problem Statement

Loan approval is an important decision for financial institutions. Manually evaluating every applicant can be time-consuming and may lead to inconsistent decisions.

This project aims to build a machine learning model that can predict loan eligibility based on applicant information.

The target variable is:

- `1` → Eligible / Approved
- `0` → Not Eligible / Not Approved

### Objectives

The main objectives of this project are:

- Understand and analyze the loan application dataset.
- Handle missing values and duplicate records.
- Perform exploratory data analysis (EDA).
- Encode categorical variables.
- Prepare features for machine learning.
- Split the dataset into training and testing sets.
- Train multiple classification models.
- Compare model performance using evaluation metrics.
- Select the most suitable model.
- Predict loan eligibility for new applicants.

---

## 🔍 Dataset Features

The dataset contains information about loan applicants.

| Feature | Description |
|---|---|
| `Loan_ID` | Unique identifier for the loan application |
| `Gender` | Gender of the applicant |
| `Married` | Marital status |
| `Dependents` | Number of dependents |
| `Education` | Education level |
| `Self_Employed` | Whether the applicant is self-employed |
| `ApplicantIncome` | Applicant's income |
| `CoapplicantIncome` | Co-applicant's income |
| `LoanAmount` | Requested loan amount |
| `Loan_Amount_Term` | Loan repayment term |
| `Credit_History` | Applicant's credit history |
| `Property_Area` | Property location |
| `Loan_Status` | Target variable indicating loan eligibility |

---

## 📂 Data Source

The dataset is a commonly used loan prediction dataset containing approximately 600 loan applications and 13 columns.

A public version of the dataset is available on Kaggle:

**Dataset:** Loan Predication / Loan Prediction Dataset  
**Source:** Kaggle

[View Dataset on Kaggle](https://www.kaggle.com/ninzaami/loan-predication)

The dataset contains applicant information such as income, education, employment status, credit history, loan amount, and property area. 

---

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

1. Checked the shape and structure of the dataset.
2. Inspected data types.
3. Identified missing values.
4. Handled missing categorical values using the mode.
5. Handled missing numerical values.
6. Checked for duplicate records.
7. Removed unnecessary identifier information.
8. Encoded categorical variables.
9. Separated independent and dependent variables.
10. Split the dataset into training and testing sets.
11. Applied feature scaling for Logistic Regression.

---

## 📈 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand relationships and patterns within the dataset.

The analysis included:

- Distribution of applicant income.
- Distribution of loan amounts.
- Education analysis.
- Gender analysis.
- Marital status analysis.
- Credit history analysis.
- Property area analysis.
- Loan eligibility distribution.
- Correlation analysis.
- Data visualization using Matplotlib and Seaborn.

---

## 🤖 Machine Learning Models

Three classification algorithms were implemented and compared:

### 1. Logistic Regression

Logistic Regression was used as the primary baseline classification model.

**Accuracy: 86.18%**

### 2. Random Forest

Random Forest was implemented to evaluate whether an ensemble of decision trees could improve prediction performance.

**Accuracy: 83.74%**

### 3. XGBoost

XGBoost was implemented as a gradient boosting-based classification model.

**Accuracy: 83.74%**

---

## 📊 Model Comparison

The models were evaluated using Accuracy, Precision, Recall, and F1-score.

| Model | Accuracy | Precision | Recall | F1-score |
|---|---:|---:|---:|---:|
| **Logistic Regression** | **86.18%** | 0.840 | **0.988** | **0.908** |
| Random Forest | 83.74% | **0.849** | 0.929 | 0.888 |
| XGBoost | 83.74% | 0.828 | 0.965 | 0.891 |

Based on the evaluated test-set results, **Logistic Regression was selected as the final model** because it achieved the highest accuracy and F1-score among the three tested models.

---

## 📌 Final Model

### Logistic Regression

The final Logistic Regression model achieved:

- **Accuracy:** 86.18%
- **Precision:** 0.840
- **Recall:** 0.988
- **F1-score:** 0.908

The model was evaluated using:

- Confusion Matrix
- Classification Report
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC analysis

----
🛠️ Technologies Used
- Programming Language
- Python 3.x
- Data Processing
- Pandas
- NumPy
- Data Visualization
 -Matplotlib
- Seaborn
- Machine Learning
- Scikit-learn
- XGBoost
- Model Saving
- Joblib
- Development Environment
- Jupyter Notebook / JupyterLab

