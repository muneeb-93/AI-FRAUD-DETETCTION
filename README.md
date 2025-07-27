# AI-FRAUD-DETECTION(HSBC HACKATHON)
# 🛡️ AI-Powered Fraud Detection System

This project was built for the HSBC ML Hackathon. It detects fraudulent transactions in real-time using a hybrid ML approach.

---

## 📌 Problem Statement

Design a real-time fraud detection model using **innovative ML techniques**, not conventional rule-based methods, to minimize false positives and maximize actual fraud detection.

---

## 📂 Dataset

- Provided anonymized transaction data
- Highly imbalanced: <2% fraud
- Columns: step, customer, merchant, category, gender, amount, fraud, etc.

---

## 🧠 Models Used

### 🔹 1. AutoEncoder (Unsupervised)
- Learns only from normal data
- Flags high reconstruction error as fraud

### 🔹 2. CatBoost (Supervised)
- Works great with categorical data
- High accuracy + explainability

### 🔸 Hybrid Approach:
- Combines AutoEncoder error with CatBoost features
- Boosts detection power and precision

---

## 📊 Results

| Model       | Precision | Recall | F1-Score | AUC    |
|-------------|-----------|--------|----------|--------|
| CatBoost    | 0.89      | 0.76   | 0.82     | 0.997  |
| AutoEncoder | 0.23      | 0.16   | 0.19     | 0.948  |

- Final model: **Hybrid CatBoost + AE**
- Inference Time: **0.0026s per 100 samples**
- Model Size: **225 KB**

---

## 📈 Features

- 📌 Anomaly-based learning (AutoEncoder)
- ✅ Categorical boosting (CatBoost)
- 🚀 Hybrid fusion for robustness
- 📉 SHAP explainability (planned)
- 🧠 Future-ready for deployment

---

## 🏁 Final Output

- Accepts new test dataset
- Returns `submission.csv` with fraud predictions


