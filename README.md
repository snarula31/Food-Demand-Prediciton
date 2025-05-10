# 🍽️ Food Demand Forecasting using Machine Learning

## 📌 Project Overview

This project aims to accurately forecast food demand for a meal delivery service by leveraging historical data and machine learning techniques. Predicting food demand is essential to optimize inventory, reduce food wastage, and streamline supply chain operations.

---

## 🧠 Problem Statement

Meal delivery services often face challenges in demand forecasting due to fluctuating customer behavior and seasonal trends. The objective of this project is to build a robust machine learning model that can predict the number of meals required for a given center, meal type, and week.

---

## 📂 Dataset Description

The dataset includes the following files:
- `train.csv` – Historical demand data
- `test.csv` – Data for prediction
- `meal_info.csv` – Meal category and cuisine details
- `fulfilment_center_info.csv` – Information about meal distribution centers

Key columns:
- `center_id`, `meal_id`, `week`
- `checkout_price`, `base_price`
- `emailer_for_promotion`, `homepage_featured`
- `num_orders` (target variable)

---

## 🔧 Tools & Technologies Used

- **Python**
  - `pandas`, `numpy` – Data preprocessing and manipulation
  - `matplotlib`, `seaborn` – Data visualization
  - `scikit-learn` – ML models and evaluation
  - `xgboost`, `randomforest` – Advanced regression models

---

## 📊 Exploratory Data Analysis

- Distribution of orders across weeks
- Meal and center-level trends
- Impact of promotional features
- Price sensitivity analysis

---

## 🛠️ Feature Engineering

- Merged datasets to enhance feature space
- Created interaction terms (e.g., `center_meal_combo`)
- Handled skewness and missing values
- Encoded categorical variables

---

## 🤖 Model Building

Tested multiple regression models:
- Linear Regression
- Random Forest Regressor
- XGBoost Regressor

**Evaluation Metric**: RMSE (Root Mean Squared Error)

Selected the model with the lowest RMSE on validation data.

---

## ✅ Results

- Final model: **XGBoost Regressor**
- Achieved significantly lower RMSE compared to baseline
- Insights generated to improve promotional strategies and pricing

---

## 📁 Project Structure

