<!-- ══════════════════════════════════════════════════════════ -->
<!--                                                              -->
<!--   📊  S T O C K   M A R K E T   A N A L Y S I S              -->
<!--       Five years · 491 companies · one Power BI report      -->
<!--                                                              -->
<!-- ══════════════════════════════════════════════════════════ -->

<h1 align="center">📈 Stock Market Analysis — Power BI</h1>

<p align="center">
  <em>Five years of daily market data across 491 global companies,<br/>
  turned into an interactive 8-page story about risk, return, and timing.</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-Desktop-6C4AB6?style=for-the-badge&logo=powerbi&logoColor=white"/>
  <img src="https://img.shields.io/badge/DAX-41%20measures-1D9E75?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Dashboards-8%20pages-6C4AB6?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Data-Kaggle-1D9E75?style=for-the-badge"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Companies-491-6C4AB6?style=flat-square"/>
  <img src="https://img.shields.io/badge/Trading%20days-1%2C258-1D9E75?style=flat-square"/>
  <img src="https://img.shields.io/badge/Shares%20traded-3.55T-6C4AB6?style=flat-square"/>
  <img src="https://img.shields.io/badge/Sectors-11-1D9E75?style=flat-square"/>
</p>

---

## 🟣 The one-line pitch

> I took a raw Kaggle dataset of daily stock prices and built the whole analytical workflow end to end — cleaning, modelling, 41 custom DAX measures, and 8 interactive dashboards covering everything from **sector performance** to **Sharpe ratios**, **drawdown**, and **Value at Risk**.

---

## 🟢 What the data actually said

Three findings that surprised me — and might surprise you too:

| 🟣 Finding | 🟢 What it means |
|-----------|------------------|
| **Energy beat tech** | Over the full 5 years, Energy was the *best-performing sector* (530% avg return), not Technology. The 2022 oil surge did the heavy lifting. |
| **Winning stocks still crashed** | Every stock that returned **3,000%+** also fell **more than 95%** from its peak. MRNA returned 3,752% *and* dropped 97.5%. Timing was everything. |
| **Volume ≠ returns** | The correlation between trading volume and returns was just **0.29**. The most talked-about stocks were rarely the best performers. |

---

## 🟣 The 8 dashboards

| # | Page | What it answers |
|:-:|------|-----------------|
| 1 | **📊 Market Overview** | The executive snapshot — headline KPIs and top performers |
| 2 | **🔍 Stock Deep-Dive** | Full OHLCV history and moving averages for any single stock |
| 3 | **⚖️ Performance Comparison** | Risk vs return across multiple stocks side by side |
| 4 | **💧 Volume & Liquidity** | Trading activity and intraday spread analysis |
| 5 | **💰 Dividends & Corporate Actions** | Income and split history |
| 6 | **🏭 Sector Analysis** | 11 GICS sectors ranked by performance and risk |
| 7 | **🛡️ Risk Dashboard** | Sharpe ratio, drawdown, and Value at Risk |
| 8 | **📅 Time Series & Events** | Price history mapped to COVID, rate hikes, and the AI boom |

---

## 🟢 Under the hood

<table>
<tr>
<td width="50%" valign="top">

### 🟣 Data model
- **6 tables** in a star schema
- **489-ticker** hand-built sector map
- **Market Events** table (6 macro periods)
- **Company Stats** table for risk categories
- **3 relationships**, fully interactive

</td>
<td width="50%" valign="top">

### 🟢 41 DAX measures across 13 folders
- Price, performance, volume, dividends
- Sector aggregation
- Moving averages (20 / 50 / 200-day)
- Drawdown & peak-to-trough
- Sharpe ratio & risk-adjusted return
- **Value at Risk (95% & 99%)**
- Pearson correlation (native DAX)

</td>
</tr>
</table>

---

## 🟣 Skills demonstrated

`Data modelling` &nbsp;•&nbsp; `Star schema design` &nbsp;•&nbsp; `Advanced DAX` &nbsp;•&nbsp; `Statistical measures` &nbsp;•&nbsp; `Financial risk metrics` &nbsp;•&nbsp; `Time intelligence` &nbsp;•&nbsp; `Report UX design` &nbsp;•&nbsp; `Data storytelling`

The tricky part wasn't the charts — it was writing DAX that computes **Pearson correlation**, **Sharpe ratios**, and **historical Value at Risk** natively inside the model, and debugging engine-level limitations along the way.

---

## 🟢 Repository contents

```
📁 stock-market-analysis-powerbi
├── 📊 Stock_Market_Analysis.pbix          ← the Power BI report
├── 📄 Stock_Market_Analysis_Report.docx   ← written analysis (10 sections)
├── 📁 screenshots/                         ← dashboard previews
│   ├── 01-market-overview.png
│   ├── 07-risk-dashboard.png
│   └── ...
└── 📄 README.md                            ← you are here
```

> **Note on the dataset:** the source data comes from the [Massive Yahoo Finance Dataset](https://www.kaggle.com/datasets/iveeaten3223times/massive-yahoo-finance-dataset) on Kaggle. If the `.pbix` exceeds GitHub's 100 MB limit, load the CSV into Power BI Desktop via *Get Data → Text/CSV*.

---

## 🟣 Future enhancements

Things I'd add with more time — and know how to approach:

- 📉 **Value at Risk backtesting** — validate the VaR estimates against realised losses
- 🎲 **Monte Carlo simulation** — probabilistic price paths (via Python visual)
- 📊 **Beta vs S&P 500** — market-relative volatility (needs an index benchmark)
- 🔥 **Correlation heatmap** — stock-to-stock diversification analysis
- 🔮 **ARIMA / Prophet forecasting** — proper time-series modelling that handles market-day gaps

---

<p align="center">
  <br/>
  <strong>🟣🟢 Built with curiosity, caffeine, and a lot of DAX debugging. 🟢🟣</strong>
  <br/><br/>
  <em>Data: <a href="https://www.kaggle.com/datasets/iveeaten3223times/massive-yahoo-finance-dataset">Massive Yahoo Finance Dataset (Kaggle)</a> · Tool: Power BI Desktop · Period: Nov 2018 – Nov 2023</em>
</p>
