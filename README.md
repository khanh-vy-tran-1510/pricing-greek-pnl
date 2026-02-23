# Equity Derivatives: Pricing, Greeks, and PnL Analysis
## Overview

This project is a hands-on exploration of equity options pricing, Greeks calculation, delta hedging, and PnL decomposition, implemented in Python. It is designed to replicate the workflow of an equity derivatives desk while also illustrating the analytical methods used by quantitative researchers.

The repo contains two main notebooks:
- Version 1 — Black-Scholes & Greeks
- Version 2+3 — Delta Hedging & PnL Decomposition

## Notebook descriptions

### Version 1 - Black-Scholes & Greeks

- Implements the Black-Scholes pricing formula for European calls and puts.
- Calculates the main Greeks: Delta, Gamma, Theta, Vega, and Rho.
- Simulates basic price paths of the underlying stock.
- Visualizes Greeks as a function of strikes and option type.
- Provides insights into sensitivity and risk near expiration.

**Key Insights**:
- Delta measures sensitivity to the underlying.
- Gamma spikes near expiration → hedging becomes unstable.
- Theta represents time decay, showing the “cost” of holding options.
- Rho shows sensitivity to interest rates (small for equity options).

### Version 2 — Delta Hedging & PnL Decomposition

- Implements discrete delta hedging for short options.
- Tracks PnL over time, decomposed into:
  - Delta contribution
  - Gamma contribution
  - Theta contribution
- Simulates multiple paths to study hedging variability.
- Visualizes contributions using cumulative PnL plots and waterfall charts.
- Explores hedging errors, stress tests (volatility shocks), and risk concentration.

**Key Insights**:
- Delta hedging reduces first-order risk but leaves second-order (Gamma) exposure.
- Short calls collect Theta but pay Gamma → losses if stock moves strongly.
- Hedging frequency impacts PnL stability.
- Stress-testing with volatility or maturity shifts highlights potential model risk.

## Potential Extensions
- Monte Carlo Greeks for pathwise derivatives
- Stochastic volatility modeling (Heston model)
- Volatility surface calibration
- Multi-option portfolio hedging

## References
- Hull, J. Options, Futures, and Other Derivatives, 11th Edition
- Black, F. & Scholes, M. (1973) The Pricing of Options and Corporate Liabilities
- Wilmott, P. Paul Wilmott on Quantitative Finance
