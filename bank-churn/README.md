# Churn of bank clients

## Description: 
The dataset consists of historical behaviour of bank clients.

**Purpose:** forecast of churn probability in the next 6 months
  
  
**Metrics of success:**  F1 > 0.59 (additional metric - AUC-ROC)
  
  
**Source of data:**  [Kaggle](https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling)
  
  
**Features:**
- `RowNumber` — index of row
- `CustomerId` — unique client identifier
- `Surname` — client's surname of client
- `CreditScore` — client's credit score
- `Geography` — client's location (country)
- `Gender` — client's gender
- `Age` — client's age
- `Tenure` — number of client's real estate objects
- `Balance` — client's account balance
- `NumOfProducts` — number of bank products used by a client
- `HasCrCard` — if a client has a credit card 
- `IsActiveMember` — if a client is active
- `EstimatedSalary` — client's estimated salary 

**Target:**
- `Exited` — client's churn

## Tools used:
  - for tables - `pandas`
  - for scaling numeric data - `sklearn.preprocessing`
  - for classifier - `sklearn.ensemble`, `sklearn.linear_model`
  - for visualization - `seaborn`, `matplotlib.pyplot`

## Results:
  - The best model to forecast bank clients' churn is Random forest with max depth of 9 and 93 estimators
  - Testing this model results in F1 = 0.6
