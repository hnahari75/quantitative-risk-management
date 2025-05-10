# Quantitative Risk Management: Monte Carlo VaR with Futures Hedging

In this project, we construct a portfolio through Markowitz theory for a 1-year investment horizon and hedge it using index futures to reduce the systematic risk of the market. We implement a Monte Carlo Value at Risk (VaR) model using historical data and simulations via geometric Brownian motion, and compare the VaR for both the hedged and unhedged portfolios. We observe the efficiency of the hedging and successfully reduce the risk.

##  Overview

- **Goal**: Use Monte Carlo simulations to evaluate risk and make it quantifiable, then significantly reduce the portfolio’s exposure to systematic market risk.
- 
- **Approach**:
  - Construct a portfolio by implementing Markowitz portfolio theory and applying it on the historical (daily) closing prices of non-dominated stocks.
  - Use the the historical data and geometric brownian motion to simulate the future behaviors of the prices.
  - Use this simulation to calculate the Value at Risk (VaR) of the portfolio, before hedging.
  - Use Capital Asset Pricing Model (CAPM) to calculate beta, i.e. to quantify the exposure of the portfolio to the systematic risk of the market (S&P 500 index).
  - Hedge the systematic risk by shorting S&P 500 index futures.
  - Validate the risk reduction by comaring the VaR of the hedged and unhedged portfolios.

##  Technologies

- `Python`
- `Pandas`, `NumPy` – data manipulation and simulation
- `Matplotlib`, `Seaborn` – visualization
- `yfinance` or `pandas_datareader` – data acquisition
- `scikit-learn` (optional) – factor modeling or regression for beta estimation

##  How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/hnahari75/quant-risk-management.git
   cd quant-risk-management
