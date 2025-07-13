# 🏠 House Price Prediction using Machine Learning

This project aims to build a machine learning model that predicts **house prices** using the **California Housing dataset**. It walks through a complete end-to-end pipeline from loading data to training a model and evaluating its performance.

---

## 🔍 Problem Statement

Predict **house prices** in different districts of California based on various features like income, number of rooms, location, etc.

---

## 🧠 Type of Machine Learning Used

- **Category:** 🧠 **Supervised Learning**
- **Type:** 📈 **Regression**
- **Model Used:** 🔹 `Linear Regression` (from `scikit-learn`)

---

## 📊 Dataset: California Housing Dataset

This dataset contains information collected from the 1990 California census, including:

- Income
- Average rooms per household
- Population
- Location (latitude, longitude)
- ... and other features

The target variable is:
- `PRICE`: Value of houses in a block (in $100,000s)

---

## 🔁 Step-by-Step Workflow

### 1. **Import Libraries**
- `NumPy`, `Pandas` for data manipulation
- `Seaborn`, `Matplotlib` for visualization
- `Scikit-learn` for ML algorithms

### 2. **Load and Prepare Data**
- Used `fetch_california_housing()` to get the dataset
- Converted it into a Pandas DataFrame
- Added the target column: `TargetPrice`

### 3. **Data Analysis**
- Checked for missing values
- Generated a correlation heatmap to understand feature relationships

### 4. **Data Splitting**
- Features and target split into:
  - `X` (independent variables)
  - `y` (target: house price)
- Used `train_test_split` (80% training, 20% testing)

### 5. **Model Training**
- Trained a **Linear Regression model** on the training data

### 6. **Model Evaluation**
- Predicted prices on the test set
- Evaluated using:
  - ✅ `R² Score` (Coefficient of Determination)
  - ✅ `Mean Squared Error (MSE)`

**📌 R² Score Obtained:** `0.622`  
This is a good score and falls within the **expected range of 0.50 – 0.75** for Linear Regression on this dataset.

### 7. **Visualization**
- Plotted a **scatter plot** of **actual vs predicted prices**
- Included a red reference line for perfect prediction

---

## 📈 Output Graph (Actual vs Predicted Prices)

The following graph shows how close the model's predictions were to actual house prices:

![Actual vs Predicted Plot]  


## ✅ Conclusion

- Successfully built and evaluated a regression model for predicting house prices.
- Model shows decent performance (R² = 0.622) using a basic Linear Regression algorithm.
- The project can be improved further by using more advanced models like Random Forest or XGBoost.

---

## 📁 Project Files

| File | Description |
|------|-------------|
| `House_Price_Prediction.ipynb` | Main notebook with code |
| `README.md` | Project documentation |

---
