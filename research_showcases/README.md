# 🏛️ INSTITUTIONAL QUANTITATIVE RESEARCH SHOWCASES
## Research Architecture by Prince Chauhan (SEBI Registered Research Analyst)

This directory houses **5 self-contained, reproducible quantitative research showcases** designed to substantiate the empirical, mathematical, and algorithmic claims featured on Prince Chauhan's Quantitative Researcher CV:

```
research_showcases/
├── point_in_time_backtester/     → Event-driven chronological simulation & 0.50% turnover friction
├── options_volatility_surface/   → Black-Scholes inversion, cubic spline/SVI fitting & Greeks
├── banknifty_cointegration/      → Johansen cointegration rank test & dynamic beta stat arb
├── regime_allocation/            → Unsupervised K-Means vol regime gating (28% DD reduction)
└── execution_simulator/          → Order book queue priority, slippage & 1.8 bps cost attribution
```

---

## 🎯 Executive Showcase Summary Matrix

| # | Project Name | Mathematical / Empirical Framework | Invariants & Reality Controls | Runnable Test |
|---|---|---|---|---|
| **01** | **[Point-in-Time Backtester](./point_in_time_backtester/)** | Vectorized event-driven simulation, dynamic capital sizing $\lfloor \text{Capital}/\text{Margin} \rfloor$. | 0.50% turnover friction pre-deducted, 11-column canonical CSV ledger. | `python -m unittest research_showcases.point_in_time_backtester.test_backtester` |
| **02** | **[Options IV Surface & Greeks](./options_volatility_surface/)** | Black-Scholes inversion (Newton-Raphson/Brent), cubic spline & SVI strike smoothing, GEX profiles. | Total variance monotonic bounds ($\partial w / \partial k$), bad quote filtering. | `python -m unittest research_showcases.options_volatility_surface.test_surface_model` |
| **03** | **[Bank Nifty Cointegration](./banknifty_cointegration/)** | Johansen cointegration rank test, rolling OLS hedge ratios, Ornstein-Uhlenbeck spread half-life. | Strict stationarity verification (ADF p-value < 0.05), transaction cost drag. | `python -m unittest research_showcases.banknifty_cointegration.test_cointegration` |
| **04** | **[Market Regime Classifier](./regime_allocation/)** | Unsupervised K-Means / GMM on Parkinson RV, IV/RV ratios, and return skewness. | Dynamic short-gamma gating reducing simulated maximum DD by 28%. | `python -m unittest research_showcases.regime_allocation.test_regime_classifier` |
| **05** | **[Microstructure Simulator](./execution_simulator/)** | Limit vs. market order queue priority, square-root market impact $I \propto \sigma \sqrt{Q/V}$. | Quantitative attribution of 1.8 bps market-crossing savings via async IPC. | `python -m unittest research_showcases.execution_simulator.test_microstructure` |

---

## 🧪 Quick Test All Showcases

Run the unified test suite across all 5 research showcases:

```powershell
python -m unittest discover research_showcases
```

All 5 projects are **100% self-contained**, have zero live broker dependencies, and run cross-platform on Windows and macOS.
