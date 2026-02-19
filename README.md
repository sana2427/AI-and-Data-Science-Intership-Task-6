# Task 1: Term Deposit Subscription Prediction (Bank Marketing)

## Overview
This repository contains the solution for **Task 1: Term Deposit Subscription Prediction**, completed as part of my AI & Data Science Internship tasks.

The project builds a machine learning system that predicts whether a bank customer will subscribe to a term deposit after a marketing campaign.

---

## Objective
The objective of this task is to:

- Predict customer subscription (Yes/No)
- Reduce unnecessary marketing calls
- Improve campaign success rate
- Understand customer behavior using Explainable AI (LIME)

---

## Dataset
**Dataset Name:** Bank Marketing Dataset  
**Type:** Structured CSV dataset

### Target Variable
`y` → Term Deposit Subscription  
- yes → Customer subscribed
- no → Customer did not subscribe

### Features (Examples)
- Age
- Job
- Marital Status
- Education
- Balance
- Housing Loan
- Contact Type
- Month
- Campaign Calls
- Previous Outcome
- Call Duration

---

## Tools & Technologies Used
- Python
- NumPy
- pandas
- Matplotlib
- Seaborn
- Scikit-learn
- LIME (Explainable AI)
- Jupyter Notebook / Google Colab

---

## Full Preview of Notebook Output

```
https://nbviewer.org/github/sana2427/AI-and-Data-Science-Intership-Task-6/blob/main/DS_Internship_Task_6.ipynb
```

---

## Approach

### 1️⃣ Data Loading
- Loaded dataset using `pandas.read_csv()`
- Converted CSV into DataFrame for analysis

### 2️⃣ Data Inspection
Used:
- `.shape`
- `.info()`
- `.head()`
- `.isnull().sum()`

Checked dataset structure and class imbalance.

### 3️⃣ Data Preprocessing
- Converted target variable (yes/no → 1/0)
- Separated categorical & numerical features
- Applied One-Hot Encoding to categorical data
- Scaled numerical features
- Split dataset into training and testing sets

### 4️⃣ Model Training
Trained two classification models:

**Logistic Regression**
- Baseline model

**Random Forest**
- Advanced model for complex patterns

### 5️⃣ Model Evaluation
Evaluated using:
- Confusion Matrix
- F1 Score
- ROC Curve (AUC Score)

### 6️⃣ Explainable AI (LIME)
- Explained 5 individual predictions
- Identified which features influenced decisions
- Made model decisions interpretable

---

## Results & Insights
- Random Forest performed better than Logistic Regression
- Call duration strongly affects subscription
- Previous successful campaign increases probability
- Short calls usually lead to rejection
- Dataset is highly imbalanced (most customers say No)
- F1 score is more reliable than accuracy

---

## Conclusion
This task demonstrates a complete machine learning workflow including preprocessing, classification modeling, evaluation, and explainability.

The model successfully predicts potential customers and explains why the prediction was made.  
Such a system can help banks target interested customers, reduce marketing costs, and improve campaign efficiency.

---

## Skills Gained
- Classification Modeling
- Feature Encoding
- Model Evaluation (F1, ROC, Confusion Matrix)
- Explainable AI using LIME
- Customer Behavior Analysis
