# London SMC Signals

Educational Forex website focused exclusively on **Smart Money Concepts (SMC)** for the **London session**.

## Features

- **Live London clock** + session status + Kill Zone countdown
- **Live reference rates** via free Frankfurter API (no key required) + CDN fallback
- Clear 4-step London SMC playbook (Asian range → liquidity sweep → structure confirmation → entry)
- Interactive **Signal Checklist** tool – input your levels and get a disciplined assessment
- Core SMC concepts glossary
- Embedded TradingView charts (EURUSD, GBPUSD, USDJPY, GBPJPY, XAUUSD)
- Dark, modern UI

## Connected APIs

| API | Purpose | Auth | Notes |
|-----|---------|------|-------|
| [Frankfurter](https://frankfurter.dev) | Daily mid rates for majors | None | Primary source, central-bank blended |
| fawazahmed0 currency-api (jsDelivr) | Fallback rates | None | Used if Frankfurter fails |
| TradingView Widget | Live charts | None | Browser embed |

For true real-time ticks or historical OHLC (needed for automatic Asian-range detection), a free key from [Twelve Data](https://twelvedata.com) (800 calls/day) or similar can be added next.

## How to use

1. Open `index.html` in any modern browser (Chrome, Firefox, Edge, Safari).
2. No build step or server required – it is a single self-contained file.
3. For best experience, mark Asian High/Low on the chart first, then use the Signal Tool.

## Important

This is an **educational tool only**. It does not generate automated real-time signals or place trades. Always perform your own analysis and risk management.

## Local preview (optional)

If you want a local server:

```bash
# Python
python3 -m http.server 8080

# or Node
npx serve .
```

Then open http://localhost:8080
