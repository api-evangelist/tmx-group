# TMX Group (tmx-group)

TMX Group operates Canadian capital-markets infrastructure - Toronto Stock Exchange, TSX Venture Exchange, TSX Alpha, and the Montreal Exchange - and sells market data through its TMX Datalinx arm. Alongside sales-gated real-time broadcast feeds (TL1/TL2, QuantumFeed, MX Order Book Feed) it offers a self-serve TMX Analytics platform (hub.tmxanalytics.com) whose REST Data Science APIs deliver Canadian and US equity daily stats, intraday trade/quote bars, TAQ NBBO tick data, broker analytics, short interest, buybacks, corporate actions and reference data, and Montreal Exchange options and futures analytics, plus cloud/S3 flat-file and notebook delivery.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tmx-group/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tmx-group/refs/heads/main/apis.yml)

## Tags

- Financial
- Market Data
- Stocks
- Exchange
- Derivatives
- Analytics
- Reference Data
- Canada

## Timestamps

- **Created:** 2026-07-21
- **Modified:** 2026-07-21

## APIs

### TMX Essential Analytics for Equities API

End-of-day equity analytics for Canadian and US markets - basic, daily, and advanced daily stats plus liquidity analytics and liquidity summaries - via POST endpoints such as /v1/ca/dailystats, /v1/us/advanceddailystats, and /v1/ca/liquidityanalytics returning JSON (T-1 data by 6:30am ET).

- **Human URL:** [https://docs.tmxanalytics.com/#prod-tmx-ds-api-essential-analytics-for-equities](https://docs.tmxanalytics.com/#prod-tmx-ds-api-essential-analytics-for-equities)
- **Base URL:** `https://analyticsapi.tmxanalytics.com/v1`

### TMX Equity Intraday Trades and Quotes API

One-minute and one-second trade and quote bars for Canadian and US equities via /v1/ca/tradebar1min, /v1/ca/tradebar1sec, /v1/ca/quotesbar1min, /v1/ca/quotesbar1sec and US equivalents.

- **Human URL:** [https://docs.tmxanalytics.com/#prod-tmx-ds-api-equity-intraday-trades](https://docs.tmxanalytics.com/#prod-tmx-ds-api-equity-intraday-trades)
- **Base URL:** `https://analyticsapi.tmxanalytics.com/v1`

### TMX Trades and Quotes Tick Data (TAQ NBBO) API

Historical trade-and-quote tick data with national best bid and offer for Canadian and US listings via /v1/ca/taqnbbo and /v1/us/taqnbbo.

- **Human URL:** [https://docs.tmxanalytics.com/#prod-tmx-ds-api-trades-and-quotes-tick-data](https://docs.tmxanalytics.com/#prod-tmx-ds-api-trades-and-quotes-tick-data)
- **Base URL:** `https://analyticsapi.tmxanalytics.com/v1`

### TMX Broker Analytics API

Broker-level trading activity for Canadian markets - broker daily stats, broker liquidity, and broker summaries - via /v1/ca/brokerdailystats, /v1/ca/brokerliquidity, and /v1/ca/brokersummary, with GET-based V2 equivalents on the Insight API.

- **Human URL:** [https://docs.tmxanalytics.com/#prod-tmx-ds-api-broker-analytics](https://docs.tmxanalytics.com/#prod-tmx-ds-api-broker-analytics)
- **Base URL:** `https://analyticsapi.tmxanalytics.com/v1`

### TMX Corporate Actions and Reference Data API

Issuer profiles, global symbol directories and deltas, and global corporate actions via /v1/ca/issuers, /v1/globalsymbols, and /v1/globalsymbolsdelta, with V2 additions covering TSX reference data (CRV bulletins, entitlements, FITC, SMF) and S&P/TSX index data (/v2/sptsx/sdc, sde, sdl).

- **Human URL:** [https://docs.tmxanalytics.com/#prod-tmx-ds-api-corporate-actions-and-reference-data](https://docs.tmxanalytics.com/#prod-tmx-ds-api-corporate-actions-and-reference-data)
- **Base URL:** `https://analyticsapi.tmxanalytics.com/v1`

### TMX Options and Futures Analytics API

Montreal Exchange derivatives analytics - MX daily stats for options and futures via /v1/ca/mxdailystats, with instrument, order book, and trade datasets documented alongside.

- **Human URL:** [https://docs.tmxanalytics.com/#prod-tmx-ds-api-essential-analytics-for-options-and-futures](https://docs.tmxanalytics.com/#prod-tmx-ds-api-essential-analytics-for-options-and-futures)
- **Base URL:** `https://analyticsapi.tmxanalytics.com/v1`

### TMX Short Interest Analytics API

Short interest analytics for Canadian listings including days to cover (/v1/daystocover) and percent of float (/v1/percentfloat).

- **Human URL:** [https://docs.tmxanalytics.com/#prod-tmx-ds-api-short-interest-analytics](https://docs.tmxanalytics.com/#prod-tmx-ds-api-short-interest-analytics)
- **Base URL:** `https://analyticsapi.tmxanalytics.com/v1`

### TMX Buybacks API

North American share buyback activity via /v1/northamericanbuybacks.

- **Human URL:** [https://docs.tmxanalytics.com/#prod-tmx-ds-api-buybacks](https://docs.tmxanalytics.com/#prod-tmx-ds-api-buybacks)
- **Base URL:** `https://analyticsapi.tmxanalytics.com/v1`

### TMX Price Adjustment Curve API

Price adjustment curves for historical price series via /v1/pac, /v1/pacexplain, /v1/original, and /v1/smoothened.

- **Human URL:** [https://docs.tmxanalytics.com/#prod-tmx-ds-api-price-adjustment-curve](https://docs.tmxanalytics.com/#prod-tmx-ds-api-price-adjustment-curve)
- **Base URL:** `https://analyticsapi.tmxanalytics.com/v1`

### TMX MOC Imbalance Analytics API

Market-on-close imbalance analytics for the Toronto Stock Exchange closing auction via /v1/ca/moci.

- **Human URL:** [https://docs.tmxanalytics.com/#prod-tmx-ds-api-new-moc-imbalance-analytics](https://docs.tmxanalytics.com/#prod-tmx-ds-api-new-moc-imbalance-analytics)
- **Base URL:** `https://analyticsapi.tmxanalytics.com/v1`

### TMX Data Science API V2 (Insight API)

Second-generation GET-based REST surface on insightapi.tmxanalytics.com/v2 covering broker analytics, issuers, global symbols, TSX reference data (CRV bulletins, entitlements, FITC, SMF), and S&P/TSX index datasets, authenticated with the same hub-issued API key and bearer token as V1.

- **Human URL:** [https://docs.tmxanalytics.com/#tmx-data-science-api-v2](https://docs.tmxanalytics.com/#tmx-data-science-api-v2)
- **Base URL:** `https://insightapi.tmxanalytics.com/v2`

## Common Properties

- [Website](https://www.tmx.com)
- [Portal](https://hub.tmxanalytics.com/)
- [Documentation](https://docs.tmxanalytics.com/)
- [GitHub Organization](https://github.com/TMXGroup)
- [LinkedIn](https://www.linkedin.com/company/tmx-group)
- [Blog](https://www.tmx.com/newsroom)
- [Pricing](https://www.tmxinfoservices.com/market-data/pricing-and-contract-documents)
- [Sign Up](https://hub.tmxanalytics.com/login)
- [Terms of Service](https://www.tmx.com/terms-of-use)
- [Privacy Policy](https://www.tmx.com/en/privacy-policy)
- [Support](https://docs.tmxanalytics.com/#tmx-api-support)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
