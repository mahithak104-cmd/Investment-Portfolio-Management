# Investment Portfolio Management

## Transforming Historical Market Data into Actionable Investment Insights

Investment decisions require more than tracking stock prices. Investors need to understand risk, evaluate returns, analyze relationships between asset classes, and determine how portfolio allocation influences overall performance.

This project analyzes historical financial market data for four exchange-traded funds (ETFs) representing US equities, international equities, bonds, and gold. Using Python-based financial analysis, the project compares three hypothetical investment portfolios—Conservative, Balanced, and Growth—to evaluate their historical performance, volatility, and diversification characteristics.

Through financial data analysis, correlation modeling, portfolio allocation, and dashboard development, this project demonstrates how historical market data can be transformed into meaningful investment insights and data-driven portfolio comparisons.

## Tools & Technologies

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- yfinance
- Financial Data Analysis
- Portfolio Risk Analysis
- Correlation Analysis
- Data Visualization

## Business Problem

Investors must balance potential returns against investment risk while considering diversification across different asset classes. However, historical price data alone does not clearly explain how investments behave individually or how their interactions influence portfolio performance.

A structured analytical approach is needed to compare investment alternatives, evaluate historical risk-return trade-offs, understand diversification opportunities, and communicate findings through clear visualizations.

This project addresses these challenges by developing a Python-based framework for analyzing asset performance and comparing hypothetical portfolio allocations.

## Analytical Objectives

- How have the selected asset classes performed historically?
- Which assets experienced greater return variability?
- How strongly are the selected asset classes correlated?
- How do conservative, balanced, and growth-oriented allocations compare?
- Which portfolio achieved the highest historical return relative to volatility?
- How did a hypothetical $10,000 investment grow over the observed period?
- How do different annual return assumptions affect long-term investment growth?
- What limitations should investors consider when interpreting historical results?

## Dataset

Historical adjusted price data was retrieved from Yahoo Finance using the `yfinance` Python library.

Four ETFs were selected to represent different asset classes:

| ETF | Asset Class | Analytical Purpose |
|---|---|---|
| SPY | US Equities | Analyze domestic stock-market performance |
| VXUS | International Equities | Evaluate international diversification |
| BND | Bonds | Examine fixed-income performance |
| GLD | Gold | Analyze an alternative asset class |

The analysis begins on January 1, 2021. The final date depends on the market data available when the notebook is executed.

## Analytical Methodology

### 1. Data Collection and Preparation

Historical adjusted closing prices were retrieved and organized into a structured pandas DataFrame.

Data preparation included:
- Selecting the required ETF price series
- Organizing observations by trading date
- Checking missing values
- Preparing the dataset for return calculations

### 2. Investment Return Analysis

Daily percentage returns were calculated to measure changes in asset prices between consecutive trading sessions.

Annualized historical returns were calculated to compare the compounded growth rates of the selected assets and hypothetical portfolios.

This analysis provides a common framework for comparing historical investment performance.

### 3. Investment Risk Analysis

Annualized volatility was calculated using the standard deviation of daily returns and an assumed 252 trading days per year.

Volatility was used as a measure of historical return variability to compare the relative risk characteristics of the portfolios.

### 4. Correlation Analysis

A Pearson correlation matrix and heatmap were developed to examine the relationships between asset-class returns.

The analysis helps identify assets that have historically moved more closely together or exhibited weaker linear relationships, which may influence diversification benefits.

### 5. Portfolio Construction

Three hypothetical portfolios were created to compare different asset allocation strategies.

| Asset Class | Conservative | Balanced | Growth |
|---|---:|---:|---:|
| US Stocks | 20% | 45% | 65% |
| International Stocks | 10% | 20% | 25% |
| Bonds | 60% | 25% | 5% |
| Gold | 10% | 10% | 5% |
| **Total Allocation** | **100%** | **100%** | **100%** |

The portfolios were designed to demonstrate how changes in asset weights can influence historical portfolio behavior.

### 6. Portfolio Performance Evaluation

The portfolios were compared using the following metrics:

- **Annualized Return:** Measures historical compounded investment growth.
- **Annualized Volatility:** Measures the variability of portfolio returns.
- **Sharpe Ratio:** Evaluates historical return relative to volatility, assuming a zero risk-free rate.
- **Ending Portfolio Value:** Shows the simulated value of an initial $10,000 investment.

The historical portfolio calculations assume daily rebalancing to the specified target weights. Transaction costs, taxes, and fund expenses are excluded.

### 7. Dashboard Development

A financial dashboard was developed using Matplotlib to summarize portfolio performance and asset relationships.

The dashboard combines portfolio allocation, historical growth, risk-return comparisons, and a correlation heatmap into a single visual report.

### 8. Scenario-Based Forecasting

Illustrative five-year compound-growth scenarios were calculated using hypothetical annual returns of 2%, 6%, and 10%.

The scenarios demonstrate how different assumed growth rates affect potential investment values over time. They are mathematical illustrations, not predictions of actual market returns.

## Investment Portfolio Management Dashboard

The dashboard presents key portfolio metrics and visualizations to support financial analysis and comparison.

### Dashboard Preview

<img width="4765" height="3248" alt="investment_portfolio_dashboard" src="https://github.com/user-attachments/assets/9e82f6e8-2419-4fff-9e8b-297d6e6120b2" />

### Dashboard Highlights

- Comparison of three hypothetical portfolio allocations
- Historical growth of a simulated $10,000 investment
- Risk-versus-return visualization
- Asset-class correlation heatmap
- Annualized return and volatility KPIs
- Sharpe ratio comparison
- Illustrative investment growth scenarios

## Key Findings

### 1. Asset Correlation Analysis

The historical correlation matrix showed differences in how the selected asset classes moved together.

- Bonds and gold exhibited a correlation of approximately **0.80**.
- International stocks and bonds exhibited a correlation of approximately **0.16**.
- US and international stocks exhibited a correlation of approximately **0.30**.

These results suggest that diversification benefits vary across asset combinations. Correlations are historical and may change under different market conditions.

### 2. Portfolio Risk-Return Comparison

The initial portfolio analysis produced the following results:

| Portfolio | Annualized Return | Annualized Volatility | Sharpe Ratio |
|---|---:|---:|---:|
| Conservative | 11.64% | 12.14% | 0.968 |
| Balanced | 7.47% | 8.51% | 0.889 |
| Growth | 4.36% | 7.40% | 0.613 |

These are the results from the initial analysis. The metrics should be regenerated and validated using consistent return calculations before being treated as final findings.

The initial results showed that the Conservative portfolio had the highest reported annualized return, while the Growth portfolio had the lowest reported volatility. This illustrates why portfolio labels alone cannot determine actual historical performance.

### 3. Historical Portfolio Growth

A hypothetical $10,000 investment was used to compare portfolio growth over the historical observation period.

The growth visualization highlights differences in the paths and ending values of the three portfolios. These results reflect the selected period, target allocations, and rebalancing assumptions rather than guaranteed future outcomes.

### 4. Scenario-Based Investment Growth

Compound-growth scenarios were used to demonstrate how different assumed annual returns affect the future value of an initial investment.

This analysis illustrates the effect of compounding while emphasizing that actual returns fluctuate and may be negative.

## Key Business Insights

- Diversification should consider correlations between assets rather than allocation percentages alone.
- Higher historical returns do not necessarily indicate lower investment risk.
- Portfolio performance depends on asset behavior, allocation weights, the evaluation period, and rebalancing assumptions.
- Historical volatility and correlation provide useful context but cannot capture every potential market risk.
- Scenario analysis can help communicate long-term growth assumptions and uncertainty.

## How to Run the Project

1. Clone or download this GitHub repository.
2. Open `Investment_Portfolio_Management.ipynb` in Google Colab.
3. Run the notebook cells sequentially from top to bottom.
4. Allow the notebook to install dependencies and retrieve historical market data.
5. Review the return calculations, correlation matrix, portfolio comparisons, and dashboard visualizations.

An internet connection is required to retrieve historical prices.

## 📁 Repository Structure

```text
investment-portfolio-management/
│
├── Investment_Portfolio_Management.ipynb
├── investment_portfolio_dashboard.png
└── README.md
```

## Skills Demonstrated

- Financial data collection and preprocessing
- Python-based financial analysis
- Investment return and volatility calculations
- Correlation and diversification analysis
- Portfolio allocation and comparison
- Financial KPI development
- Data visualization and dashboard design
- Analytical interpretation and reporting

## Author

**Mahitha Kalinathabotla**

Master of Science in Business Analytics  
University at Albany, SUNY

Connect with me on [LinkedIn](www.linkedin.com/in/mahitha-kalinathabotla).

---

*This project is intended for educational purposes only. Historical analysis and hypothetical scenarios should not be interpreted as guarantees of future performance or personalized investment advice.*
