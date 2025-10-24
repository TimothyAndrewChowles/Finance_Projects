```markdown
#Leveraged ETF Backtesting & Monte Carlo Simulation

## Overview
This project explores the long-term performance and risk of **leveraged ETFs** (TQQQ) compared to their unleveraged counterpart (QQQ).  
Using real historical market data, I performed **Monte Carlo simulations** and **backtesting** to understand how different investment strategies would perform since TQQQ’s inception.

The purpose is to develop a **data-driven investment thesis** that examines whether young, risk-tolerant investors can benefit from leveraged ETF exposure, particularly inside tax-advantaged accounts like Roth IRAs.

---

## 🎯 Objective
Simulate and compare the performance of two distinct investment strategies over time.

### Strategy 1 – *TQQQ (10%+ Dip DCA Strategy)*
- Begin with an **initial $3,000 investment**
- Add **$500** whenever TQQQ experiences a **daily drop of 10% or more**
- Purchase additional shares at the **next day’s open**
- Tracks number of additional buys and total invested capital

### Strategy 2 – *QQQ (Perfect Timing Strategy)*
- Invest **$3,000** at each **yearly low closing price**
- Represents a hypothetical “perfect timing” benchmark

---

## 🧮 Methods

### Data & Tools
- **Python** with Pandas, NumPy, and Matplotlib
- Monte Carlo simulation for randomized performance modeling
- Backtesting engine for rule-based investing
- Data visualization for cumulative returns and drawdowns

### Workflow
1. Load historical QQQ and TQQQ price data  
2. Simulate both strategies day-by-day  
3. Record daily portfolio value, drawdowns, and total invested  
4. Compare the performance visually on a single graph  
5. Compute risk and performance metrics  

---

## 📊 Metrics Calculated
| Metric | Description |
|---------|--------------|
| **CAGR** | Compound Annual Growth Rate |
| **Volatility** | Annualized standard deviation of returns |
| **Sharpe Ratio** | Return per unit of total volatility |
| **Sortino Ratio** | Return per unit of downside volatility |
| **Max Drawdown** | Largest peak-to-trough loss |
| **Calmar Ratio** | CAGR divided by Max Drawdown |
| **Value at Risk (VaR)** | Potential daily loss at 95% confidence |
| **Conditional VaR (CVaR)** | Expected loss beyond VaR threshold |

---

## 📈 Visualization
The simulation outputs a chart comparing both strategies since TQQQ’s inception:
- **TQQQ (10% Dip DCA)** — blue line  
- **QQQ (Perfect Timing)** — orange line  

This visualization shows cumulative value, growth trends, and drawdowns, highlighting how volatility impacts compounding over time.

---

## 💡 Investment Thesis
Based on the backtesting and Monte Carlo results:
- **TQQQ outperformed QQQ** over long horizons when the investor stayed disciplined during drawdowns.
- **Time horizon** is the key advantage for young investors; short-term dips compound into long-term gains.
- **Volatility drag** exists but is outweighed by compounding in upward-trending markets.
- **Tax efficiency** is poor in taxable accounts due to short-term gains but excellent in **tax-advantaged accounts** (Roth IRA, 401(k), Traditional IRA).
- For **young investors**, combining consistent contributions, time, and tax sheltering allows leveraged ETFs to serve as long-term growth amplifiers.

---

## 🧠 Findings Summary
| Strategy | CAGR | Max Drawdown | Sharpe | Sortino | Total Invested |
|-----------|------|---------------|---------|----------|----------------|
| **TQQQ (Dip DCA)** | *Higher expected CAGR, higher risk* | *Deeper drawdowns* | *Higher Sharpe in bull markets* | *Outperforms over long horizons* | *Variable (based on dips)* |
| **QQQ (Perfect Timing)** | *Stable CAGR, lower volatility* | *Smaller drawdowns* | *Moderate Sharpe* | *Ideal baseline comparison* | *Fixed $3,000* |

---

## 🔬 Future Improvements
- Add backtesting for **SPXL vs SPY** for broader comparison  
- Introduce **volatility-based rebalancing** filters  
- Expand Monte Carlo analysis across multiple market regimes  
- Include **after-tax return modeling** for taxable vs Roth accounts  

---

## 🧾 Author
**Timothy Chowles**  
Finance & Information Systems | Illinois State University  
Exploring the intersection of data analytics, investing, and long-term wealth building.  
📧 timothy.chowles@siemens.com  
🔗 [LinkedIn](https://www.linkedin.com/in/timothy-chowles)

---
```
