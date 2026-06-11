# Time-Series-Forecasting-in-R
Coursework from the university module Time Series - an applied forecasting project in R using the fpp3 framework, taking a real retail time series through the full pipeline from exploratory analysis to validated out-of-sample forecasts.

# Overview
 
This module applies the modern tidy forecasting workflow (`fpp3` / `fable`, the framework from Hyndman & Athanasopoulos' *Forecasting: Principles and Practice*) to a real economic time series: **monthly retail turnover for Liquor Retailing in New South Wales, Australia (1982–2022)**, sourced from the Australian Bureau of Statistics.
 
The work moves from data exploration through model building, validation, and a critical comparison of forecasts against actual subsequently-released data — including a discussion of how the COVID-19 structural break affects the models.

# Contents
 
**Assignments** (`assignments/`)
 
1. **Exploratory analysis** — visualizing the series (`autoplot`, `gg_season`, `gg_subseries`), identifying trend, seasonality and heteroscedasticity, choosing a Box-Cox transformation (Guerrero method), and STL decomposition.
2. **ETS vs. benchmarks & cross-validation** — fitting an automatic ETS model against Mean, Naïve and Seasonal-Naïve baselines; residual diagnostics (ACF, Ljung-Box); and time-series cross-validation, with a discussion of why CV is the more reliable accuracy estimate.
3. **ARIMA model selection** — unit-root testing (KPSS), determining the required differencing, reading ACF/PACF plots to propose candidate models, and comparing manual specifications against an auto-selected ARIMA by AICc and test-set RMSE.


**Project** (`project/`)
 
A complete forecasting study answering 12 structured questions: Box-Cox transformation, STL decomposition, stationarity testing, building a short-list of ETS and ARIMA candidates, model comparison via AICc and a 24-month test set, residual diagnostics (Ljung-Box), out-of-sample point forecasts with 80% prediction intervals, **back-testing the forecasts against newly-released ABS data**, and a discussion of model benefits, limitations, and a proposed annual re-forecasting process.

# Key techniques
 
Box-Cox transformation · STL decomposition · ETS (exponential smoothing) · ARIMA / seasonal ARIMA · unit-root tests (KPSS) · ACF/PACF identification · AICc model selection · time-series cross-validation · residual diagnostics (Ljung-Box) · prediction intervals · forecast back-testing

# Note
 
Academic coursework, shared as part of my data-analysis portfolio.
