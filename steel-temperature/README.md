# Forecast of steel temperature

## Description:

**Purpose:** The steel factory wants to optimise its expenses therefore it needs to forecast the temperature of steel after processing

**Metrics of success:** mean absolute error (MAE) < 6.5

**Process description:**
- the first temperature is measured
- steel is heated with electrodes, bulk and wire are added, gas is used - temperature is measured a couple of times
- the last temperature is measured

**Data description:**
- `data_arc.csv` — electrode heating
- `data_bulk.csv` — bulk added (volume)
- `data_bulk_time.csv` — bulk added (time)
- `data_gas.csv` — gas
- `data_temp.csv` — temperature measurements
- `data_wire.csv` — wire added (volume)
- `data_wire_time.csv` — wire added (time)

`Key` is a batch number

## Tools used:
- for tables - `pandas`
- for visualization - `matplotlib.pyplot`, `seaborn`
- for regression - `sklearn.linear_model`, `sklearn.ensemble`, `sklearn.tree`
- for quality metrics - `sklearn.metrics`
- for choosing features - `.feature_importances`, `.corr`

## Results:
- The lowest MAE on test data was achieved while using linear regression
- MAE is 6.16'
