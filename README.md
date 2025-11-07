# Quant-Portfolio-MarketData-ETL

A robust ETL pipeline for time-series financial data (SPY & VIX), demonstrating data integrity, feature engineering, and readiness for quantitative analysis.

## 🎯 Project Objective

This project builds a foundational ETL (Extract, Transform, Load) pipeline. It ingests raw financial data, demonstrates data resilience by cleaning and imputing errors, engineers new features (trend and risk), and saves a clean, feature-rich dataset ready for advanced backtesting.

## 🛠️ Technical Stack

* **Language:** Python
* **Data Source:** `yfinance`
* **Analysis:** `pandas`, `numpy`
* **Documentation:** `Jupyter Notebook`

## 📂 Project Assets

* **`MarketData-ETL.ipynb`**: The Jupyter Notebook containing all Python code, execution, and step-by-step documentation of the ETL process.
* **`SPY_VIX_Raw.csv`**: The raw, merged, un-cleaned data file.
* **`SPY_Clean_Featured_Data.csv`**: The final, clean, and feature-rich dataset. This is the output deliverable, ready for modeling.

## 📈 Final Data Columns

The final clean CSV file includes:
* **SPY_Close**: Adjusted closing price for SPY.
* **VIX_Close**: Closing value for the VIX.
* **SPY_Log_Returns**: Daily log returns for SPY.
* **SMA_20**: 20-Day Simple Moving Average of SPY_Close.
* **Volatility_20**: 20-Day rolling standard deviation of SPY_Log_Returns.