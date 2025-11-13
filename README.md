# Impact of Electric Vehicles: Data Analysis and Predictive Modeling

This repository contains an exploratory and predictive analysis of Electric Vehicle (EV) trip and performance data. The notebook evaluates how various factors impact EV behavior by applying regression models, time-series forecasting, and anomaly detection methods. The goal is to study EV trip patterns, model future values, and identify unusual usage trends using modern machine learning techniques.

---

## Overview

The notebook analyzes EV-related data by performing several types of modeling and statistical analysis.  
The workflow includes:

1. Loading and inspecting trip-level EV data  
2. Building regression models to estimate EV-related target variables  
3. Time series forecasting with ARIMA  
4. Detecting anomalies in EV trip behavior  
5. Hyperparameter optimization using Grid Search  
6. Evaluating model performance using MSE and R²  

This provides both predictive and diagnostic insights into EV operations.

---

## Dataset

The dataset is imported as a CSV file and includes columns representing trip metrics such as:

- Trip distance  
- Vehicle weight factors  
- Battery usage indicators  
- Habitual vs random trip characteristics  
- Time-based sequences used for forecasting  

The notebook prints `.head()` outputs to provide initial inspection.

---

## Methods and Models Used

### 1. Linear Regression Models
Several regression models are used to analyze relationships between independent features and EV trip target values.

Models include:

- Linear Regression  
- Ridge Regression  
- Gradient Boosting Regressor  

Performance metrics:

- Mean Squared Error (MSE)  
- R² Score  

These metrics help compare how well each model fits the EV data.

---

### 2. Time-Series Forecasting with ARIMA

The notebook applies:

- ARIMA model fitting  
- Residual diagnostics  
- Multi-step forecasting  

The ARIMA process is used to predict future trip-distance values or battery-related trends.

A forecast plot is generated comparing historical data against model-predicted values.

---

### 3. Anomaly Detection with Isolation Forest

The notebook uses IsolationForest to identify:

- Unusual trip lengths  
- Outlier driving patterns  
- Data errors or non-typical user behavior  

A plot is generated to show normal vs anomalous points in the dataset.

This helps understand irregular EV behavior that could indicate operational inefficiencies or abnormal usage.

---

### 4. Gradient Boosting with Grid Search Optimization

To improve predictive accuracy, the notebook uses:

- GradientBoostingRegressor  
- GridSearchCV for hyperparameter tuning  

The process returns:

- Best parameters found  
- Updated model accuracy on the test set  

This step determines the most optimal configuration for EV prediction tasks.

---

## Results Summary

The notebook outputs include:

- MSE and R² scores from multiple regression models  
- ARIMA forecast series for future EV trends  
- Visual anomaly detection results  
- Best parameters and improved R² score after grid search  

These results collectively provide insight into how EV trip patterns can be analyzed and predicted.

---

## Requirements

Install the necessary packages:
pip install pandas numpy scikit-learn statsmodels matplotlib

## How to Run

1. Place the dataset CSV file in the project directory.  
2. Open the notebook in Jupyter or Google Colab.  
3. Run all cells in order.  
4. Review the output plots and evaluation metrics.  

