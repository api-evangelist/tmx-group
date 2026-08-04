# TMX Group (tmx-group)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
