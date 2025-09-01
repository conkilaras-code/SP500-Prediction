# S\&P 500 Next-Day Closing Price Prediction

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python) ![License: MIT](https://img.shields.io/badge/License-MIT-green)

This project predicts the **next-day closing price** of the S\&P 500 index using a **linear regression model** trained on historical data.

---

## **Features**

* **Lagged Closes:** Previous day and 5-day lag
* **Moving Averages:** 5, 50, 100-day averages
* **Daily Returns & Volatility**
* **Standardized features** with `StandardScaler`
* **Sequential train/test split** for time-series integrity

---

## **Quick Start**

1. **Clone the repository**

```bash
git clone https://github.com/yourusername/sp500-linear-regression.git
cd sp500-linear-regression
```

2. **Install dependencies**

```bash
pip install pandas numpy matplotlib seaborn yfinance scikit-learn
```

3. **Run the Jupyter Notebook**

```bash
jupyter notebook
```

4. Explore: feature engineering, model training, evaluation, and next-day prediction.

---

## **Evaluation Metrics**

* **Mean Squared Error (MSE)**
* **Root Mean Squared Error (RMSE)**
* **R² Score**

---

## **Model Limitations**

* **Autocorrelation:** Prices are sequential; the model may appear accurate without capturing new trends.
* **Past ≠ Future:** Historical patterns may not continue.
* **Overfitting:** Model can capture noise instead of meaningful patterns.
* **Limited features:** External factors like macroeconomics are not included.
* **Testing limitations:** Single train/test split; rolling-window or walk-forward testing would be more realistic.

---

## **Summary**

Predicting stock prices is inherently difficult due to the complex and dynamic nature of financial markets. Prices are influenced by countless factors, and no single model can perfectly forecast future movements. Attempting such predictions is a core aspect of finance—trying to anticipate the unpredictable behavior of markets.

---

## **License**

MIT License
