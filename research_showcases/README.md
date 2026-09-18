# 🏛️ INSTITUTIONAL QUANTITATIVE RESEARCH SHOWCASES
## Research Architecture by Prince Chauhan (SEBI Registered Research Analyst)

This directory houses **7 self-contained, reproducible quantitative research showcases** designed to substantiate the empirical, mathematical, and algorithmic claims featured on Prince Chauhan's Quantitative Researcher CV:

```
research_showcases/
├── point_in_time_backtester/          → Event-driven chronological simulation & 0.50% turnover friction
├── options_volatility_surface/        → Black-Scholes inversion, cubic spline/SVI fitting & Greeks
├── banknifty_cointegration/           → Johansen cointegration rank test & dynamic beta stat arb
├── regime_allocation/                 → Unsupervised K-Means vol regime gating (28% DD reduction)
├── execution_simulator/               → Order book queue priority, slippage & 1.8 bps cost attribution
├── institutional_tearsheet_generator/ → 6x2 KPI Scorecard, monthly heatmap grid & ReportLab PDF engine
└── strategy_validator_gate/           → 11-stage audit gate, 2x friction stress & Monte Carlo DD cones
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
| **06** | **[Tear Sheet Generator](./institutional_tearsheet_generator/)** | 6x2 KPI Scorecard, 8-year monthly returns heatmap grid, peak-to-trough underwater drawdown dynamics. | Publication-grade PDF report engine for Executive CRO & Investment Committee review. | `python -m unittest research_showcases.institutional_tearsheet_generator.test_tearsheet_builder` |
| **07** | **[Strategy Validator Gate](./strategy_validator_gate/)** | 11-stage production audit gate (Rules L1–L22), trade boundary clamping ($\le 15:14:59$). | 2x turnover friction stress test and Monte Carlo drawdown cones (1,000 paths). | `python -m unittest research_showcases.strategy_validator_gate.test_validator_gate` |

---

## 🧪 Quick Test All Showcases

Run the unified test suite across all 7 research showcases:

```powershell
python -m unittest discover research_showcases
```

All 7 projects are **100% self-contained**, have zero live broker dependencies, and run cross-platform on Windows and Linux/macOS.
