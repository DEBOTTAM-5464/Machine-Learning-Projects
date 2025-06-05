# 🚗 Car Price Category Classification

This project predicts whether a car's selling price is **High (≥ median)** or **Low (< median)** using machine learning classifiers. It uses features like car age, fuel type, transmission, and seller type to train multiple models and evaluate performance.

---

## 📁 Dataset

- Input CSV: `car data.csv`
- Key features:  
  - **Present_Price**, **Kms_Driven**, **Fuel_Type**, **Transmission**, **Owner**, etc.

---

## 🧪 Workflow

### ✅ 1. Data Preprocessing
- Extract **Car Age** from `Year`
- Drop `Car_Name` and `Year`
- Encode categorical features: `Fuel_Type`, `Selling_type`, `Transmission` using `LabelEncoder`

### ✅ 2. Target Variable
- Target: `Price_Category`  
  - 1 → Selling Price ≥ Median  
  - 0 → Selling Price < Median

### ✅ 3. Split and Scale
- 80-20 train-test split
- Apply **StandardScaler** for feature normalization

---

## 🤖 Models Used

- **Logistic Regression**
- **Random Forest**
- **Support Vector Machine (SVM)**
- **Decision Tree**
- **K-Nearest Neighbors (KNN)**
- **XGBoost**

Each model is trained and evaluated using key metrics.

---

## 📊 Evaluation Metrics

For each model:
- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **AUC (ROC)**
- **Confusion Matrix**
- **ROC Curve**

---

## 📌 Output

- Summary table showing metric scores for all models
- ROC curve plots for each model

---

## 🛠️ Libraries Used

- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `sklearn`: model selection, preprocessing, metrics
- `xgboost` for gradient boosting

