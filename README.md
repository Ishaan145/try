# Quantitative Research Report on Stock Analysis with Case Study on BSE Ltd (BSE-EQ)
<p align="justify">
This project combines equity research with quantitative finance techniques and Python based modeling to simulate and analyze BSE Ltd.'s stock price behavior using historical and derivative market data.
Purpose of this report is to Elevating Traditional Stock Analysis with Advanced Quantitative Methods and Python. This project is created as part of academic blend finance and technology using Python. It demonstrates how financial data can be transformed into actionable insight through simulation and modeling.
</p>

## Contents

- **Fundamentals & Financials** Business, Pe/Pb, Dividend, Comparison 
- **Monte Carlo Simulation** using Geometric Brownian Motion
- **Linear Regression** on EPS vs Stock Price for valuation forecasting
- **Visualization** of price paths, histograms, and technical signals
- **Black-Scholes Model** for European option pricing
- **Technical Analysis**: Chart, EMA (20/50/100), IV, Fibonacchi Levels
- **Derivative Analysis**

## Libraries Used

- `numpy`, `pandas` – numerical & data analysis
- `matplotlib`, `seaborn` – plotting
- `scikit-learn` – regression modeling
- `scipy.stats` – statistical calculations
- `yfinance` – historical data

## Files

- [`BSE_Derivative_data.csv`](https://ishaan145.github.io/Equity-Research/Main/Derivative/Data/BSE_Derivative_data.csv) – main Jupyter Notebook
- [`BSE_Derivative_data.csv`](https://ishaan145.github.io/Equity-Research/Main/Derivative/Data/BSE_Derivative_data.csv) – printable report version
- [`BSE_Derivative_data.csv`](https://ishaan145.github.io/Equity-Research/Main/Derivative/Data/BSE_Derivative_data.csv) – simulated outcome statistics
- [`BSE_Derivative_data.csv`](https://ishaan145.github.io/Equity-Research/Main/Derivative/Data/BSE_Derivative_data.csv) –  [View Option Data](https://ishaan145.github.io/Equity-Research/Main/Derivative/Data/Option_data.html)

## Disclaimer
<p align="justify">
All data used is for educational purposes. No investment advice is provided. This report is intended purely for educational purposes.
All data presented in this report has been sourced from publicly available data as of 08/07/2025, information on the National Stock Exchange of India Ltd (NSE) website: https://www.nseindia.com/get-quotes/equity?symbol=BSE 
</p>
---

**Author**: Ishaan Saxena  
**Release**: You can view the project document by downloading the [**Project Report**](https://ishaan145.github.io/Equity-Research/Main/Derivative/Data/BSE_Derivative_data.pdf).  
**Released On** August 2025

## Overview
<p align="justify">
The primary objective of this report is to demonstrate how a foundational stock analysis, such as the comprehensive research on BSE Ltd. provided, can be significantly enhanced through the integration of advanced quantitative techniques and computational tools, particularly Python. While fundamental and technical analyses offer indispensable insights into a company's intrinsic value and market sentiment, quantitative methods introduce layers of statistical rigor, predictive modeling, and sophisticated risk assessment. These advanced approaches are increasingly vital in navigating the complexities of modern financial markets, providing a more robust and data-driven perspective for investment decisions. This report aims to bridge the gap between conventional financial research and cutting-edge analytical capabilities.
</p>

## Structure
<p align="justify">
This report is structured to provide a comprehensive and integrated assessment of BSE Ltd. It commences with a review of the existing fundamental and technical analyses, building upon the initial research provided. Subsequently, it introduces a layer of quantitative enhancements, detailing how Python-based methodologies can be applied to deepen the understanding of stock behavior and market dynamics. The analytical approach emphasizes the synthesis of observations from all these layers fundamental, technical, and quantitative to deliver a holistic and robust evaluation of BSE Ltd.'s investment profile and future outlook.
</p>

##  Quantitative Models

###  Monte Carlo Simulation
**Simulation Parameters:**
```python
S0 = 2376.30      # Current stock price
mu = 0.12         # Expected annual return
sigma = 0.45      # Annual volatility
T = 1             # Time horizon (1 year)
steps = 252       # Trading days
n_simulations = 1000
```

**Key Results:**
- **Mean Ending Price**: ₹2,686.52
- **Median Ending Price**: ₹2,441.62
- **95% Confidence Interval**: ₹1,172.30 - ₹5,171.12

###  Other Models Implemented
- **Linear Regression**: EPS vs Stock Price correlation
- **Black-Scholes Model**: European option pricing
- **Geometric Brownian Motion**: Price path simulation

##  Technical Analysis

### Moving Averages (EMA)
| EMA Period | Level | Status | Signal |
|------------|-------|--------|---------|
| **EMA(20)** | ₹2,693.10 |  Resistance | Bearish |
| **EMA(50)** | ₹2,534.77 |  Resistance | Bearish |
| **EMA(100)** | ₹2,273.15 |  Support | Critical |

###  Key Support & Resistance
- **Immediate Support**: ₹2,400 (Strong OI buildup)
- **Resistance Zone**: ₹2,550 - ₹2,600
- **Critical Support**: ₹2,273 (EMA 100)

###  Option Chain Insights
- **Max Pain Zone**: ₹2,500
- **High Call OI**: ₹2,600-₹2,700 strikes
- **High Put OI**: ₹2,400-₹2,500 strikes
- **Implied Volatility**: 45-47% (elevated)

## ⚙️ Installation & Usage

### Prerequisites
```bash
pip install numpy pandas matplotlib seaborn scikit-learn scipy yfinance
```

### Quick Start
```python
# Clone the repository
git clone https://github.com/yourusername/BSE-Stock-Analysis.git

# Navigate to project directory
cd BSE-Stock-Analysis

# Run the analysis
python bse_analysis.py
```

##  Project Structure

```
BSE-Stock-Analysis/
├──  README.md         
├──  report.html 
├──  bse_analysis.py    
├──  data/
│   ├── BSE_Derivative_data.csv
│   └── historical_prices.csv
├──  images/
│   ├── monte_carlo_simulation.png
│   ├── ema_analysis.png
│   └── fibonacci_levels.png
├──  notebooks/
│   └── BSE_Analysis.ipynb
└──  docs/
    └── methodology.md
```

##  Key Findings

<div align="center">
  <h3> Investment Thesis: CAUTIOUS STANCE</h3>
</div>

###  Bearish Indicators
- **Overvaluation**: P/E of 86.5x vs peers (20-45x)
- **Technical Breakdown**: Below EMA(20) and EMA(50)
- **High IV**: Market expects significant volatility
- **SEBI Regulatory Impact**: Jane Street ban affecting derivative volumes

###  Key Risks
- **Valuation Stretch**: Highest P/E among global exchange operators
- **Technical Weakness**: Strong bearish momentum
- **Regulatory Headwinds**: Derivative volume concerns
- **Competition**: Upcoming NSE IPO

###  Potential Catalysts
- **Strong Fundamentals**: Record Q3 FY25 performance
- **Market Leadership**: Technology and brand advantages
- **Economic Moat**: Sustainable competitive advantages


##  Data Sources

- **Primary**: [NSE India](https://www.nseindia.com/get-quotes/equity?symbol=BSE)
- **Historical Data**: Yahoo Finance API
- **Option Chain**: Real-time derivative market data
- **Financial Statements**: Public filings and quarterly reports

##  Disclaimer

<div align="center">
  <p><strong>IMPORTANT NOTICE</strong></p>
</div>

<p align="justify">
<strong>This report is intended purely for educational purposes.</strong> All data presented has been sourced from publicly available information as of July 8, 2025. This analysis does not constitute investment advice, and readers should conduct their own research and consult with qualified financial advisors before making any investment decisions.
</p>

<p align="justify">
The quantitative models and simulations presented are based on historical data and mathematical assumptions that may not accurately predict future market behavior. Past performance does not guarantee future results.
</p>

---

<div align="center">
  <h3>📧 Contact & Collaboration</h3>
  <p>
    <strong>Author:</strong> Ishaan Saxena<br>
    <strong>Release Date:</strong> August 2025<br>
    <strong>Project Type:</strong> Academic Research & Financial Analysis
  </p>
  
  <p>
    <a href="mailto:your.email@domain.com"> Email</a> |
    <a href="https://linkedin.com/in/yourprofile"> LinkedIn</a> |
    <a href="https://github.com/yourusername"> GitHub</a>
  </p>
</div>

---

<div align="center">
  <p><em> If you found this research helpful, please consider starring this repository!</em></p>
  <p><strong>🔗 <a href="./report.html">Access Complete Interactive Report</a></strong></p>
</div>
