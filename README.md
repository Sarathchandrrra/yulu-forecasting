# yulu-forecasting
Forecasting Yulu ride demand using ARIMA and Prophet

# Yulu Ride Demand Forecasting

This project demonstrates how to forecast ride-sharing demand (simulated for Yulu) using **ARIMA (SARIMAX)** and **Facebook Prophet**.  
It was developed in **Google Colab**, using Python libraries such as `statsmodels`, `prophet`, and `scikit-learn`.

---

## Problem Statement

Yulu, an urban micro-mobility provider, wants to predict:
- Daily ride demand across time  
- Weekly and seasonal variations  
- Improve fleet rebalancing and battery swaps  

---

## Tools & Techniques

| Step | Description |
|------|-------------|
| Data | Synthetic daily rides data (1 year, with weekly seasonality + trend) |
| Models | ARIMA (SARIMAX) and Prophet (additive, weekly seasonality) |
| Metrics | MAPE, RMSE |
| Visualization | Matplotlib + Prophet built-in plots |
| Platform | Google Colab (runs on CPU) |


---

##Results

| Model     | MAPE (%) | RMSE |
|-----------|----------|------|
| ARIMA     | ~12.4    | ~68  |
| Prophet   | ~9.8     | ~54  |

**Prophet outperformed ARIMA** slightly on both accuracy and interpretability (especially in capturing weekly seasonality).

---

##Business Impact (Hypothetical)

- Improved **fleet rebalancing** by predicting weekday/weekend shifts  
- Reduced **bike idle time** by 10–12%  
- Enabled **dashboard-based planning** for operations team  

---

##Files in this repo

- `Yulu_Forecasting.ipynb` – full Colab notebook   
- `README.md` – this file  

---

## 🚀 To Run

```bash
pip install -r requirements.txt
