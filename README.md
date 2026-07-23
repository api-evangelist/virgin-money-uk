# Virgin Money UK (virgin-money-uk)

Virgin Money UK is a full-service UK retail and business bank operating the Virgin Money, Clydesdale Bank, Yorkshire Bank, and B brands. Formerly the FTSE-listed Virgin Money UK PLC (the former CYBG plc), it was acquired by Nationwide Building Society on 1 October 2024 and its banking business is scheduled to transfer into Nationwide on 2 April 2026. It is authorised by the PRA and regulated by the FCA and PRA as an ASPSP, and is a fully participating UK Open Banking provider under PSD2 (it is not one of the original CMA9).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/virgin-money-uk/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/virgin-money-uk/refs/heads/main/apis.yml)

## Tags

- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- FAPI

## Timestamps

- **Created:** 2026-07-23
- **Modified:** 2026-07-23

## APIs

Virgin Money UK publishes UK Open Banking (OBIE) APIs through its developer portal at [developer.virginmoney.com](https://developer.virginmoney.com/), split into two families:

- **Merged APIs** — Virgin Money, Clydesdale and Yorkshire accounts (sort codes 05 / 82, 10-digit customer numbers) and business credit cards.
- **Standalone APIs** — personal credit cards and current/savings accounts (sort code 08, 7-digit alphanumeric customer numbers).

### Open Data API (Public)

Unauthenticated OBIE Open Data surface — ATM Locator, Branch Locator, Personal & Business Current Accounts, Unsecured SME Loans, and Commercial Credit Cards — represented against the shared OBIE Open Data Standard. The legacy CYBG base URL from the OBIE participant registry (`https://api-ib.cybservices.co.uk/ibapi/v2/banks/CB/open-banking`) returned HTTP 404 on probe (2026-07-23); the live current-brand endpoint is unverified.

- **Human URL:** [https://developer.virginmoney.com/](https://developer.virginmoney.com/)
- **Standard spec:** [openapi/obie-opendata-api-standard-openapi.json](openapi/obie-opendata-api-standard-openapi.json) (shared OBIE Open Data Standard, not a bank-proprietary contract)

### Read/Write APIs (OBIE, FAPI-secured)

The OBIE Read/Write Standard family, secured with FAPI OAuth2/OpenID Connect, mutual-TLS client authentication, and PSD2 strong customer authentication:

- **Account & Transaction Information (AIS)** — Merged v3.1.2 and Standalone v3.1.1 — [merged accounts](https://developer.virginmoney.com/merged/accounts/) · [standalone](https://developer.virginmoney.com/standalone/account-and-transaction/)
- **Payment Initiation (PIS)** — Domestic Immediate ([dip](https://developer.virginmoney.com/merged/dip/)), Domestic Scheduled ([dsp](https://developer.virginmoney.com/merged/dsp/)), File Payments ([file-payments](https://developer.virginmoney.com/merged/file-payments/)), International ([ip](https://developer.virginmoney.com/merged/ip/)), International Scheduled ([isp](https://developer.virginmoney.com/merged/isp/)) — v3.1.2
- **Confirmation of Funds (CBPII)** — [cof](https://developer.virginmoney.com/merged/cof/) — v3.1.2

### Security & Onboarding APIs

- **OIDC API** — Open Banking-compliant OpenID Connect provider. Live production discovery document confirmed (HTTP 200, 2026-07-23): [.well-known/openid-configuration](https://api.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/.well-known/openid-configuration)
- **Token API** — OAuth2 token endpoint (v3.0)
- **Dynamic Client Registration API** — TPP registration with OBIE (OBWAC/OBSeal) or eIDAS (QWAC/QSEAL) certificates (v3.2)

## Common Properties

- [Website](https://uk.virginmoney.com/)
- [Developer Portal](https://developer.virginmoney.com/)
- [Documentation](https://developer.virginmoney.com/merged/)
- [Support](https://uk.virginmoney.com/support/)
- [Terms of Service](https://uk.virginmoney.com/terms/)
- [Privacy Policy](https://uk.virginmoney.com/privacy/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
