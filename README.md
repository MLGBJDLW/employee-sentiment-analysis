# 🧠 Employee Sentiment Analysis – Final Summary

This project analyzes internal employee email communications to assess sentiment trends, engagement risks, and behavioral patterns using NLP and machine learning techniques.

---

## 📌 Project Overview

We apply a pipeline of GPT-based sentiment classification, feature engineering, and predictive modeling to derive insights from employee communications.

Key goals include:
- Labeling each message with sentiment (Positive / Neutral / Negative)
- Aggregating sentiment scores monthly per employee
- Detecting high-risk behavior patterns
- Modeling future sentiment trends with ML regressors

---

## ✅ Key Features

### 🔠 Sentiment Labeling
Used **OpenAI GPT-4o** to classify raw email content based on tone and intent.

### 📊 EDA & Visualization
- Distribution of sentiment classes
- Monthly average sentiment trends
- High-risk employee identification

### 🧮 Modeling
Trained and compared:
- Linear Regression
- Random Forest
- MLP Neural Network
- Logistic Regression (for binary classification)

Each model evaluated using **R²**, **RMSE**, and confusion matrices.

---

## 🏆 Employee Rankings

- Top 3 Most Positive Employees
- Top 3 Most Negative Employees
- Employees flagged as potential flight risks

See: `Output/employee_rankings.csv`, `Output/risk_employees.csv`

---

## 📈 Model Performance Summary
| Model               | Type           | R² / Accuracy | RMSE     |
| ------------------- | -------------- | ------------- | -------- |
| Linear Regression   | Regression     | 0.794569      | 0.430228 |
| Random Forest       | Regression     | 0.756679      | 0.468226 |
| MLP Neural Network  | Regression     | 0.791572      | 0.433355 |
| Logistic Regression | Classification | 0.338028      | –        |

