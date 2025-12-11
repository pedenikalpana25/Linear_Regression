# 🚗 Cars24 Car Price Prediction using Linear Regression

This project predicts the **selling price of used cars** using Linear Regression on the Cars24 dataset.  
The goal is to understand how car features such as engine size, mileage, max power, fuel type, and age affect the selling price.

---

## 📁 Project Contents

- **Cars24_LinearRegression.ipynb** – Main Jupyter Notebook with:
  - Data cleaning
  - EDA (exploratory data analysis)
  - Feature engineering
  - Model building (Linear Regression)
  - Performance evaluation

- **README.md** – Project documentation

---

## 📌 Problem Statement

This project predicts car selling prices using Cars24 dataset features such as:
- full_name (car make + model)
- year (manufacturing year)
- seller_type (Dealer / Individual)
- km_driven (total distance driven)
- fuel_type (Petrol, Diesel, CNG, etc.)
- transmission_type (Manual / Automatic)
- mileage
- engine (engine capacity in CC)
- max_power
- seats

Using these features, a Linear Regression model is built to accurately estimate the selling price of used cars.

---

## 🧹 Data Preprocessing Steps

- Removed unnecessary symbols from `engine` and `max_power`
- Converted them to numeric
- Extracted:
  - `make`
  - `model`
  - `age` from the year column
- One-Hot Encoding for:
  - fuel_type  
  - seller_type  
  - transmission_type  
  - seats  
- Removed unrealistic values (like mileage = 0)
- Treated outliers with percentile capping

---

## 📊 Exploratory Data Analysis

Visualizations included:
- Histogram of selling price
- Boxplots for:
  - fuel type vs price
  - seller type vs price
  - seats vs price
- Correlation heatmap
- Pairplot for selected numerical features

Insights:
- Diesel and Electric cars have higher median prices  
- Dealers sell at higher prices than individuals  
- Newer cars have higher selling prices  
- Max power and engine strongly correlate with price  

---

## 🤖 Model Used – Linear Regression
Train-Test Split:
Train: 80%
Test: 20%


Metrics evaluated:
- R² Score  
- MAE (Mean Absolute Error)  
- RMSE (Root Mean Square Error)

Model is interpretable and shows how each feature contributes to price.



---

## 📦 Tech Stack
-Jupyter Notebook
- Python  
- Pandas  
- NumPy  
- Seaborn  
- Matplotlib  
- Scikit-Learn  

---

## 📬 Author

**Pedeni Kalpana**  
Aspiring Data Analyst  
Email: **kalpanapedeni2000@gmail.com**  
LinkedIn: **linkedin.com/in/pedeni-kalpana**



