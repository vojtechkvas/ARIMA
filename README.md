# ARIMA Model Fitting and Time Series Prediction

---

## Overview

This project provides a comprehensive workflow for **time series analysis** and **forecasting** using the **Autoregressive Integrated Moving Average (ARIMA)** model. The core steps involve generating a synthetic time series, analyzing its statistical properties, fitting an optimal ARIMA model, and generating predictions with confidence intervals.

### Key Features
* **Synthetic Data Generation:** Creates a non-stationary time series using `statsmodels.tsa.arima_process.ArmaProcess` and a cumulative sum (`np.cumsum`).
* **Time Series Plotting:** Utilizes a custom utility function (`tsplot` in `utils.py`) to visualize the time series, its **Autocorrelation Function (ACF)**, and **Partial Autocorrelation Function (PACF)**.
* **Model Fitting:** Fits an ARIMA model (specifically shown as **ARIMA(1,1,1)**) and explores model selection using tools like `pmdarima` for automated parameter search (e.g., based on **BIC**).
* **Prediction and Forecasting:** Generates in-sample predictions and long-run forecasts, demonstrating that a series with a differentiation order of $d=1$ tends to forecast as a **straight line** over the long term.

---

## Installation

To set up the environment, clone the repository and install the required Python packages using `pip` and the `requirements.txt` file.

```bash
pip install -r requirements.txt