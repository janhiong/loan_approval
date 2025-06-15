# Predicting Loan Approval Using Machine Learning

**INFO 213: Data Science Programming II**  
College of Computing and Informatics, Drexel University  
**Authors:** Janhi Ong, Jayda Foo  
**Date:** May 20, 2025

## 📌 Project Overview

This project applies multiple machine learning techniques to predict loan approval status based on applicant financial and personal attributes. The goal is to evaluate the effectiveness of models such as Perceptron, Adaline, Logistic Regression, and Random Forest in classifying whether a loan should be approved or rejected.

---

## 📂 Dataset

- **Source:** Provided as `loan_approval_dataset.csv`
- **Size:** 4,269 records × 13 features
- **Key Features:**
  - `income_annum`: Annual income of the applicant
  - `loan_amount`: Amount of the loan requested
  - `cibil_score`: Credit score
  - `education`, `self_employed`, `no_of_dependents`, and asset values
  - `loan_status`: Target variable (Approved / Rejected)

---

## 🧠 Methodology

### 🔎 1. Data Preprocessing
- Removed irrelevant ID fields
- Cleaned column names and missing values
- Converted categorical variables using one-hot encoding

### 📊 2. Exploratory Data Analysis
- Analyzed the relationship between loan approval and:
  - Loan amount, income, and credit score
  - Asset values (residential, commercial, luxury, bank)
  - Education and employment status

### 🛠 3. Model Building
Trained and tuned the following models:
- **Perceptron**
- **Adaline**
- **Logistic Regression**
- **Random Forest**

Applied standardization (MinMaxScaler / StandardScaler) when appropriate and used grid search for hyperparameter tuning.

---

## 📈 Results

| Model              | Accuracy |
|-------------------|----------|
| Perceptron        | 88.8%    |
| Adaline           | 67.1%    |
| Logistic Regression (Tuned) | 92.3%    |
| Random Forest (Tuned)       | **98.1%** |

✅ **Random Forest** was the best performer with nearly perfect precision and recall on both classes.

---

## 🧪 Key Insights

- Credit score (`cibil_score`) is the strongest predictor of loan approval.
- Asset values and income show significant correlation.
- Education and employment status had minimal predictive power.

---

## 📁 Repository Structure

