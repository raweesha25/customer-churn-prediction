# 📊 Customer Churn Prediction

## 📌 Project Overview
Customer churn is a major challenge in the telecom industry. Companies need to identify customers who are likely to leave so they can take preventive actions.

This project builds a machine learning model to:
- Predict customer churn
- Identify key factors influencing churn
- Provide business recommendations to reduce churn

---

## 🎯 Objective
To classify customers into:
- **Churn (1)** → Likely to leave
- **Not Churn (0)** → Likely to stay

---

## 📁 Dataset
- **Dataset:** Telco Customer Churn Dataset
- **Total Records:** 7032 customers
- **Features:** 21 columns including:
  - Demographics (gender, senior citizen)
  - Services (internet, phone, streaming)
  - Billing (monthly charges, total charges)
  - Contract details

---

## 🛠️ Tools & Technologies
- Python
- Pandas & NumPy
- Matplotlib & Seaborn
- Scikit-learn

---

## ⚙️ Project Workflow

### 1️⃣ Data Cleaning
- Converted `TotalCharges` to numeric
- Handled missing values
- Removed unnecessary column (`customerID`)
- Encoded target variable (`Churn → 0/1`)

---

### 2️⃣ Exploratory Data Analysis (EDA)

Performed visual analysis to understand patterns:

- Churn distribution
- Contract type vs churn
- Internet service vs churn
- Tech support vs churn
- Monthly charges vs churn
- Tenure vs churn

---

## 🔍 Key Insights

- Customers with **month-to-month contracts** have the highest churn
- Customers with **low tenure** are more likely to leave early
- **Fiber optic users** show higher churn compared to DSL users
- Customers without **tech support** are more likely to churn
- Higher **charges** are associated with higher churn

---

## 🤖 Model Building

### 🔹 Logistic Regression (Best Model)
- Accuracy: **80.4%**
- ROC-AUC: **0.836**
- Recall (Churn): **57%**

### 🔹 Random Forest
- Accuracy: **78.4%**
- ROC-AUC: **0.812**
- Recall (Churn): **47%**

---

## 📊 Model Comparison

| Model                | Accuracy | ROC-AUC | Recall (Churn) | F1-score |
|---------------------|----------|--------|----------------|----------|
| Logistic Regression | 0.804    | 0.836  | 0.57           | 0.61     |
| Random Forest       | 0.784    | 0.812  | 0.47           | 0.54     |

👉 Logistic Regression performed better overall.

---

## 📈 Feature Importance

Top features influencing churn:

### 🚨 Increase Churn
- Month-to-month contract
- Fiber optic internet
- High total charges

### ✅ Reduce Churn
- Longer tenure
- Two-year contracts
- DSL internet

---

## 💼 Business Recommendations

- Encourage customers to switch to **long-term contracts**
- Improve **early customer experience**
- Offer **loyalty programs**
- Investigate issues with **fiber optic service**
- Provide **better customer support services**

---

## 🚀 How to Run the Project

### Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
