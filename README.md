# 📊 Investment Portfolio Management

A Python-based financial analytics project that evaluates investment returns, portfolio risk, asset correlations, and diversification strategies using historical ETF data.

## 📌 Project Overview

This project analyzes four exchange-traded funds (ETFs) representing US equities, international equities, bonds, and gold. It compares three hypothetical investment portfolios—Conservative, Balanced, and Growth—to understand how asset allocation influences historical risk and return.

The project also includes a dashboard with financial KPIs, asset allocation charts, historical portfolio growth, risk-return comparisons, and a correlation heatmap.

## 🎯 Project Objectives

- Collect and analyze historical financial market data.
- Calculate daily returns and annualized performance metrics.
- Measure investment risk using annualized volatility.
- Analyze correlations between asset classes.
- Construct and compare diversified portfolio allocations.
- Visualize historical portfolio performance.
- Explore hypothetical investment growth scenarios.

## 🛠️ Tools and Technologies

- **Python** — financial analysis and calculations
- **Google Colab** — notebook development and execution
- **Pandas** — data manipulation and analysis
- **NumPy** — numerical calculations
- **Matplotlib** — data visualization
- **yfinance** — historical market data retrieval

## 📈 Dataset

Historical adjusted price data is retrieved using Yahoo Finance through the `yfinance` Python library.

| ETF  | Asset Class            | Portfolio Role                |
| ---- | ---------------------- | ----------------------------- |
| SPY  | US equities            | Domestic stock exposure       |
| VXUS | International equities | International diversification |
| BND  | Bonds                  | Fixed-income exposure         |
| GLD  | Gold                   | Alternative asset exposure    |

The dataset covers the historical period requested in the notebook, beginning January 2021. The actual end date depends on data availability when the notebook is executed.

## 🔍 Methodology

### 1. Data Collection and Preparation

Retrieved historical adjusted prices, organized the data using pandas, and handled missing observations.

### 2. Return Analysis

Calculated daily percentage returns and annualized historical returns.

### 3. Risk Analysis

Measured annualized volatility using the standard deviation of daily returns and the square root of 252 trading days.

### 4. Correlation Analysis

Constructed a correlation matrix and heatmap to examine relationships between asset returns and assess potential diversification benefits.

### 5. Portfolio Construction

Created three hypothetical portfolio allocations:

| Asset Class          | Conservative | Balanced |   Growth |
| -------------------- | -----------: | -------: | -------: |
| US Stocks            |          20% |      45% |      65% |
| International Stocks |          10% |      20% |      25% |
| Bonds                |          60% |      25% |       5% |
| Gold                 |          10% |      10% |       5% |
| **Total**            |     **100%** | **100%** | **100%** |

### 6. Portfolio Performance Evaluation

Compared the portfolios using annualized returns, annualized volatility, and the Sharpe ratio under a zero risk-free-rate assumption.

### 7. Dashboard Development

Created visualizations to communicate asset allocation, historical portfolio growth, risk-return trade-offs, and asset correlations.

### 8. Scenario Analysis

Calculated illustrative compound-growth scenarios using hypothetical annual return assumptions. These scenarios are not predictions of future market performance.

## 📊 Dashboard

The dashboard includes:

- **Portfolio Allocation:** stacked chart comparing asset weights.
- **Historical Portfolio Growth:** simulated growth of a hypothetical $10,000 investment.
- **Risk vs. Return:** comparison of annualized return and volatility.
- **Correlation Heatmap:** visualization of relationships between asset returns.
- **Portfolio KPIs:** return, volatility, Sharpe ratio, and ending portfolio value.



## 💡 Key Findings

The historical analysis illustrates how different portfolio allocations can produce different risk-return outcomes.

- Asset correlations vary, which can affect diversification benefits.
- Portfolio returns and volatility depend on both individual asset performance and portfolio weights.
- A portfolio with a conservative allocation does not necessarily produce the lowest historical volatility in every period.
- Scenario analysis demonstrates the impact of compounding under different assumed annual returns.

Actual numerical findings should be interpreted using the metrics generated when the notebook is executed.

## 🚀 How to Run the Project

1. Clone or download this repository.
2. Open `Investment_Portfolio_Management.ipynb` in Google Colab.
3. Run the notebook cells from top to bottom.
4. Allow the notebook to install dependencies and download market data.
5. Review the tables, dashboard, and scenario analysis.

An internet connection is required to retrieve historical market data.

## 📁 Repository Structure

```text
investment-portfolio-management/
├── Investment_Portfolio_Management.ipynb
├── investment_portfolio_dashboard.png
└── README.md
```

## ⚠️ Limitations

- Historical performance does not guarantee future results.
- Correlations and volatility can change over time.
- The analysis excludes taxes, transaction costs, and fund expenses.
- Results depend on the selected historical period and portfolio rebalancing assumptions.
- Forecast scenarios use hypothetical return assumptions.
- Portfolio allocations are educational examples, not personalized investment recommendations.

## 🎓 Learning Outcomes

Through this project, I practiced:

- Financial data collection and preprocessing
- Investment return and risk calculations
- Correlation and diversification analysis
- Portfolio allocation and performance comparison
- Financial data visualization
- Python-based analytical reporting

## 👩‍💻 Author

**Your Name**

Connect with me on [LinkedIn](www.linkedin.com/in/mahitha-kalinathabotla).

---

*This project is for educational purposes only and does not constitute financial or investment advice.*
