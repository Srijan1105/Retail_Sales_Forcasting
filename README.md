# Retail_Sales_Forcasting
Build a machine learning model to forecast future sales for a retail store based on historical sales data. It can help in inventory planning, resource allocation, and revenue projection.

# 🛒 Walmart Sales Forecasting 📈

This project aims to forecast **weekly sales** for Walmart stores using historical data and machine learning techniques. It explores how factors such as holidays, fuel prices, CPI, unemployment, and seasonal trends affect retail sales.

---

## 📂 Dataset

The dataset used is `Walmart_Sales.csv`, containing:

- `Store`: Store ID
- `Date`: Week ending date
- `Weekly_Sales`: Sales for the given store in that week (target)
- `Holiday_Flag`: Whether the week is a special holiday week (1 or 0)
- `Temperature`, `Fuel_Price`, `CPI`, `Unemployment`: Economic indicators

Dataset Link: https://www.kaggle.com/datasets/mikhail1681/walmart-sales?resource=download
---

## 🧠 Tech Stack

- **Language:** Python
- **Libraries:**
  - `pandas`, `numpy` – data handling
  - `matplotlib`, `seaborn` – data visualization
  - `scikit-learn` – machine learning
  - `joblib` – model serialization

---

## 🔍 Project Workflow

### 1. Data Preprocessing
- Converted `Date` to datetime format
- Extracted features: `Month`, `Week`, `Year`, `DayOfWeek`

### 2. Exploratory Data Analysis (EDA)
- Sales trends by store over time
- Correlation between sales and economic indicators

### 3. Model Building
- **Model Used**: Random Forest Regressor
- Features:
  - `Store`, `Holiday_Flag`, `Temperature`, `Fuel_Price`
  - `CPI`, `Unemployment`, `Month`, `Week`, `Year`, `DayOfWeek`

### 4. Evaluation
- **Metrics:**
  - RMSE (Root Mean Squared Error)
  - MAE (Mean Absolute Error)
- Visual comparison of actual vs predicted sales

---

## 📊 Sample Results

| Metric | Value |
|--------|-------|
| RMSE   | ~XXX  |
| MAE    | ~XXX  |

> (Replace XXX with your actual output values)

---

## 📦 How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/your-username/walmart-sales-forecasting.git
   cd walmart-sales-forecasting
