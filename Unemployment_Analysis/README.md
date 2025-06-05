# 📉 Unemployment Rate Prediction

This project predicts **Unemployment Rate** based on historical employment data using various regression models. The dataset combines multiple features like employment numbers, labor participation rates, region, and date to build predictive models.

---

## 🗂 Dataset Overview

- **File**: `merged_unemployment_data.csv`
- **Selected Features**:
  - `Region`
  - `Date`
  - `Unemployment Rate (File1)` *(Target variable)*
  - `Employed (File1)`
  - `Labour Participation Rate (File1)`

---

## ⚙️ Workflow

### ✅ 1. Data Cleaning & Feature Engineering
- Dropped missing values (`NaN`)
- Converted `Date` column into **Month** and **Year**
- Encoded `Region` column numerically using `LabelEncoder`

### ✅ 2. Feature Set
- **Input Features (`X`)**:
  - Region (encoded)
  - Month
  - Year
  - Employed (File1)
  - Labour Participation Rate (File1)
- **Target (`y`)**:
  - Unemployment Rate (File1)

### ✅ 3. Train-Test Split
- 80% training data
- 20% testing data
- Random seed set to `42` for reproducibility

---

## 🤖 Regression Models Used

- **Linear Regression**
- **Decision Tree Regressor**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**
- **Support Vector Regressor (SVR)**
- **K-Nearest Neighbors Regressor (KNN)**

Each model is trained and evaluated using the same dataset split for consistency.

---

## 📊 Evaluation Metrics

Each model is evaluated based on:
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score**

Results are printed in the console for comparison across models.

---

## 🛠️ Technologies & Libraries

- `pandas`, `numpy`
- `scikit-learn` (models, metrics, preprocessing)
- Dataset: CSV format

---

## 🚀 How to Run

1. Place `merged_unemployment_data.csv` in your working directory.
2. Install required libraries if not already available:
   ```bash
   pip install pandas numpy scikit-learn

