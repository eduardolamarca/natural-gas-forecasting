# ⛽ Natural Gas Consumption Forecasting

Time series forecasting of monthly natural gas consumption in the United
States, comparing additive and multiplicative **Holt-Winters** models.

*Developed as part of the MBA in Artificial Intelligence & Analytics Applied
to Business — FGV (Fundação Getulio Vargas).*

---

## 🎯 Objectives

1. Explore the long-term trend and monthly seasonality of consumption
2. Train additive and multiplicative Holt-Winters (exponential smoothing) models
3. Evaluate forecasts against actual data using MAPE, MAE and RMSE

---

## 📊 Methodology

| Step | Description |
|---|---|
| Data | FRED series `NATURALGAS`, monthly, billions of cubic feet (2000 onwards) |
| Exploration | Trend charts (plotnine, Plotly, seaborn) and monthly seasonality boxplot |
| Training set | January 2020 – December 2024 (60 months) |
| Test set | January 2025 onwards |
| Models | Holt-Winters additive and multiplicative, 12-month seasonality |
| Evaluation | MAPE, MAE, RMSE |

---

## 🛠️ Tech stack

Python · pandas · statsmodels · scikit-learn · Plotly · plotnine · seaborn ·
Jupyter · Docker (Dev Container)

---

## 📁 Project structure

```
natural-gas-forecasting/
│
├── .devcontainer/        ← reproducible development environment
├── data/                 ← dataset snapshot downloaded from FRED
├── notebooks/
│   └── natural_gas_forecast.ipynb
├── requirements.txt
└── README.md
```

---

## 🚀 How to run

**Option 1 — Dev Container (recommended):** open the folder in VS Code and
select "Reopen in Container". All dependencies are installed automatically.

**Option 2 — Local environment:**

```bash
git clone https://github.com/eduardolamarca/natural-gas-forecasting.git
cd natural-gas-forecasting
pip install -r requirements.txt
jupyter notebook
```

Then open `notebooks/natural_gas_forecast.ipynb` and run all cells.
The data is downloaded directly from FRED, so an internet connection is required.

---

## 📂 Data source

Federal Reserve Bank of St. Louis —
[FRED: Natural Gas Consumption (NATURALGAS)](https://fred.stlouisfed.org/series/NATURALGAS)

---

*Project by [Eduardo Lamarca](https://www.linkedin.com/in/eduardolamarca/)
— Data Analyst open to opportunities in Europe 🇪🇺*
