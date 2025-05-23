# 📊 Employee Sentiment Analysis – Final Summary

## 🔍 Project Overview

This project analyzes internal employee email communications to assess sentiment trends and potential engagement risks. Using GPT-based sentiment classification, exploratory data analysis, and predictive modeling, we derive meaningful insights into employee behavior and morale.

---

## ✅ Key Tasks and Methodology

- **Sentiment Labeling**: Used OpenAI GPT-4o to label each message as Positive, Neutral, or Negative.
- **EDA**: Analyzed sentiment distribution and monthly sentiment trends.
- **Scoring**: Assigned +1/-1/0 to messages and aggregated monthly scores per employee.
- **Ranking**: Identified top 3 positive and negative employees for each month.
- **Flight Risk Detection**: Flagged employees with 4+ negative messages in any 30-day window.
- **Modeling**: Built Linear Regression, Random Forest, MLP, and Logistic Regression models to predict sentiment scores.

---

## 🏆 Employee Rankings (Latest Month)

**Top 3 Positive Employees**:
- Eric Bass
- John Arnold
- Bobette Riner

**Top 3 Negative Employees**:
- *(Data from latest month; none heavily negative)*

---

## 🚨 Flight Risk Employees

> No employees were flagged as flight risks under the rule:  
> *4 or more negative messages within any rolling 30-day period*.

---

## 📈 Model Performance Summary

| Model               | Type           | R² / Accuracy | RMSE     |
|--------------------|----------------|---------------|----------|
| Linear Regression  | Regression     | 0.761407      |0.576588  |
| Random Forest      | Regression     | 0.744090      | 0.597146 |
| MLP Neural Network | Regression     | -0.115005     | 1.24645  |
| Logistic Regression| Classification | 0.468085      | —        |

---

## 📂 Project Structure

- `Data_Intern.ipynb`: All analysis code
- `Final_Report_Employee_Sentiment.docx`: Formal report with findings and visuals
- `/output/`: Processed CSV files like scores, rankings, flight risks
- `/visualization/`: All charts and graphs

---

## ✅ Recommendations

- Monitor sentiment trends regularly
- Investigate consistent low scorers and at-risk employees
- Use Random Forest for monthly score forecasting
