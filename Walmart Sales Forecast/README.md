
# 🛒 Supermarket Sales Forecasting – Time Series & Machine Learning

## 📌 Overview

This project addresses the problem of **forecasting weekly sales across 45 different supermarket stores** using historical data. Accurately predicting sales is critical for inventory planning, supply chain optimization, and business strategy. The goal is to identify the most effective algorithm to forecast the next **12 weeks** of sales based on two years of historical weekly data.

By leveraging both **traditional time series models** and **modern machine learning techniques**, this project explores the best approach to forecasting sales in a retail environment.

---

## ❓ Problem Statement

Supermarkets often struggle with:
- Overstocking and understocking products.
- Inefficient resource allocation.
- Revenue losses due to poor demand prediction.

**Objective:**  
To develop a predictive system that can accurately forecast **weekly sales for each store** over the next **12 weeks**, helping businesses:
- Make data-driven inventory decisions.
- Improve financial planning.
- Optimize supply chains.

---

## 🔍 Dataset

- Historical sales data spanning **2 years** (weekly frequency).
- Contains **45 different stores**, each with their own sales patterns.
- Features used:
  - `Store`: Store ID
  - `Date`: Weekly timestamps
  - `Weekly_Sales`: Sales revenue for each store

---

## ⚙️ Techniques Used

Three forecasting approaches were implemented and compared:

### 1. **SARIMA (Seasonal ARIMA)**
- Captures seasonality and trends in time series data.
- Trained store-wise using parameters tuned manually and via ADF tests.
- Output: Individual forecasts per store + Global RMSE & MSE.

### 2. **XGBoost (Gradient Boosted Trees)**
- Powerful ensemble learning model for structured data.
- Feature engineered:
  - Lag features (previous week sales)
  - Date-based features (month, week, year, etc.)
- Trained on all stores combined.
- Output: Individual forecasts per store + Global RMSE & MSE.

### 3. **Deep Learning (LSTM)**
- Recurrent Neural Network to handle sequential data.
- Inputs reshaped into 3D format (samples, timesteps, features).
- Output: Global and store-wise forecasts.
- Still under refinement — shows promise but needs tuning.

---

## 📈 Evaluation Metrics

To evaluate model performance:

- **RMSE (Root Mean Squared Error)** – Emphasizes large errors.
- **MSE (Mean Squared Error)** – Penalizes squared errors.

| Model         | RMSE           | MSE               |
|---------------|----------------|-------------------|
| SARIMA        | 94,309.81      | 6.89 × 10⁹         |
| **XGBoost**   | **56,263.98**  | **3.17 × 10⁹**     |
| Deep Learning | 95,187.24      | 9.06 × 10⁹         |

---

## ✅ Conclusion

- **XGBoost outperforms** traditional time series models and deep learning in this setup.
- Best suited for this kind of tabular, multi-store sales data.
- **SARIMA** performs reasonably well but struggles with scalability and variance across stores.
- **Deep Learning** is promising but requires further tuning and more data for optimal performance.

---




## 🛠️ Tools & Libraries

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- **Statsmodels** – for SARIMA
- **XGBoost**
- **TensorFlow / Keras** – for LSTM
- Scikit-learn

---

## 📊 Visualizations

Each model includes:
- Line plots comparing actual vs predicted sales
- Error distribution graphs
- RMSE/MSE tables

---

## 🙌 Acknowledgements

Special thanks to open-source contributors and datasets that made this project possible. Inspired by real-world retail forecasting challenges.

---

## 📬 Contact

For collaboration or queries:
📧 kumarabhaykatiyar@gmail.com

---
