# 🚀 Fraud Detection in Financial Transactions

![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Fraud%20Detection-brightgreen)
![Python](https://img.shields.io/badge/Python-3.x-blue)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📄 Overview

This project aims to detect fraudulent transactions in financial datasets using **Machine Learning**. The focus is on leveraging **Logistic Regression** and **K-Nearest Neighbors (KNN)** to classify transactions as either fraudulent or genuine. 

Through **Exploratory Data Analysis (EDA)**, **Feature Engineering**, and **Model Evaluation**, the project demonstrates practical steps to enhance fraud detection mechanisms and minimize financial risks.

---

## 🎯 Objective

To classify financial transactions as:
- **Fraudulent (1)** or
- **Non-Fraudulent (0)**

Key focus areas include:
- Handling imbalanced data.
- Enhancing model performance through feature engineering.
- Building interpretable and accurate ML models.

---

## 📊 Dataset Overview

| **Property**           | **Details**                        |
|------------------------|------------------------------------|
| **Rows & Columns**     | 1,000 rows, 7 columns             |
| **Key Features**       | `Transaction Amount`, `Risk Score`, `Merchant Category`, `Customer Age Group`, `Payment Method`, `Transaction Time` |
| **Target Variable**    | `Fraudulent`: 1 (fraud), 0 (genuine) |
| **Imbalance**          | Majority class: Non-Fraudulent (~700) |

---

## ⚙️ Workflow

1. **Exploratory Data Analysis (EDA)**:
   - Detected and removed **99 outliers** using the **IQR method**.
   - Verified no missing values or duplicate rows.
   - Visualized class distribution to address imbalance.

2. **Data Preprocessing**:
   - **Categorical Encoding**: Label Encoding for categorical features.
   - **Data Balancing**: Applied **SMOTE** to handle class imbalance.
   - **Feature Scaling**: Standardized numerical features using `StandardScaler`.

3. **Model Building**:
   - Split dataset into **Training (70%)** and **Testing (30%)** sets.
   - Implemented **Logistic Regression** and **KNN**.

4. **Evaluation Metrics**:
   - Used **Accuracy**, **Precision**, **Recall**, **F1-Score**, and **Confusion Matrix**.

---

## 📈 Results

| **Model**              | **Accuracy** | **F1-Score** | **Fraud Recall** | **Fraud Precision** |
|------------------------|--------------|--------------|------------------|---------------------|
| Logistic Regression    | 63%          | 0.65         | 70%              | 61%                 |
| K-Nearest Neighbors    | 68%          | 0.71         | 80%              | 64%                 |

### Key Insights:
- **KNN** achieved higher **recall (80%)** for fraudulent transactions, reducing false negatives.
- **Logistic Regression** provided interpretable results but underperformed in comparison.

---

## 📌 Conclusion

Based on the evaluation:
- **KNN** is the preferred model for fraud detection, with superior performance in detecting fraudulent transactions.
- **Logistic Regression**, while interpretable, struggled to balance precision and recall effectively.

---

## 🛠 Future Work

1. **Model Optimization**:
   - Hyperparameter tuning for KNN.
   - Experiment with advanced algorithms like Random Forest and Gradient Boosting.

2. **Advanced Metrics**:
   - Evaluate models using **ROC-AUC** for better discrimination analysis.

3. **Scalability**:
   - Apply models to larger datasets for real-world validation.

---

## 🧰 Tools & Technologies

- **Python**: NumPy, Pandas, Scikit-learn, Matplotlib, Seaborn.
- **ML Techniques**: Logistic Regression, KNN, SMOTE.

---
