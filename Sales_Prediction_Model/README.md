# 📊 Advertising Sales Classification (Binary)

This project applies multiple machine learning classifiers to predict whether advertising campaigns lead to **High Sales** or **Low Sales** based on advertising budget features from TV, Radio, and Newspaper.

---

## 📁 Dataset Overview

- Source: `Advertising.csv`  
- Features:  
  - `TV`, `Radio`, `Newspaper` (advertising budgets)  
- Target (binarized):  
  - `HighSales` — 1 if sales are at or above median sales, 0 otherwise

---

## 🧪 Workflow

### ✅ 1. Data Preprocessing
- Converted continuous sales to binary target using median split  
- Split data into 80% train, 20% test  
- Standardized features with `StandardScaler`

### ✅ 2. Models Used
- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Support Vector Machine (SVM)  
- Decision Tree  
- Random Forest  
- Gradient Boosting  
- XGBoost  
- Naive Bayes  

All models were trained on standardized training data and tested on standardized test data.

---

## 📊 Evaluation Metrics

For each model, the following metrics were calculated:  
- Accuracy  
- Precision  
- Recall  
- F1 Score  
- ROC AUC  
- ROC Curve plotted for visual comparison  
- Confusion Matrix visualized with heatmaps

---

## 📌 Output

- Printed classification metrics for all models in the console  
- ROC curves for each classifier plotted in a grid  
- Confusion matrices plotted in a grid for easy comparison

---

## 🛠️ Libraries Used

- `pandas`, `numpy` for data handling  
- `scikit-learn` for modeling, preprocessing, and evaluation  
- `xgboost` for gradient boosted trees  
- `matplotlib`, `seaborn` for visualization

---
