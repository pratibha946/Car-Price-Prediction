# 🚗 Car Price Prediction Using Machine Learning

This project aims to predict the price of cars based on various features using different machine learning models. It provides a structured workflow from data exploration to model evaluation and highlights key automotive pricing trends.

---

## 📌 Project Objective

To build and evaluate machine learning models that can predict the price of a car using numerical and categorical attributes. The models are designed to assist dealerships, buyers, and sellers in understanding car value objectively.

---

## 🗃️ Dataset Summary

- **Source**: UCI Machine Learning Repository
- **Records**: ~200
- **Target Variable**: `price`
- **Features Used**:
  - Numerical: `engine-size`, `horsepower`, `curb-weight`, `highway-mpg`, `city-mpg`, `wheel-base`, etc.
  - Categorical: `body-style`, `drive-wheels`, `engine-location`, etc.

---

## 🔍 Exploratory Data Analysis

- **Data Cleaning**: Missing values handled appropriately
- **Visualizations**:
  - Regression and box plots to show relationships
  - Correlation heatmaps
  - Pivot tables to explore group-wise pricing
- **Insights**:
  - `engine-size` shows strong positive correlation with price
  - Rear-engine cars tend to be more expensive
  - Drive wheels and body styles moderately influence pricing

---

## 🧠 Machine Learning Models

### ✅ Simple Linear Regression
- Examined individual feature impact (`engine-size`, `highway-mpg`).

### ✅ Multiple Linear Regression
- Used multiple predictors for improved accuracy:
  `horsepower`, `curb-weight`, `engine-size`, `highway-mpg`.

### ✅ Polynomial Regression
- Captured non-linear relationships between features and price.
- Demonstrated with features like `engine-size`.

### ✅ Pipelines
- Built using `Pipeline` from `sklearn`:
  - Preprocessing with `StandardScaler`
  - Model chaining
  - Clean and modular ML workflow

---

## 📊 Model Evaluation

- **Metrics**:
  - R² (Coefficient of Determination)
  - Mean Squared Error (MSE)
- **Results**:
  - Polynomial regression performed better for non-linear features
  - High correlation observed with `engine-size`, `curb-weight`, `horsepower`

---

## 🚀 Future Enhancements

- Add more variables (e.g., brand, model year, fuel type)
- Test advanced models: Random Forest, XGBoost
- Use GridSearchCV for hyperparameter tuning
- Deploy model using Flask or Streamlit for real-time predictions

---

## 🛠️ Tech Stack

- **Language**: Python
- **Libraries**: pandas, matplotlib, seaborn, sklearn, numpy, scipy
- **Tool**: Jupyter Notebook

