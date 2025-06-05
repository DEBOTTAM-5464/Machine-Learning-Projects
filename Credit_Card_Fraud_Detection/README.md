# 💳 Credit Card Fraud Detection (Downsampled)

This project applies multiple machine learning classifiers to detect **fraudulent credit card transactions** using a downsampled version of the highly imbalanced dataset.

---

## 📁 Dataset Overview

- Source: `creditcard.csv`
- Original: 284,807 transactions (492 frauds)
- **Downsampled**:  
  - 200 fraud cases  
  - 9,800 legitimate cases  
  - Total: **10,000** (balanced for training stability)

---

## 🧪 Workflow

### ✅ 1. Data Preprocessing
- Downsampled fraud and legitimate cases
- Combined and shuffled
- Scaled **Time** and **Amount** features using `StandardScaler`

### ✅ 2. Target Variable
- `Class`:  
  - `1` → Fraud  
  - `0` → Legit

---

## 🧠 Models Used

- **Logistic Regression**
- **Random Forest**
- **Decision Tree**
- **Support Vector Machine (SVM)**
- **K-Nearest Neighbors (KNN)**

Each model was trained and evaluated on the downsampled, stratified data.

---

## 📊 Evaluation Metrics

For each model:
- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **ROC AUC**
- **ROC Curve Plot**
- **Confusion Matrix** (optional to visualize)

---

## 📌 Output

- Console summary of performance for each model
- ROC curves for visual model comparison

---

## 🛠️ Libraries Used

- `pandas`, `matplotlib`, `seaborn`
- `scikit-learn` (`train_test_split`, models, metrics, preprocessing)

---

## 🔍 Note

This project demonstrates model performance in **balanced scenarios** using downsampling. Real-world deployment should involve **more advanced imbalance handling techniques** (e.g., SMOTE, anomaly detection, cost-sensitive learning).

