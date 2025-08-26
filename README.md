# 📈 Stock Portfolio Optimization & Quantitative Risk Analysis

This project implements a **complete quantitative investment framework** in Python.  
It covers **dynamic stock selection, portfolio optimization, advanced risk metrics, performance attribution, backtesting**, and **machine learning-based market regime detection**.

---

## 🚀 Key Features

### 1️⃣ Dynamic Stock Selection
- Reads and cleans stock universe from `Companies and Types.csv`.
- Auto-formats tickers (e.g., appending `.NS` for NSE).
- Removes invalid entries.
- Filters stocks based on:
  - Returns above benchmark
  - Sharpe Ratio > 1
  - Controlled volatility

---

### 2️⃣ Portfolio Optimization
- **10,000 random weight simulations**
- Calculates for each:
  - Portfolio return
  - Volatility
  - **Sharpe Ratio**
  - **Sortino Ratio**
- Identifies:
  - Max Sharpe portfolio
  - Min volatility portfolio
  - Max Sortino portfolio
- Visualizes **Efficient Frontier** and optimal portfolios.

---

### 3️⃣ Risk Analysis – Value at Risk (VaR) & Conditional VaR (CVaR)
- Historical method
- Parametric method (Normal Distribution)
- Monte Carlo simulation
- Risk plotted over return distribution with thresholds

---

### 4️⃣ Performance Attribution – CAPM
- Calculates **Alpha**, **Beta**, **Treynor Ratio**, and **R²** using regression against a benchmark.
- Plots CAPM regression line with annotated results.

---

### 5️⃣ Backtesting & Rolling Risk Metrics
- Portfolio vs benchmark:
  - Cumulative returns
  - Rolling volatility
  - Rolling Sharpe Ratio
  - Rolling Sortino Ratio
  - Drawdowns
- Computes **annualized Sortino Ratio**.

---

### 6️⃣ Market Regime Detection (Machine Learning)
- **Random Forest classifier** predicts stable vs risky market regimes.
- Macro indicators used:
  - India VIX
  - USD/INR
  - NIFTY 50
- Visualizes portfolio performance with color-coded regimes.
- Provides feature importance for regime prediction.

---

## 📂 Files
- `Stock Portfolio Optimization using Dynamic stock selection.ipynb` – Main notebook
- `requirements.txt` – Python dependencies
- `README.md` – Project overview

---

## ⚙️ Installation
```bash
git clone https://github.com/YOUR_USERNAME/stock-portfolio-optimization.git
cd stock-portfolio-optimization
pip install -r requirements.txt
jupyter notebook "Stock Portfolio Optimization using Dynamic stock selection.ipynb"
📊 Example Outputs
Efficient Frontier Plot

Optimal Portfolio Allocation

VaR & CVaR Comparison Chart

CAPM Regression Scatter Plot

Rolling Sharpe & Sortino Ratios

Market Regime Heatmap

🛠️ Technologies Used
Python 3.x

pandas, numpy, matplotlib, seaborn

yfinance

statsmodels

scikit-learn

scipy

📜 License
MIT License

✨ Author
Rohith Surya M

GitHub: @RohithSuryaM
