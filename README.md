# Spam-Email-Classification
Machine learning-based solution to classify emails

This project presents a machine learning-based solution to **classify emails as spam or non-spam** using **Logistic Regression** and **Random Forest** classifiers. It aims to enhance email productivity and security by filtering unwanted emails with high precision and recall.

---

## 🧠 Problem Statement

> With the exponential rise of unsolicited emails (spam), this project seeks to build a classification system to automatically distinguish between spam and non-spam emails. By leveraging word frequency patterns and supervised learning algorithms, we aim to reduce noise in email systems and improve focus on relevant communication.

---

## 📊 Dataset Description

- **Source**: [Kaggle Spam Email Dataset](https://www.kaggle.com/)
- **Size**: 5,172 email samples
- **Features**:
  - Frequency count of **3,000 most common words** per email
  - Final column: `Prediction` (Target variable)
    - `1` → Spam  
    - `0` → Not Spam

---

## ⚙️ Methodology

### 🔍 Data Cleaning
- Removed missing or irrelevant values
- Normalized the word frequency features

### 🧪 Feature Engineering
- Selected **top 3,000 most frequent words**
- Removed non-informative and low-variance features

### 📈 Data Visualization
- Bar chart showing **spam vs non-spam distribution**
- Histograms of **word frequencies in spam/non-spam** categories

---

## 🤖 Models Used

### 1. Logistic Regression
- Simple and interpretable model
- Fast training and suitable for real-time prediction

### 2. Random Forest Classifier
- Ensemble of decision trees
- Handles complex patterns and word interactions better

---

## 🧮 Evaluation Metrics

| Metric     | Description                                          |
|------------|------------------------------------------------------|
| Accuracy   | Overall prediction correctness                      |
| Precision  | Proportion of predicted spam that are actually spam |
| Recall     | Proportion of actual spam that were identified      |
| F1 Score   | Harmonic mean of precision and recall               |

### 📊 ROC Curve
Visualizes the **True Positive Rate vs False Positive Rate** across thresholds.

---

## 📌 Observations

- **Random Forest** outperformed Logistic Regression:
  - Accuracy ~ **97%**
  - Better balance between **precision** and **recall**
- Logistic Regression was faster but slightly less accurate

---

## 🚀 Next Steps

- Use **word embeddings** (e.g., Word2Vec, TF-IDF, BERT) to better capture context
- Explore advanced algorithms like **SVMs**, **XGBoost**, or **Deep Learning**
- Apply **cross-validation** to ensure generalization
- Expand dataset size and diversity

---
