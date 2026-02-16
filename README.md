# 💳 AI-Powered Financial Fraud Detection System

This project focuses on detecting fraudulent financial transactions 
using machine learning techniques under extreme class imbalance 
conditions across 6.3M+ real-world transactions.

---

## 🎯 Problem Statement

Financial fraud detection is a critical task where fraudulent 
transactions represent a very small fraction of total transactions. 
The challenge lies in accurately identifying fraud while minimizing 
false positives on a dataset with only 0.13% fraud rate.

---

## ⚙️ Tech Stack
Python | Scikit-learn | Pandas | NumPy | 
Matplotlib | Seaborn | Joblib | Jupyter Notebook

---

## 🧠 Approach

- Performed detailed Exploratory Data Analysis (EDA)
- Engineered balance-based and transaction-based features
- Handled class imbalance using class-weighted learning
- Built an end-to-end machine learning pipeline
- Trained a Logistic Regression model for fraud classification
- Saved the trained pipeline using `joblib` for reuse 
  without retraining

---

## 📊 Model Performance

| Metric | Score |
|---|---|
| Overall Accuracy | 94.67% |
| Fraud Recall | 94% |
| True Fraud Caught | 2,313 / 2,464 cases |
| Dataset Size | 6.3M transactions |
| Fraud Rate | Only 0.13% (extreme imbalance) |

> ✅ High recall on fraud class (94%) ensures most fraudulent 
> transactions are flagged — critical in real-world financial 
> systems where missing fraud is costlier than false alarms.

---

## 🔍 Key Data Insights

- Fraud occurs **exclusively** in TRANSFER & CASH_OUT types
- Account draining pattern (oldbalance > 0 → newbalance = 0) 
  is the strongest fraud signal
- Engineered features `balanceDiffOrig` & `balanceDiffDest` 
  significantly improved detection
- 1,188,074 zero-balance-after-transfer cases identified 
  as high-risk patterns

---

## 🤖 Model

- Algorithm: Logistic Regression
- Handling Imbalance: Class-weighted loss
- Output: Binary classification (Fraud / Not Fraud)

---

## 📁 Repository Structure

- `data/` → Dataset description and source link
- `notebooks/` → Complete model development notebook
- `model/` → Trained fraud detection pipeline
- `requirements.txt` → Project dependencies

---

## ✨ Key Highlights

- No dataset uploaded due to large size (6.3M records)
- Model trained once and reused via saved pipeline
- Suitable for real-world deployment scenarios

---

## 🚀 Future Enhancements

- Threshold tuning using Precision-Recall tradeoff
- Ensemble models (Random Forest, XGBoost) for improved recall
- Deployment using REST API or Streamlit dashboard
- Real-time fraud scoring pipeline

---

## 📧 Contact

Feel free to connect for collaboration, internships, 
or project discussions.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/kokila-m-ai-ds/)
[![Email](https://img.shields.io/badge/Email-Contact-red)](mailto:kokilakoki3376@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black)](https://github.com/kokilamariyayi)
