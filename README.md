# 🔋 Battery Cathode Performance Prediction Using Machine Learning

This project uses regression models to predict the **specific discharge capacity** and **capacity retention** of battery cathode materials based on their physical and chemical properties. It includes a complete pipeline from data preprocessing and exploratory data analysis to model training, evaluation, and saving.

---

## 📌 Problem Statement

**Objective:**  
To build a regression model that predicts how well a cathode material performs in terms of:
- 🔋 Specific Discharge Capacity (mAh g⁻¹)
- ♻️ Capacity Retention after 50 cycles (%)

These predictions are based on various material properties such as:
- Atomic Radius
- Electronegativity
- Thermal Conductivity
- Fusion Heat

---

## 📁 Dataset

- CSV file containing physical and chemical properties of cathode materials.
- Columns include:
  - Average Atomic Radius
  - Average Electronegativity
  - Thermal Conductivity
  - Fusion Heat
  - Specific Discharge Capacity (target)
  - Capacity Retention (target)

---

## 🧠 ML Pipeline

1. **Data Preprocessing**
   - Dropping unnecessary columns
   - Handling missing values
   - Feature scaling using `StandardScaler`

2. **Exploratory Data Analysis (EDA)**
   - Boxplots to detect outliers
   - Pairplots to understand feature relationships
   - Correlation heatmap

3. **Modeling**
   - Train-test split
   - Linear Regression (can also test Random Forest)
   - Evaluation using:
     - MAE (Mean Absolute Error)
     - RMSE (Root Mean Squared Error)
     - R² Score

4. **Model Saving**
   - Trained model and scaler saved using `pickle`

---

## 🛠️ Requirements

- Python ≥ 3.8
- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn
- pickle
