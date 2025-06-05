# 💼 Customer Churn Prediction

This project predicts whether a customer will **churn (exit)** using various machine learning models. It uses the `Churn_Modelling.csv` dataset and evaluates model performance through key metrics and ROC curves.

---

## 🔧 Steps Overview

### ✅ 1. Import Libraries
Includes `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`, and `xgboost`.

### ✅ 2. Load & Clean Data
- Load CSV
- Drop unnecessary columns: `RowNumber`, `CustomerId`, `Surname`

### ✅ 3. Encode Categorical Data
- Encode `Geography` and `Gender` using `LabelEncoder`.

### ✅ 4. Split Data
- Features (`X`) and target (`y = Exited`)
- Train-test split (80/20 with stratification)

### ✅ 5. Scale Features
- Apply `StandardScaler` to normalize feature values.

### ✅ 6. Define Evaluation Function
- Metrics: Accuracy, Precision, Recall, F1, AUC
- Confusion Matrix & ROC Curve plotting

### ✅ 7. Train & Evaluate Models
Models used:
- Logistic Regression  
- Random Forest  
- Gradient Boosting  
- Support Vector Machine  
- K-Nearest Neighbors  
- Decision Tree  
- Naive Bayes  
- XGBoost

Each model is trained and evaluated using the custom function.

---

## 📊 Output
For each model:
- Performance metrics printed
- ROC Curve plotted

---

## ✅ Goal
Compare models and identify the best performer for churn prediction based on metrics like F1-score and AUC.


