# 📊 Quantitative Finance Regression Analysis with Alpha Signals

This project demonstrates how to build and evaluate alpha signals from raw stock and macroeconomic data using both time-series and cross-sectional regression techniques. It explores momentum, volume surprise, volatility, and beta in explaining weekly stock return differences, while offering hands-on practice with model diagnostics and out-of-sample testing.

---

## 🔍 What It Does

- Loads historical data for FAANG stocks + market/macro indices (VIX, TLT, DXY)
- Constructs alpha signals like:
  - 1M & 3M Momentum
  - Volume Surprise
  - Rolling Volatility
  - Rolling Beta
- Adds macro factors (fear index, bonds, dollar strength)
- Runs:
  - 📈 Time-series regressions (e.g., AAPL ~ SPY + Signals)
  - 📉 Cross-sectional regressions (e.g., returns ~ factors across stocks per week)
- Tests for predictive power with out-of-sample evaluation
- Interprets R², t-stats, alpha coefficients, and model robustness

---

## 🧠 What I got to Learn

- How to engineer technical and macro signals for finance
- How to explain stock returns using regression models
- Which factors matter for stock return prediction and why
- The difference between exposure (explanation) vs prediction
- The importance of out-of-sample testing and model diagnostics

---

## 🧪 Key Findings

| Factor      | Result                             |
|-------------|-------------------------------------|
| SPY         | Strongest time-series driver        |
| VIX         | Strong negative impact on returns   |
| Mom1M       | Reversal effect in cross-section    |
| Mom3M       | Positive continuation in time-series|
| Volatility  | Low-vol stocks outperform           |
| VolumeSurp  | Mixed results, not reliable alone   |
| Beta        | No clear reward for high risk       |

---

## 🧰 Tech Stack

- Python, pandas, yfinance, statsmodels
- Jupyter Notebook
- Data from Yahoo Finance

---

## 🚀 How To Run

1. Clone this repo
2. Install dependencies:
   ```bash
   pip install yfinance pandas numpy statsmodels
