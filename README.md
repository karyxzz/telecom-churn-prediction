# 📊 Customer Churn Prediction using ANN

This project focuses on predicting customer churn in a telecom company using an Artificial Neural Network (ANN) built with TensorFlow and Keras. The goal is to identify customers who are likely to stop using the service.

---

## 🧠 Project Overview

- **Objective**: Predict whether a customer will churn (i.e., leave the company).
- **Method**: Use ANN for classification.
- **Toolkits**: Python, TensorFlow, Keras, Pandas, Matplotlib.

---

## 📁 Dataset Description

- The dataset includes customer demographics, account information, and service usage.
- **Features** include: `gender`, `SeniorCitizen`, `Partner`, `Dependents`, `tenure`, `PhoneService`, `InternetService`, etc.
- **Target**: `Churn` (Yes/No)

---

## 🔧 Data Preprocessing

- Dropped irrelevant columns like `customerID`.
- Removed rows with blank `TotalCharges`.
- Replaced "No internet service" and "No phone service" with "No".
- Converted `Yes/No` values to binary (1/0).
- Applied one-hot encoding for categorical columns.
- Performed a train-test split.

---

## 🧮 Model Architecture

- **Input Layer**: 26 features
- **Hidden Layers**:

  - Dense(26, activation='relu')
  - Dense(15, activation='relu')

- **Output Layer**:

  - Dense(1, activation='sigmoid')

- **Loss Function**: Binary Crossentropy
- **Optimizer**: Adam
- **Epochs**: 100

---

## 📈 Evaluation Metrics

- **Accuracy**: Achieved high accuracy on test data.
- **Precision** (Class 0): Indicates how many predicted non-churn customers actually stayed.
- **Precision** (Class 1): Indicates how many predicted churners actually churned.
- **Recall** and **F1-Score** were also evaluated.

---

## 📦 Dependencies

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `tensorflow` / `keras`

You can install all dependencies using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow
```

---

## ✨ Conclusion

The ANN-based approach achieved good performance in classifying customer churn. With proper preprocessing and tuning, it can be a valuable tool for telecom companies to retain customers proactively.

---
