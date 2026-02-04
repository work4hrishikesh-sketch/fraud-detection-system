# Fraud Detection in Financial Transactions

## Project Overview
This project focuses on detecting fraudulent financial transactions using machine learning techniques. The goal is to build a predictive model that can identify suspicious transactions and provide meaningful insights to help reduce financial risk.

The project follows an end-to-end data science workflow, including data cleaning, feature engineering, model development, evaluation, and business interpretation.

---

## Dataset Description
The dataset contains transaction-level data from a simulated financial system, with over 6 million records. Each transaction includes details such as transaction type, transaction amount, account balances before and after the transaction, and a fraud indicator.

The target variable (`isFraud`) is highly imbalanced, with fraudulent transactions representing a very small portion of the data.

---

## Approach
The following steps were performed in this project:

- Data loading and initial exploration  
- Removal of irrelevant identifier columns  
- Feature engineering using balance difference features  
- Log transformation of transaction amount to handle skewness  
- Handling class imbalance using class-weighted models  
- Model training using Logistic Regression and Random Forest  
- Model evaluation using recall, precision, ROC-AUC, and confusion matrix  

---

## Models Used
- **Logistic Regression**  
  Used as a baseline model due to its interpretability and simplicity.

- **Random Forest Classifier**  
  Used to capture non-linear relationships and improve fraud detection performance.

---

## Key Insights
- Fraudulent transactions are mainly associated with TRANSFER and CASH_OUT transaction types.
- High transaction amounts and abnormal balance changes are strong indicators of fraud.
- Balance difference features significantly improve the model’s ability to detect fraud.
- Recall and ROC-AUC are more reliable evaluation metrics than accuracy for this problem.

---

## Business Impact
The insights from this project can be used to implement real-time fraud detection systems, apply dynamic transaction thresholds, and strengthen security measures such as multi-factor authentication for high-risk transactions.

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## Conclusion
This project demonstrates an effective and practical approach to fraud detection using machine learning. The model and insights can be extended and integrated into real-world financial systems to enhance fraud prevention strategies.
