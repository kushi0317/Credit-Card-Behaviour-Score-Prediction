# Credit Card Behaviour Score Prediction Using Classification and Risk-Based Techniques

## Overview

Bank A aims to improve its credit risk management framework by developing a **forward-looking Behaviour Score** — a classification model that predicts whether a credit card customer will **default in the following month**.

To achieve this, we use anonymized historical behavioral data of over **30,000 credit card customers**, with a labeled target variable: `default.payment.next.month`. This binary variable indicates whether a customer defaulted on their payment in the **next billing cycle**.

The objective is to build a predictive model that flags potential defaulters **in advance**, enabling the bank to:
- Adjust credit exposure
- Trigger early warning systems
- Prioritize risk-based actions

We aim to go beyond simple prediction to build a **financially interpretable** model that allows the bank to understand **default patterns**, take early action, and better manage credit risk exposure.

---

## Key Objectives

- 📌 Build a **binary classification model** to predict customer default  
  (`default.payment.next.month`: 1 = Default, 0 = No Default)

- ⚖️ Handle **class imbalance** using techniques such as:
  - SMOTE (Synthetic Minority Over-sampling Technique)
  - Class weighting
  - Downsampling

- 📊 Perform **exploratory** and **financial analysis** to understand how behavioral variables impact default risk

- 🔍 Analyze **behavioral trends** beyond standard EDA, including:
  - Payment delays
  - Repayment consistency
  - Credit utilization

- 🛠️ Engineer features that are:
  - **Financially meaningful**
  - Predictive of default risk  
  Examples include:
    - Credit utilization ratio
    - Delinquency streaks

---

## Modeling Approach

### Model Candidates:
- Logistic Regression
- Decision Trees
- Ensemble Methods:
  - XGBoost
  - LightGBM

### Evaluation Metrics:
- Accuracy
- Precision
- Recall
- F1-score
- AUC-ROC

✅ Metrics should reflect **real-world credit risk trade-offs** and be aligned with business needs.

---

## Threshold Tuning and Risk Trade-Off

- Set a **classification threshold** aligned with the bank’s risk appetite.
- Analyze and discuss the **business implications** of false positives and false negatives.
- Justify threshold selection with respect to maximizing cost-effectiveness and risk containment.

---

## Final Deliverables

- Generate **production-style predictions** on an **unlabeled validation dataset**
- Ensure predictions are optimized for the selected evaluation metric by fine-tuning the classification threshold
- Provide **model interpretability** to support financial decision-making and regulatory compliance

---

## Summary

This project aims to deliver not just a high-performing classifier, but also a **strategically useful tool** for credit risk management. By leveraging machine learning, domain-specific feature engineering, and thoughtful metric selection, we empower the bank to make **proactive and financially informed** credit decisions.

