# Sparse Index Tracking Portfolio

This project explores methods to construct a **sparse portfolio**  
(e.g. 10–20 stocks) that tracks a benchmark index such as the S&P 500.  
The goal is to balance **tracking accuracy**, **sparsity**, and **practical constraints**.

---

## Motivation
Most equity indices (like the S&P 500) are dominated by a handful of mega-cap names.  
Replicating the index with a small number of stocks is challenging, but useful for:
- Lower transaction costs and turnover
- More interpretable portfolios
- Educational and research purposes

---

## Features
- Data pipeline using `yfinance` for index constituents and returns  
- Optimization methods:
  - Lasso / Elastic Net regression
  - Greedy forward selection
  - Mixed-Integer Quadratic Programming (cardinality constraints)
  - Factor-based tracking (PCA, Fama–French style factors)
- Constraints:
  - Long-only, weight caps, sector caps
  - Turnover and transaction cost penalties
- Evaluation:
  - In-sample vs out-of-sample tracking error
  - Turnover analysis
  - Factor exposure matching
  - Visualizations of portfolio composition and benchmark comparison

---

## Project Structure
