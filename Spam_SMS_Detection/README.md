# 📧 Spam Email Classification

This project implements multiple machine learning classifiers to detect **spam emails** from text data using the classic SMS Spam Collection Dataset. The goal is to classify messages as **spam** or **ham (non-spam)** with high accuracy.

---

## 🗂 Dataset

- Source: SMS Spam Collection Dataset (commonly named `spam.csv`)
- Columns:
  - `text`: The email/SMS message content
  - `label`: Target variable, with values:
    - `0` for ham (non-spam)
    - `1` for spam

---

## ⚙️ Workflow

### 1. Data Preparation
- Load dataset and keep only relevant columns
- Map textual labels to binary labels (`ham` → 0, `spam` → 1)

### 2. Train-Test Split
- Split data into 80% training and 20% testing subsets with stratification on label to maintain class balance

### 3. Feature Extraction
- Convert text messages into numerical features using **TF-IDF Vectorization**
- Stop words removal and max document frequency filtering (`max_df=0.9`) applied

### 4. Model Training & Evaluation
- Train multiple classifiers:
  - Naive Bayes (MultinomialNB)
  - Logistic Regression
  - Support Vector Machine (LinearSVC)
  - Random Forest
  - Decision Tree
  - Gradient Boosting
  - K-Nearest Neighbors
  - XGBoost
- Evaluate using:
  - Accuracy
  - Classification Report (Precision, Recall, F1-Score)
  - Confusion Matrix visualization
  - ROC Curve with AUC score

---

## 📊 Results

- Confusion matrices and ROC curves are plotted for each model to visually assess performance
- Models are compared on standard classification metrics printed on the console

---

## 🛠️ Libraries & Tools

- `pandas` for data handling
- `scikit-learn` for ML models and evaluation
- `xgboost` for gradient boosted trees
- `matplotlib` & `seaborn` for plotting and visualization

---

## 🚀 How to Run

1. Ensure the dataset `spam.csv` is available in your working directory
2. Install required Python packages:
   ```bash
   pip install pandas scikit-learn xgboost matplotlib seaborn

