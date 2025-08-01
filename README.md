# ml-fraud-detection
ML-based fraud detection using XGBoost and oversampling on transactional data.

# 💼 Fraud Detection with XGBoost

This project involves building a machine learning pipeline to proactively detect fraudulent transactions from financial datasets. It uses XGBoost for classification, applies oversampling to handle class imbalance, and includes end-to-end data preprocessing, model tuning, and evaluation.

---

## 📊 Project Objective

Detect fraudulent financial transactions using machine learning techniques and optimize for high recall to reduce the chance of undetected fraud.

---

## 🛠️ Tools & Technologies

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn
- SHAP (for feature importance)
- Jupyter Notebook

---

## 📁 Dataset Overview

The dataset contains transactional records with the following key fields:
- `amount`, `oldbalanceOrg`, `newbalanceOrig`
- `type` of transaction
- `isFraud` (Target)

---

## ⚙️ Workflow

1. **Data Cleaning**: Checked for missing values, outliers, and multicollinearity.
2. **Exploratory Data Analysis**: Understanding class imbalance and key trends.
3. **Preprocessing**: Label encoding and scaling.
4. **Resampling**: Balanced the dataset using oversampling on training data.
5. **Modeling**: Trained an XGBoost classifier and tuned the threshold.
6. **Evaluation**: Used accuracy, precision, recall, and F1-score.
7. **Explainability**: Used SHAP for feature interpretation.

---

## 📈 Model Performance

| Metric       | Value       |
|--------------|-------------|
| Accuracy     | 100%        |
| Precision    | 52% (fraud) |
| Recall       | 98% (fraud) |
| F1-score     | 0.68 (fraud)|

> ⚠️ High recall ensures that most fraud cases are caught. Precision tradeoff is optimized via threshold tuning.

---

## 🔍 Key Insights

- Fraud is more likely during `TRANSFER` and `CASH_OUT` transactions.
- Balance anomalies (`oldbalanceOrg`, `newbalanceOrig`) are strong fraud indicators.
- Certain high-value transactions with sudden balance drops correlate with fraud.

---

## 🚨 Fraud Prevention Recommendations

- Real-time transaction monitoring
- Multi-level authentication
- Behavioral analytics for anomaly detection
- Regular model retraining

---

## ✅ Conclusion

This project demonstrates how machine learning and proper data handling techniques can help build a robust fraud detection system that balances accuracy and practical deployment constraints.



