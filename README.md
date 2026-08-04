# Virgin Money UK (virgin-money-uk)

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
