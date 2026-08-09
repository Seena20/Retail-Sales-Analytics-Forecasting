# Retail Sales Analytics and AI-Powered Sales Forecasting

## 📊 Project Overview

Retail businesses generate large amounts of sales data every day. Analyzing this data helps businesses understand sales performance, customer behavior, product performance, regional trends, and future demand.

This project analyzes historical retail sales data from January 2023 to December 2024 and develops a Machine Learning based sales forecasting system.

The project combines Exploratory Data Analysis (EDA), business analytics, feature engineering, Machine Learning, and future sales forecasting.

---

## 🎯 Objectives

The main objectives of this project are:

- Analyze historical retail sales data.
- Perform data cleaning and quality checks.
- Identify important sales trends and patterns.
- Analyze product category and brand performance.
- Compare regional and store-level sales.
- Analyze new and returning customer behavior.
- Analyze payment modes, promotions, and holiday sales.
- Perform time-series analysis.
- Create Machine Learning features for sales forecasting.
- Train and compare multiple Machine Learning models.
- Select the best-performing forecasting model.
- Forecast sales for the next 30 days.

---

## 📂 Dataset

The dataset is stored in Excel format and contains retail sales information from:

**January 1, 2023 to December 31, 2024**

### Dataset Statistics

| Metric | Value |
|---|---:|
| Data Period | 2023–2024 |
| Number of Days | 731 |
| Missing Values | 0 |
| Duplicate Rows | 0 |
| Total Sales | ₹45.71 Billion |
| Total Revenue | ₹41.13 Billion |
| Total Units Sold | 1,817,305 |

### Dataset Features

The dataset contains the following important features:

- Date
- Store_ID
- Store_Location
- Product_ID
- Product_Category
- Product_Subcategory
- Brand
- Unit_Price
- Units_Sold
- Total_Sales
- Discount_Percentage
- Revenue
- Customer_Type
- Payment_Mode
- Promotion_Applied
- Stock_On_Hand
- Store_Rating
- Region
- Holiday_Flag

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Excel
- Google Colab

---

## 🔍 Exploratory Data Analysis

The following business areas were analyzed:

### Product Category Analysis

Electronics was identified as the highest-performing product category based on sales and revenue.

### Regional Analysis

The West region recorded the highest Total Sales.

### Store Analysis

Store `STR_103` was the highest-performing store based on Total Sales.

### Brand Analysis

Levis was the top-performing brand based on Total Sales.

### Customer Analysis

Returning customers generated approximately ₹27.39 Billion in Total Sales, significantly higher than new customers.

### Payment Mode Analysis

Sales were compared across Credit Card, Cash, Debit Card, and UPI.

### Holiday Analysis

Holiday sales contributed approximately 1.20% of total sales.

### Promotion Analysis

Sales, units sold, and discount percentages were compared between promotional and non-promotional transactions.

---

## 📈 Time-Series Analysis

Transaction-level sales were aggregated into daily sales values.

The resulting time series contains:

- 731 days of historical sales data
- 641 days for training
- 90 days for testing

---

## ⚙️ Feature Engineering

The following features were created for Machine Learning:

- Day
- Month
- Year
- DayOfWeek
- Lag_1
- Lag_7
- Lag_30
- Rolling_7
- Rolling_30

### Feature Importance

The Random Forest model showed that recent sales trends were highly important.

The most important feature was:

**Rolling_7 — 25.56%**

This indicates that recent 7-day sales behavior provides an important signal for forecasting.

---

## 🤖 Machine Learning Models

Three models were evaluated:

1. Random Forest Regressor
2. Gradient Boosting Regressor
3. Improved Gradient Boosting Regressor

---

## 📊 Model Evaluation

The models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### Model Comparison

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Random Forest | 5.521M | 6.647M | 0.035 |
| Gradient Boosting | 5.417M | 6.583M | 0.054 |
| Improved Gradient Boosting | 5.710M | 6.697M | 0.020 |

### Best Model

**Gradient Boosting Regressor**

Gradient Boosting achieved the lowest MAE and RMSE and the highest R² score among the evaluated models.

Therefore, Gradient Boosting was selected as the final forecasting model.

---

## 🔮 30-Day Sales Forecast

The selected Gradient Boosting model was used to forecast sales for:

**January 1, 2025 to January 30, 2025**

### Forecast Summary

- Forecast Period: 30 Days
- Total Forecasted Sales: Approximately ₹178.82 Crore
- Average Daily Forecast: Approximately ₹5.96 Crore
- Highest Forecasted Daily Sales: Approximately ₹6.25 Crore

---

## 📊 Key Business Insights

- Electronics was the highest-performing product category.
- West was the highest-performing region.
- STR_103 was the top-performing store.
- Levis was the top-performing brand.
- Returning customers contributed significantly higher sales.
- Holiday sales represented approximately 1.20% of total sales.
- Recent 7-day sales trends were highly important for forecasting.
- Gradient Boosting performed better than the other evaluated models.
- The final model was used to forecast the next 30 days of sales.

---

## 📁 Project Structure

```text
Retail-Sales-Analytics-Forecasting/
│
├── README.md
├── Retail_Sales_Analytics_Forecasting.ipynb
├── 4877028-Retail_Sales_Data (1).xlsx
├── requirements.txt
│
└── screenshots/
    ├── dashboard.png
    ├── monthly_sales.png
    ├── category_analysis.png
    ├── regional_analysis.png
    └── forecast.png
