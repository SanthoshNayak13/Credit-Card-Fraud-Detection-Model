# 💳 Credit Card Fraud Detection Model

A machine learning project for detecting fraudulent credit card transactions using **Python**, **Scikit-learn**, **Random Forest**, and **SMOTE**.


## 📌 Overview

This project implements a **Credit Card Fraud Detection Model** using a **Random Forest Classifier**. The model is trained to distinguish between legitimate and fraudulent credit card transactions.

The project uses the **Credit Card Fraud Detection dataset** from Kaggle, which contains **284,315 transactions**, including **492 fraudulent transactions (0.17%)**.

Because fraudulent transactions are significantly less frequent than legitimate transactions, **Synthetic Minority Over-sampling Technique (SMOTE)** is used to address the class imbalance during model training.

## 📊 Dataset

The dataset is sourced from Kaggle:

**Dataset:** [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

The dataset contains:

- **284,315 transactions**
- **492 fraudulent transactions**
- **0.17% fraudulent transactions**
- Features `V1`–`V28`
- `Amount`
- `Time`
- `Class` — target variable (`0` = legitimate, `1` = fraud)

> **Note:** Features `V1`–`V28` are PCA-transformed features to protect sensitive information.

## 🤖 Model

The project uses a **Random Forest Classifier**, a supervised machine learning algorithm based on an ensemble of decision trees.

### Technologies Used

- Python
- Scikit-learn
- Random Forest Classifier
- SMOTE
- Pandas
- NumPy
- Streamlit

## 📈 Model Performance

The model achieved the following results on the test dataset:

| Metric | Score |
|---|---:|
| Accuracy | **99.98%** |
| Precision | **99.97%** |
| Recall | **100%** |

> **Note:** Accuracy can be misleading for highly imbalanced datasets. Precision and recall are therefore particularly important for fraud detection.

## 🚀 Deployment

The model is deployed using **Streamlit**.

Users can enter the required transaction features, including:

- `V1`–`V28`
- Normalized transaction `Amount`

The application predicts whether the transaction is:

- ✅ **Legitimate**
- 🚨 **Fraudulent**

## 🖥️ Run the Project Locally

### 1. Clone the repository

```bash
git clone https://github.com/SanthoshNayak13/Credit-Card-Fraud-Detection-Model.git
cd Credit-Card-Fraud-Detection-Model
