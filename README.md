# 📊 BloomFree Terminal

> A Bloomberg-inspired financial terminal — built with pure HTML, CSS, and JavaScript. Live stocks, crypto, forex, and news. No backend, no subscription, no install.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?style=flat-square&logo=javascript)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=flat-square&logo=chart.js&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)

---

## What Is It?

A free, browser-only recreation of a Bloomberg Terminal — dark amber/green/red theme, JetBrains Mono typography, multi-panel layout, and live market data pulled from three free public APIs. Open `index.html` and you're trading-desk-ready in seconds.

---

## Features

### 🖥️ Dashboard (F1)
- Live scrolling price ticker
- 8 major market indices — S&P 500, NASDAQ, DOW, VIX, BTC, Gold, Crude Oil, USD Index
- 12-stock watchlist (AAPL, MSFT, NVDA, GOOGL, AMZN, META, TSLA, JPM, V, JNJ, WMT, BAC) with sparklines
- Live price chart with Open/High/Low/Prev stats and 1D/1W/1M/3M timeframes
- Top Movers — Gainers & Losers
- Options chain — Calls & Puts with Strike, Bid, Ask, IV, OI
- Economic calendar with impact levels
- News feed tagged BULLISH / BEARISH

### 📈 Charts (F2)
Full-screen expanded chart view for deeper technical analysis.

### 💼 Portfolio (F3)
Holdings table with P&L, market value, and weight — plus a doughnut allocation chart and summary stats (Total Value, Day P&L, Total P&L, Beta, Sharpe Ratio).

### ₿ Crypto (F4)
Full crypto market table (BTC, ETH, SOL, BNB, XRP, DOGE, ADA, AVAX), Fear & Greed Index gauge, and market dominance chart.

### 💱 FX (F5)
12 live currency pairs (EUR/USD, GBP/USD, USD/JPY, USD/INR, and more) with direction indicators.

### 🌍 Also Included
- India Market Dashboard
- Multi-timezone world clocks

---

## Tech Stack

| Tech | Purpose |
|------|---------|
| HTML / CSS / JavaScript | No frameworks, no build step |
| Chart.js | Price charts, doughnut allocation, dominance charts |
| [Finnhub API](https://finnhub.io) | Live US stock quotes |
| [CoinGecko API](https://www.coingecko.com/api) | Crypto prices (free, no key) |
| [Frankfurter API](https://www.frankfurter.app) | Live FX rates (free, no key) |

---

## Run Locally

No install. No build step. No server required.

```bash
git clone https://github.com/kulatshreeram/-BloomFree-Terminal.git
cd -BloomFree-Terminal
```

Just double-click `index.html` — or open it in any browser.

---

## ⚠️ Before You Deploy

`realtime.js` currently contains a hardcoded Finnhub API key. If you're publishing this publicly or pushing to a live site:
- Replace it with your own free key from [finnhub.io](https://finnhub.io)
- Better yet, load it from an environment variable or a config file excluded via `.gitignore`

---

## Why This Project?

Built to learn how real financial dashboards work — live data fetching, API throttling/caching, real-time UI updates, and Bloomberg-style data density — using nothing but vanilla web tech.

---

## Roadmap

- [ ] Live NSE/BSE data for Indian markets
- [ ] WebSocket streaming (replace polling)
- [ ] Custom, persisted watchlists
- [ ] Full portfolio management (add/remove holdings)

---

## License

MIT © [kulatshreeram](https://github.com/kulatshreeram)

⭐ If you like the project, consider giving it a star.
