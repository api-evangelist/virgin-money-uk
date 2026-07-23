---
name: Locate Virgin Money ATMs and branches (Open Data)
description: >-
  Retrieve Virgin Money / Clydesdale / Yorkshire ATM and branch locations and
  product data from the public, unauthenticated OBIE Open Data API — no token,
  consent, or certificate required.
api: openapi/obie-opendata-api-standard-openapi.json
operations:
  - "GET /branches"
  - "GET /atms"
  - "GET /personal-current-accounts"
  - "GET /business-current-accounts"
  - "GET /unsecured-sme-loans"
  - "GET /commercial-credit-cards"
method: generated
source: openapi/obie-opendata-api-standard-openapi.json
---

# Locate Virgin Money ATMs and branches (Open Data)

The Open Data API is **public and unauthenticated** — it follows the OBIE Open
Data Standard and requires no OAuth token, consent, or Open Banking certificate.
This is distinct from the authenticated Read/Write (AIS/PIS/CBPII) APIs.

## Steps

1. **List branches** — `GET /branches`. Returns Brand > Branch hierarchy with
   address, geolocation, services, accessibility, and opening hours. Supports
   conditional requests via `If-Modified-Since` / `If-None-Match`.
2. **List ATMs** — `GET /atms`. Returns ATM locations, features (contactless,
   audio guidance, wheelchair access), and supported currencies.
3. **List products** as needed — `GET /personal-current-accounts`,
   `GET /business-current-accounts`, `GET /unsecured-sme-loans`,
   `GET /commercial-credit-cards` for product terms, eligibility, and pricing.
4. **Filter client-side.** These endpoints return full datasets; apply
   geospatial or attribute filtering after retrieval.

## Rules

- **No auth.** Do not send an Authorization header or attempt SCA for these
  operations.
- **Caching.** Honour `Etag` / `Last-Modified` and use `If-None-Match` /
  `If-Modified-Since` to avoid re-fetching unchanged datasets.
- **Rate limits.** A `429 Too Many Requests` means back off and retry later
  (see conventions/virgin-money-uk-conventions.yml).
- **Errors.** Failures surface the OBIE `OBError` envelope; see
  errors/virgin-money-uk-problem-types.yml.
- **Endpoint caveat.** The legacy CYBG open-data base URL returned 404 on probe
  (2026-07-23); resolve the current-brand base path from the developer portal
  before calling.
