# Virgin Money UK

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Virgin Money UK is a full-service UK retail and business bank, operating the Virgin Money, Clydesdale Bank, Yorkshire Bank, and B brands across personal current and savings accounts, mortgages, credit cards, and business banking. Formerly the FTSE-listed Virgin Money UK PLC (the former CYBG plc), it was acquired by Nationwide Building Society on 1 October 2024, making it part of a mutually owned group; its banking business is scheduled to transfer into Nationwide on 2 April 2026. The bank is authorised by the Prudential Regulation Authority and regulated by the FCA and PRA as an ASPSP. It is not one of the original CMA9 but is a fully participating UK Open Banking provider under PSD2 and the Payment Services Regulations 2017, publishing OBIE Read/Write Standard APIs - Account & Transaction Information (AIS), Payment Initiation (PIS), and Confirmation of Funds (CBPII) - through its developer portal at developer.virginmoney.com, split into "Merged" APIs (Virgin Money, Clydesdale and Yorkshire accounts, sort codes 05/82) and "Standalone" APIs (personal accounts and credit cards, sort code 08). Access is secured with FAPI-grade OAuth2/OpenID Connect, PSD2 strong customer authentication, mutual-TLS client authentication, and dynamic client registration using OBIE (OBWAC/OBSeal) or eIDAS (QWAC/QSEAL) certificates.

**Areas:** Financial Services · Banking · Open Banking · PSD2 · OBIE · United Kingdom · Payments · Account Information · Confirmation of Funds · FAPI

## Virgin Money UK on APIs.io

Everything profiled for Virgin Money UK is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/virgin-money-uk/](https://apis.io/providers/virgin-money-uk/)** — or go straight to one of the APIs or properties below.

### APIs (17)

- [Virgin Money UK Account and Transaction API (AIS)](https://apis.io/apis/virgin-money-uk/account-transaction-api/) — OBIE Read/Write Account & Transaction Information (AIS) API - retrieve accounts, balances, transactions, beneficiaries, standing orders, direct debits, and…
- [Virgin Money UK Domestic Immediate Payment API (PIS)](https://apis.io/apis/virgin-money-uk/domestic-payments-api/) — OBIE Read/Write Payment Initiation (PIS) API for domestic immediate payments. Merged brand family, OBIE v3.1.2. FAPI OAuth2/OIDC + mTLS + PSD2 SCA.
- [Virgin Money UK Domestic Scheduled Payment API (PIS)](https://apis.io/apis/virgin-money-uk/domestic-scheduled-payments-api/) — OBIE Read/Write Payment Initiation (PIS) API for domestic scheduled payments. Merged brand family, OBIE v3.1.2. FAPI OAuth2/OIDC + mTLS + PSD2 SCA.
- [Virgin Money UK File Payments API (PIS)](https://apis.io/apis/virgin-money-uk/file-payments-api/) — OBIE Read/Write Payment Initiation (PIS) API for batch/file payments. Merged brand family, OBIE v3.1.2. FAPI OAuth2/OIDC + mTLS + PSD2 SCA.
- [Virgin Money UK International Payments API (PIS)](https://apis.io/apis/virgin-money-uk/international-payments-api/) — OBIE Read/Write Payment Initiation (PIS) API for international payments. Merged brand family, OBIE v3.1.2. FAPI OAuth2/OIDC + mTLS + PSD2 SCA.
- [Virgin Money UK International Scheduled Payments API (PIS)](https://apis.io/apis/virgin-money-uk/international-scheduled-payments-api/) — OBIE Read/Write Payment Initiation (PIS) API for international scheduled payments. Merged brand family, OBIE v3.1.2. FAPI OAuth2/OIDC + mTLS + PSD2 SCA.
- [Virgin Money UK Confirmation of Funds API (CBPII)](https://apis.io/apis/virgin-money-uk/confirmation-of-funds-api/) — OBIE Read/Write Confirmation of Funds (CBPII) API - allows a Card Based Payment Instrument Issuer to check whether sufficient balance is available to make a…
- [Virgin Money UK OIDC API](https://apis.io/apis/virgin-money-uk/oidc-api/) — Open Banking-compliant OpenID Connect provider for TPP authorisation. Live production discovery document confirmed (HTTP 200, 2026-07-23): issuer…
- [Virgin Money UK Token API](https://apis.io/apis/virgin-money-uk/token-api/) — OAuth2 token endpoint for obtaining access tokens used to call the OBIE Read/Write APIs. Documented at v3.0. Confirmed token endpoint (from live OIDC…
- [Virgin Money UK Dynamic Client Registration API](https://apis.io/apis/virgin-money-uk/dynamic-client-registration-api/) — OBIE Dynamic Client Registration (DCR) API allowing TPPs to register with Virgin Money brands using OBIE (OBWAC/OBSeal) or eIDAS (QWAC/QSEAL) certificates.…
- [Virgin Money UK Standalone Account and Transaction API (AIS)](https://apis.io/apis/virgin-money-uk/standalone-account-transaction-api/) — OBIE Read/Write Account & Transaction Information (AIS) API for the Standalone brand family (personal credit cards and sort-code-08 current and savings…
- [Virgin Money UK ATM API](https://apis.io/apis/virgin-money-uk/virgin-money-uk-atm-api/) — Endpoint for getting ATM data
- [Virgin Money UK BCA API](https://apis.io/apis/virgin-money-uk/virgin-money-uk-bca-api/) — Endpoint for getting Business Current Account data
- [Virgin Money UK Branch API](https://apis.io/apis/virgin-money-uk/virgin-money-uk-branch-api/) — Endpoint for getting Branch data
- [Virgin Money UK CCC API](https://apis.io/apis/virgin-money-uk/virgin-money-uk-ccc-api/) — Endpoint for getting Commercial Credit Card data
- [Virgin Money UK PCA API](https://apis.io/apis/virgin-money-uk/virgin-money-uk-pca-api/) — Endpoint for getting Personal Current Account data
- [Virgin Money UK SME API](https://apis.io/apis/virgin-money-uk/virgin-money-uk-sme-api/) — Endpoint for getting Unsecured SME Loan data

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Virgin Money Uk Agentic Access](https://apis.io/agentic-access/virgin-money-uk/virgin-money-uk-agentic-access/)

#### Collections (1)

Postman and Open Collection request collections.

- [Open Data API](https://apis.io/collections/virgin-money-uk/open-obie-opendata-api-standard/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Virgin Money Uk Opendata Overlay](https://apis.io/overlays/virgin-money-uk/virgin-money-uk-opendata-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Virgin Money Uk Authentication](https://apis.io/security/virgin-money-uk/virgin-money-uk-authentication/)
- [Virgin Money Uk Domain Security](https://apis.io/security/virgin-money-uk/virgin-money-uk-domain-security/)
- [Virgin Money Uk Vulnerability Disclosure](https://apis.io/security/virgin-money-uk/virgin-money-uk-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Virgin Money Uk Scopes](https://apis.io/scopes/virgin-money-uk/virgin-money-uk-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://uk.virginmoney.com/)
- [Documentation](https://developer.virginmoney.com/merged/)
- [Support](https://uk.virginmoney.com/support/)
- [Terms of service](https://uk.virginmoney.com/terms/)
- [Privacy policy](https://uk.virginmoney.com/privacy/)

## API Evangelist rating

**Kin Score 45.4** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 35.5 |
| Contract governance | 18.2 |
| Operational transparency | 18.4 |
| Developer ergonomics | 44.6 |
| Access clarity | 57.1 |

**Agent readiness 36.5** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | served (partial credit) |
| Idempotency | na |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 48.8** — Banking & Open Finance

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/virgin-money-uk/](https://apis.io/providers/virgin-money-uk/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Virgin Money UK: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/virgin-money-uk/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
