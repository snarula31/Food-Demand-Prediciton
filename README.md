# 🍽️ Food Demand Forecasting using Machine Learning

## 📌 Project Overview

This project aims to accurately forecast food demand for a meal delivery service by leveraging historical data and machine learning techniques. Predicting food demand is essential to optimize inventory, reduce food wastage, and streamline supply chain operations.

---

## 🧠 Problem Statement

Meal delivery services often face challenges in demand forecasting due to fluctuating customer behavior and seasonal trends. The objective of this project is to build a robust machine learning model that can predict the number of meals required for a given center, meal type, and week.

---

# Data Dictionary

The dataset consists of three individual datasheets, the first dataset contains the historical demand data for all centers, the second dataset contains the information of each fulfillment center and the third dataset contains the meal information.

Weekly Demand data (train.csv): \
Contains the historical demand data for all centers. The Train dataset consists of 9 variables and records of 423727 unique orders. test.csv contains all the following features except the target variable. The Test dataset consists of 8 variables and records of 32573 unique orders.

| Variable  | Definition |
| ------------- | ------------- |
| id 	| Unique ID |
| week 	| Week No |
| center_id | Unique ID for fulfillment center |
| meal_id | Unique ID for Meal |
| checkout_price | Final price including discount, taxes & delivery charges |
| base_price | Base price of the meal |
| emailer_for_promotion | Emailer sent for promotion of meal |
| homepage_featured | Meal featured at homepage |
| num_orders | (Target) Orders Count |

\
fulfilment_center_info.csv: \
Contains information for each fulfilment center. The dataset consists of 5 variables and records of 77 unique fulfillment centers. 

| Variable  | Definition |
| ------------- | ------------- |
| center_id |	Unique ID for fulfillment center |
| city_code |	Unique code for city |
| region_code |	Unique code for region |
| center_type |	Anonymized center type |
| op_area |	Area of operation (in km^2) |

\
meal_info.csv: \
Contains information for each meal being served 

| Variable  | Definition |
| ------------- | ------------- |
| meal_id |	Unique ID for the meal |
| category |	Type of meal (beverages/snacks/soups….) |
| cuisine |	Meal cuisine (Indian/Italian/…) |

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

