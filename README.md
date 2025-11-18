# Breast Cancer Diagnosis Classifier (Logistic Regression)

This project implements a binary classifier using **Logistic Regression** to predict breast mass diagnosis (Malignant/Benign).

## 🎯 Goal

To build, train, and evaluate a Logistic Regression model on a medical dataset, focusing on key metrics like **Precision**, **Recall**, and **ROC-AUC**.

## 📊 Dataset & Preprocessing

* **Dataset:** Breast Cancer Wisconsin (Diagnostic) Dataset.
* **Target:** `diagnosis` (Malignant $\rightarrow$ 1, Benign $\rightarrow$ 0).
* **Preprocessing:** Features were **standardized** using `StandardScaler` to prepare them for the model.

## ⚙️ Key Results (Test Set)

The model showed excellent performance, demonstrating strong separability between the two classes.

| Metric | Score | Interpretation |
| :--- | :--- | :--- |
| **ROC-AUC** | **0.9975** | Near-perfect class distinction. |
| **Precision** | 0.9836 | High certainty in Malignant predictions. |
| **Recall** | 0.9375 | Catches the vast majority of true Malignant cases. |

### 📈 Threshold Tuning

By lowering the classification threshold from $0.5$ to $0.3$, **Recall** was improved from $0.9375$ to **$0.9688$** (reducing False Negatives from 4 to 2), which is critical for minimizing missed diagnoses in a medical context.
