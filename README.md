# BTC Pref Flywheel — Amplification Hurdle Rate

An interactive visualization tool for understanding the dynamics of Bitcoin-treasury companies' preferred stock issuance and leverage sustainability.

## What This Tool Does

This model helps answer the question: **How hard does Strategy have to press the accelerator to actually increase leverage?**

Given assumptions about:
- Bitcoin price appreciation (CAGR)
- BTC stack growth (acquisitions via equity issuance)
- Current amplification ratio (Pref + Debt / BTC NAV)

The tool calculates the **maximum preferred stock issuance** that can occur without increasing the amplification ratio — the "hurdle rate."

## Features

- **Live Data**: Fetches real-time data from Strategy's public APIs (BTC holdings, NAV, pref/debt notional, mNAV)
- **ATH Reference**: Shows distance from Bitcoin all-time high to contextualize appreciation assumptions
- **Debt Retirement Scenarios**: Toggle convertible bonds to model retirement and see impact on amplification
- **Preferred Shares ATM Runway**: Estimates years until shareholder vote needed based on ATM authorization limits
- **Mobile Responsive**: Works on desktop and mobile devices

## Key Concepts

- **Amplification**: (Pref Notional + Debt Notional) / BTC NAV — measures leverage
- **Hurdle Rate**: The dollar amount of prefs that can be issued annually while maintaining current amplification
- **mNAV**: Enterprise Value / BTC NAV — determines if equity channel is open (mNAV ≥ 1)

## Deployment

### Vercel (Recommended)
1. Push to GitHub
2. Connect repo to Vercel
3. Deploy (no build step needed — it's a static HTML file)

### Local
Simply open `index.html` in a browser. Note: Live data fetch requires CORS-enabled API access.

## Data Sources

- [Strategy Bitcoin KPIs API](https://api.strategy.com/btc/bitcoinKpis)
- [Strategy MSTR KPI Data API](https://api.strategy.com/btc/mstrKpiData)

## Disclaimer

**NFA (Not Financial Advice)**. This tool is for educational and informational purposes only. Do your own research.

## Author

Built by [@docstacks](https://x.com/docstacks) on X

---

*Based on the "BTC Pref Flywheel" model for analyzing preferred capital structures in Bitcoin-treasury companies.*

