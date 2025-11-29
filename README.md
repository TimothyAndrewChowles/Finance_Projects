# 📈 Leveraged ETF Backtesting & Monte Carlo Simulation

## Overview
This project analyzes the long-term performance and risk of **leveraged ETFs (TQQQ)** compared to their underlying unleveraged ETF **(QQQ)**.  
It combines **historical backtesting** and **Monte Carlo simulations** to evaluate how leverage, volatility, and disciplined reinvestment affect portfolio growth over time.

The goal is to build a **data-driven investment thesis** exploring how younger, risk-tolerant investors might benefit from leveraged ETFs—particularly when held inside **tax-advantaged accounts** such as Roth IRAs or 401(k)s.

---

## 🎯 Objective
Simulate and compare two investment strategies since TQQQ’s inception:

### Strategy 1 – TQQQ (10%+ Dip DCA Strategy)
- Initial investment: **$3,000**
- Add **$500** whenever TQQQ drops **10% or more** in a single trading day
- Buy additional shares at the **next day’s open**
- Continue accumulating over time and track total invested capital

### Strategy 2 – QQQ (Perfect Timing Strategy)
- Invest **$3,000** once per year at that year’s **lowest closing price**
- Represents an idealized “perfect timing” benchmark

---

## ⚙️ Methodology
1. Loaded and cleaned historical TQQQ and QQQ data  
2. Simulated both investment strategies day-by-day  
3. Tracked portfolio values, total invested capital, and daily returns  
4. Visualized cumulative growth and drawdowns on a single graph  
5. Computed performance and risk metrics  
6. Performed Monte Carlo simulations to model random future paths  

---

## 🧮 Tools & Libraries
- **Python**
  - `pandas` – data manipulation and time-series analysis  
  - `numpy` – numerical computation  
  - `matplotlib` / `seaborn` – visualization  
  - `scipy` – Monte Carlo and statistical distributions  

---

## 📊 Metrics Calculated

| Metric | Definition |
|--------|-------------|
| **CAGR** | Compound Annual Growth Rate |
| **Volatility** | Annualized standard deviation of daily returns |
| **Sharpe Ratio** | Risk-adjusted return (higher = better per unit of volatility) |
| **Sortino Ratio** | Risk-adjusted return penalizing downside risk only |
| **Max Drawdown** | Largest peak-to-trough decline over the period |
| **Calmar Ratio** | Return vs. drawdown trade-off (CAGR / Max Drawdown) |
| **VaR (95%)** | 5% worst-case daily loss estimate |
| **CVaR (95%)** | Average daily loss beyond the VaR threshold |

---

## 📈 Visualization
The model plots both strategies’ cumulative growth since TQQQ’s inception:
- **Blue line:** TQQQ (10% Dip DCA Strategy)
- **Orange line:** QQQ (Perfect Timing Benchmark)

This allows for direct comparison of compounding, drawdowns, and recovery speeds.

---

## 💡 Key Results

| Metric | **TQQQ (Dip DCA)** | **QQQ (Perfect Timing)** |
|---------|---------------------|---------------------------|
| **CAGR** | 0.50 | 0.30 |
| **Volatility** | 0.61 | 0.20 |
| **Sharpe Ratio** | 0.83 | 1.48 |
| **Sortino Ratio** | 1.08 | 2.10 |
| **Max Drawdown** | 0.81 | 0.30 |
| **Calmar Ratio** | 0.62 | 1.02 |
| **VaR (95%)** | -0.06 | -0.02 |
| **CVaR (95%)** | -0.09 | -0.03 |

---

## 🧠 Interpretation of Results
- **TQQQ** outperformed in total growth (CAGR 50% vs. 30%) but carried higher volatility and deeper drawdowns.  
- **QQQ** provided smoother, more consistent returns with better risk-adjusted performance (Sharpe and Sortino).  
- Despite the risk, the **dip-buying strategy** allowed TQQQ to capture extreme upside over long periods.  
- The **Calmar Ratio** shows that while TQQQ’s drawdowns were severe, its returns still compensated for that risk in trending markets.  
- **Monte Carlo results** confirmed that extended bull markets strongly favor leveraged exposure, while prolonged bear markets erode value quickly.  

---

## 💬 Investment Thesis
1. **Younger investors** with long time horizons can afford short-term volatility.  
2. **TQQQ**, when held in **tax-advantaged accounts** (e.g., Roth IRA), removes the tax drag from daily derivative turnover.  
3. **Volatility hurts traders but rewards disciplined investors** who buy dips and hold through cycles.  
4. Leveraged ETFs can act as a **“growth amplifier”** for early investors who contribute regularly and resist emotional selling.  
5. Over decades, **time, compounding, and tax-free growth** outweigh short-term market noise.

---

## 🔬 Future Enhancements
- Add support for **SPXL vs SPY** or other 3× leveraged ETFs  
- Introduce **volatility-based entry filters**  
- Expand Monte Carlo runs with varying market drift and volatility assumptions  
- Include **after-tax return modeling** for taxable vs. Roth accounts  

---

## 🧾 Author
**Timothy Chowles**  
Finance & Information Systems | Illinois State University  
Exploring applied finance, investment analytics, and portfolio research  

📧 timothy.chowles@outlook.com
🔗 [LinkedIn](https://www.linkedin.com/in/timothy-chowles)

---
