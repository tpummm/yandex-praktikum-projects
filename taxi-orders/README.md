# Taxi orders

## Description

The dataset consists of historical taxi orders

**Purpose:** forecast taxi orders in order to manage drivers' activity for the next hour

**Metrics of success:** RMSE < 48

**Features:** 
- `datetime` — time of orders

**Target:** 
- `num_orders` — number of orders

## Tools used:
- for tables - `pandas`
- for visualization - `matplotlib.pyplot`, `seaborn`
- for trend and seasonality detection - `statsmodels.tsa.seasonal`
- for regression - `sklearn.linear_model`, `sklearn.ensemble`, `lightgbm`
- for quality metrics - `sklearn.metrics`

## Results:
- While forecasting taxi orders for the next hour gradient boosting model demonstrated lowest RMSE (42.5)
- The quality of gradient boosting model exceeds one of constant models (80.4 and 58.9)
- Some fluctuations that happen in the morning on certain days cannot be detected
