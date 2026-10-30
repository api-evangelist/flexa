# Flexa

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

Flexa is a digital-currency payments network that lets businesses accept crypto and other digital assets from customers anywhere, with instant authorization, fraud-resistant settlement, and automatic conversion into a preferred payout currency so merchants avoid price volatility. The Flexa Payments API is built around the "commerce intent" resource, which represents any attempt to collect a digital-currency payment and tracks requested debits against actual credits; supporting resources include assets, refunds, events, links, brands, and flexcodes. Flexa ships prebuilt mobile UI Components for iOS, Android, and React Native, plus in-person (Point of Sale) and online acceptance options, and a production-grade test mode that uses a valueless ERC-20 "Credit" (CR) token. Flexa is backed by Pantera Capital and supports 99+ digital assets across Ethereum, Bitcoin, Lightning, Solana, and more.

**Areas:** Company · Cryptocurrency · Payments · Digital Currency · Fintech · Blockchain · Merchant Payments · Web3

## Flexa on APIs.io

Everything profiled for Flexa is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/flexa/](https://apis.io/providers/flexa/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [Flexa Assets API](https://apis.io/apis/flexa/flexa-assets-api/) — Assets encompass all the value that flows through the Flexa platform. In the Flexa API, both national currencies (“fiat“) and digital currencies (“crypto“…
- [Flexa Commerce Intents API](https://apis.io/apis/flexa/flexa-commerce-intents-api/) — Commerce intents offer a versatile way to process digital asset payments from your customers using any sales channel.
- [Flexa Events API](https://apis.io/apis/flexa/flexa-events-api/) — Events are created when any of the core resources on the Flexa platform change in a meaningful way, such as when a commerce intent succeeds or a digital…
- [Flexa Refunds API](https://apis.io/apis/flexa/flexa-refunds-api/) — Refunds are the only way by which a Flexa payment can be reversed. Refunds are always initiated by the recipient, and can be made for either a partial…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Flexa Events Webhooks](https://apis.io/asyncapis/flexa/flexa-events-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [flexa](https://apis.io/servers/flexa/flexa/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Flexa Agentic Access](https://apis.io/agentic-access/flexa/flexa-agentic-access/)

#### Collections (4)

Postman and Open Collection request collections.

- [Flexa Assets API](https://apis.io/collections/flexa/open-flexa-assets-api/)
- [Flexa Assets Commerce Intents API](https://apis.io/collections/flexa/open-flexa-commerce-intents-api/)
- [Flexa Assets Events API](https://apis.io/collections/flexa/open-flexa-events-api/)
- [Flexa Assets Refunds API](https://apis.io/collections/flexa/open-flexa-refunds-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Flexa Openapi Overlay](https://apis.io/overlays/flexa/flexa-openapi-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Flexa Authentication](https://apis.io/security/flexa/flexa-authentication/)
- [Flexa Domain Security](https://apis.io/security/flexa/flexa-domain-security/)
- [Flexa Vulnerability Disclosure](https://apis.io/security/flexa/flexa-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://flexa.co/)
- [Documentation](https://docs.flexa.co/introduction)
- [Getting started](https://docs.flexa.co/payments/getting-started)
- [API reference](https://docs.flexa.co/api-reference/introduction)
- [Support](https://support.flexa.co/en/)
- [Blog](https://flexa.co/newsroom)
- [Security](https://flexa.co/security/bug-bounty-program)
- [Terms of service](https://flexa.co/legal/terms)
- [Privacy policy](https://flexa.co/legal/privacy)
- [GitHub](https://github.com/flexa)

## API Evangelist rating

**Kin Score 45.1** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 60.4 |
| Contract governance | 4.5 |
| Operational transparency | 21.1 |
| Developer ergonomics | 73.2 |
| Access clarity | 21.1 |

**Agent readiness 31.4** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | verified |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 27.7** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/flexa/](https://apis.io/providers/flexa/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Flexa: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/flexa/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
