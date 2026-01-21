# Static Equally-Weighted Risk Contributions (EWRC) Portfolio Analysis

This project compares a static Equal Weight Risk Contribution (EWRC) portfolio against the Golden Butterfly (GB) portfolio to evaluate whether risk parity improves diversification and risk-adjusted returns.

## Key Features
- **Assets**: 5-asset portfolio (GLD, IEF, VTI, VIOV, VGLT)  
- **Sample Period**: January 2013 – October 2025  
- **Strategies Compared**:  
  - **EWRC**: Weights assets so each contributes equally (~20%) to total portfolio risk  
  - **Golden Butterfly**: Equal-weighted (20% each asset) benchmark portfolio  
- **Rebalancing**: Static weights (no rebalancing)  

## Performance Summary

**Portfolio Metrics**
| Metric | EWRC | Golden Butterfly |
|--------|------|------------------|
| **CAGR** | 5.85% | 7.40% |
| **Volatility** | 7.45% | 8.84% |
| **Sharpe Ratio** | 0.54 | 0.63 |
| **Sortino Ratio** | 0.71 | 0.81 |
| **Max Drawdown** | -20.9% | -21.1% |

**Asset Sharpe Ratios (2013-2025)**
| Ticker | Sharpe Ratio |
|--------|--------------|
| VTI | 0.75 |
| VIOV | 0.46 |
| GLD | 0.32 |
| IEF | -0.023 |
| VGLT | -0.012 |

## Key Findings

- **EWRC**: 55% bonds, 28% equities → balanced risk (~20% per asset)
- **Golden Butterfly**: 20% each asset → 66% risk from equities

**Main Result**: EWRC successfully balanced risk but underperformed (5.85% vs 7.40% CAGR) due to overweighting bonds with negative Sharpe ratios.

## Files Included
- `Risk Parity.ipynb`: Notebook with code and analysis  
- `Risk Parity presentation.pdf`: Final report with detailed findings  
- `data/`: Contains price data for 5 assets  

## Tools Used
- Python  
- pandas, numpy  
- matplotlib, seaborn  

## How to Run
Open the notebook using **Jupyter Notebook** or **VS Code**.  
Ensure that the asset price data is available.  

## References

1. Qian, Edward. "Risk Parity and Diversification." *Journal of Investing*, vol. 20, no. 1, Spring 2011, pp. 119–127.
2. Sharpe, William F. "Capital Asset Prices: A Theory of Market Equilibrium under Conditions of Risk." *The Journal of Finance*, vol. 19, no. 3, 1964, pp. 425–42.

---
**Author**: Safwan Khan  
*(MS in Quantitative Finance, Northeastern University)*  
**Course**: FINA 6238 – Fall 2025
