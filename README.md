# ST Trading AI Bot — Web Frontend

Mobile-first production interface for ST Trading AI Bot.

## Run locally

Open `index.html` in a browser, or run any static web server in this directory.

## Backend contract

The analyzer sends `POST /api/analyze` with:

```json
{ "pair": "EUR/USD", "timeframe": "1m" }
```

Expected response:

```json
{ "direction": "UP", "confidence": 87 }
```

The frontend never generates a random trading signal. Authentication, quotas, activation codes, market feeds and AI analysis must be enforced by the secure backend.
