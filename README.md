# Quantitative Risk Management: Monte Carlo VaR with Futures Hedging

This project implements a Monte Carlo-based Value-at-Risk (VaR) model for a portfolio of S&P 500 stocks, with systematic risk hedged using index futures. It showcases quantitative risk management techniques commonly used in professional trading and portfolio risk analysis.

##  Overview

- **Goal**: Estimate portfolio risk using Monte Carlo simulation and reduce exposure to market movements via hedging.
- **Approach**: 
  - Generate future price paths for each stock using historical data and stochastic modeling.
  - Compute portfolio returns and simulate risk metrics.
  - Hedge systematic risk using S&P 500 index futures.
  - Evaluate the effectiveness of the hedge.

##  Methodology

- **VaR Estimation**: Monte Carlo simulation based on multivariate normal or empirical return distributions.
- **Hedging**: Use of beta exposure to compute the optimal hedge ratio with S&P 500 index futures.
- **Pricing & Returns**: Returns modeled via log-normal distribution; scenarios are simulated to estimate the tail loss.
- **Backtesting (optional)**: Performance of the hedged portfolio can be tested over historical periods.

##  Technologies

- `Python`
- `Pandas`, `NumPy` – data manipulation and simulation
- `Matplotlib`, `Seaborn` – visualization
- `yfinance` or `pandas_datareader` – data acquisition
- `scikit-learn` (optional) – factor modeling or regression for beta estimation

##  How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/quant-risk-management.git
   cd quant-risk-management
