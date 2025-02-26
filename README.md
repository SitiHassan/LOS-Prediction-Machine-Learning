# LOS-Prediction-Machine-Learning

## Introduction
This project aims to predict the **Length of Stay (LOS)** among patients admitted to hospitals in England. The focus is on emergency admissions through **213 Accident and Emergency (A&E) departments** between **March 23, 2014, and March 22, 2018**, using a **synthetic dataset**. This project serves as a proof-of-concept for utilizing **synthetic data** for **LOS prediction**, exploring how machine learning can improve **resource allocation** and **timely discharges**.

The NHS defines a **"Long Stay"** as **21 days or more**. The dataset includes:
- **Short Stay** cases: **11,998,058** (94.32%)
- **Long Stay** cases: **724,158** (5.68%)

## Methodology
### **Machine Learning Algorithms**
**Four machine learning algorithms** were applied to classify LOS as **Short Stay vs. Long Stay**:
- **Logistic Regression**
- **Decision Tree**
- **Gradient Boosting**
- **Random Forest**

### **Data Handling & Preprocessing**
The dataset was highly **imbalanced**, so **three resampling techniques** were applied:
- **SMOTE (Synthetic Minority Over-sampling Technique)**
- **Hybrid SMOTE-Tomek**
- **Random Undersampling**

### **Feature Engineering & Selection**
**Feature selection and engineering** were performed using **Recursive Feature Elimination with Cross-Validation (RFECV)** to identify the most relevant predictors for LOS.

## Results

- **XGBoost outperformed all models**, particularly in **Precision**, which is crucial for minimizing misclassification.
- **21 key predictors** were identified, covering **socio-demographic** and **healthcare resource factors**.
