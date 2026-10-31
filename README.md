# Pocket Network

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

Pocket Network is the decentralized RPC layer of Web3 — a permissionless, fully open data delivery protocol built on Cosmos SDK and CometBFT (the Shannon upgrade, June 2025). 5,000+ independent supplier nodes serve relays across 60-69+ blockchains, metered in compute units at $1/billion and settled on-chain in POKT under deflationary tokenomics (PIP-41, 97.5% mint ratio). Grove (grove.city) is the for-profit infrastructure company that operates the largest gateway on the network — rpc.grove.city — and maintains PATH, the open-source Go gateway any operator can run to expose Pocket Network as a single HTTP endpoint. Grove offers free no-API-key per-IP public endpoints per chain (eth.rpc.grove.city, solana.rpc.grove.city, etc.) plus paid portal applications with relay analytics and SLAs. Together they form the canonical decentralized alternative to Alchemy / Infura / QuickNode for serving JSON-RPC, REST, and WebSocket traffic to any public blockchain.

**Areas:** Web3 · Blockchain · RPC · Decentralized Infrastructure · Pocket Network · Grove · Path · Shannon · Cosmos · POKT

## Pocket Network on APIs.io

Everything profiled for Pocket Network is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/pocket-network/](https://apis.io/providers/pocket-network/)** — or go straight to one of the APIs or properties below.

### APIs (16)

- [Pocket Network Application API](https://apis.io/apis/pocket-network/pocket-network-application-api/) — Pocket application module — applications stake POKT to consume relays
- [Pocket Network Bank API](https://apis.io/apis/pocket-network/pocket-network-bank-api/) — POKT supply, balances, and burn tracking
- [Pocket Network Blocks API](https://apis.io/apis/pocket-network/pocket-network-blocks-api/) — Block and consensus state queries
- [Pocket Network Consensus API](https://apis.io/apis/pocket-network/pocket-network-consensus-api/) — Block, header, and consensus queries
- [Pocket Network Gateway API](https://apis.io/apis/pocket-network/pocket-network-gateway-api/) — Pocket gateway module — gateways stake POKT and proxy relays for applications
- [Pocket Network Health API](https://apis.io/apis/pocket-network/pocket-network-health-api/) — PATH service liveness and readiness probes
- [Pocket Network Mempool API](https://apis.io/apis/pocket-network/pocket-network-mempool-api/) — Mempool inspection and broadcast
- [Pocket Network Proof API](https://apis.io/apis/pocket-network/pocket-network-proof-api/) — Pocket proof module — claims and proofs that suppliers submit to earn POKT
- [Pocket Network Relays API](https://apis.io/apis/pocket-network/pocket-network-relays-api/) — JSON-RPC, REST, and WebSocket relays proxied to Shannon suppliers
- [Pocket Network Service API](https://apis.io/apis/pocket-network/pocket-network-service-api/) — Pocket service module — services represent the data sources (EVM chains, Solana, etc.) the network serves
- [Pocket Network Session API](https://apis.io/apis/pocket-network/pocket-network-session-api/) — Pocket session module — sessions group applications, suppliers, and services for a given block window
- [Pocket Network Status API](https://apis.io/apis/pocket-network/pocket-network-status-api/) — Node status and network info
- [Pocket Network Supplier API](https://apis.io/apis/pocket-network/pocket-network-supplier-api/) — Pocket supplier module — suppliers stake POKT and serve relays via RelayMiner
- [Pocket Network Tokenomics API](https://apis.io/apis/pocket-network/pocket-network-tokenomics-api/) — Pocket tokenomics module — global mint, burn, and reward parameters
- [Pocket Network Transactions API](https://apis.io/apis/pocket-network/pocket-network-transactions-api/) — Transaction lookup and broadcast
- [Pocket Network Validators API](https://apis.io/apis/pocket-network/pocket-network-validators-api/) — Staking and validator queries

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (8)

Multi-step workflows that chain operations into a business task.

- [Pocket Network CometBFT Node Block Inspect](https://apis.io/arazzos/pocket-network/pocket-network-cometbft-node-block-inspect-workflow/)
- [Pocket Network PATH Relay Readiness](https://apis.io/arazzos/pocket-network/pocket-network-path-relay-readiness-workflow/)
- [Pocket Network Shannon Application Balance](https://apis.io/arazzos/pocket-network/pocket-network-shannon-application-balance-workflow/)
- [Pocket Network Shannon Application Session](https://apis.io/arazzos/pocket-network/pocket-network-shannon-application-session-workflow/)
- [Pocket Network Shannon Block Explorer](https://apis.io/arazzos/pocket-network/pocket-network-shannon-block-explorer-workflow/)
- [Pocket Network Shannon Service Economics](https://apis.io/arazzos/pocket-network/pocket-network-shannon-service-economics-workflow/)
- [Pocket Network Shannon Supplier and Gateway Survey](https://apis.io/arazzos/pocket-network/pocket-network-shannon-supplier-gateway-survey-workflow/)
- [Pocket Network Shannon Transaction Lookup](https://apis.io/arazzos/pocket-network/pocket-network-shannon-transaction-lookup-workflow/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Pocket Network Agentic Access](https://apis.io/agentic-access/pocket-network/pocket-network-agentic-access/)

#### JSON Schema (2)

The data models the API reads and writes.

- [Pocket Network Relay](https://apis.io/schemas/pocket-network/pocket-network-relay/)
- [Pocket Network Shannon Actor](https://apis.io/schemas/pocket-network/pocket-network-shannon-actor/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Pocket Network Context](https://apis.io/jsonld/pocket-network/pocket-network-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Pocket Network Vocabulary](https://apis.io/vocabularies/pocket-network/pocket-network-vocabulary/)

#### Examples (3)

Example requests and responses.

- [Pocket Network Eth Block Number Example](https://apis.io/examples/pocket-network/pocket-network-eth-block-number-example/)
- [Pocket Network List Shannon Services Example](https://apis.io/examples/pocket-network/pocket-network-list-shannon-services-example/)
- [Pocket Network Shannon Latest Block Example](https://apis.io/examples/pocket-network/pocket-network-shannon-latest-block-example/)

#### Collections (22)

Postman and Open Collection request collections.

- [Pocket Network CometBFT RPC Application API](https://apis.io/collections/pocket-network/open-pocket-network-application-api/)
- [Pocket Network CometBFT RPC Application Bank API](https://apis.io/collections/pocket-network/open-pocket-network-bank-api/)
- [Pocket Network CometBFT RPC Application Blocks API](https://apis.io/collections/pocket-network/open-pocket-network-blocks-api/)
- [Pocket Network CometBFT RPC API](https://apis.io/collections/pocket-network/open-pocket-network-cometbft-rpc-api/)
- [Pocket Network CometBFT RPC Application Consensus API](https://apis.io/collections/pocket-network/open-pocket-network-consensus-api/)
- [Pocket Network CometBFT RPC Application Gateway API](https://apis.io/collections/pocket-network/open-pocket-network-gateway-api/)
- [Pocket Network CometBFT RPC Application Health API](https://apis.io/collections/pocket-network/open-pocket-network-health-api/)
- [Pocket Network CometBFT RPC Application Mempool API](https://apis.io/collections/pocket-network/open-pocket-network-mempool-api/)
- [Pocket Network PATH Gateway API](https://apis.io/collections/pocket-network/open-pocket-network-path-gateway-api/)
- [Pocket Network CometBFT RPC Application Proof API](https://apis.io/collections/pocket-network/open-pocket-network-proof-api/)
- [Pocket Network CometBFT RPC Application Relays API](https://apis.io/collections/pocket-network/open-pocket-network-relays-api/)
- [Pocket Network CometBFT RPC Application Service API](https://apis.io/collections/pocket-network/open-pocket-network-service-api/)
- [Pocket Network CometBFT RPC Application Session API](https://apis.io/collections/pocket-network/open-pocket-network-session-api/)
- [Pocket Network Shannon RPC API](https://apis.io/collections/pocket-network/open-pocket-network-shannon-rpc-api/)
- [Pocket Network CometBFT RPC Application Status API](https://apis.io/collections/pocket-network/open-pocket-network-status-api/)
- [Pocket Network CometBFT RPC Application Supplier API](https://apis.io/collections/pocket-network/open-pocket-network-supplier-api/)
- [Pocket Network CometBFT RPC Application Tokenomics API](https://apis.io/collections/pocket-network/open-pocket-network-tokenomics-api/)
- [Pocket Network CometBFT RPC Application Transactions API](https://apis.io/collections/pocket-network/open-pocket-network-transactions-api/)
- [Pocket Network CometBFT RPC Application Validators API](https://apis.io/collections/pocket-network/open-pocket-network-validators-api/)
- [Pocket Network CometBFT RPC API](https://apis.io/collections/pocket-network/postman-pocket-network-cometbft-rpc-api/)
- [Pocket Network PATH Gateway API](https://apis.io/collections/pocket-network/postman-pocket-network-path-gateway-api/)
- [Pocket Network Shannon RPC API](https://apis.io/collections/pocket-network/postman-pocket-network-shannon-rpc-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Pocket Network — jsonschema rules](https://apis.io/rules/pocket-network/pocket-network-jsonschema-spectral-rules/)
- [Pocket Network API Rules](https://apis.io/rules/pocket-network/pocket-network-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Pocket Network Authentication](https://apis.io/security/pocket-network/pocket-network-authentication/)
- [Pocket Network Domain Security](https://apis.io/security/pocket-network/pocket-network-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Pocket Network Plans Pricing](https://apis.io/plans/pocket-network/pocket-network-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Pocket Network Rate Limits](https://apis.io/rate-limits/pocket-network/pocket-network-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Pocket Network Finops](https://apis.io/finops/pocket-network/pocket-network-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Documentation](https://path.grove.city/)
- [Getting started](https://pocket.network/pocket-developer-guide/)
- [Pricing](https://grove.city/pricing)
- [Changelog](https://github.com/pokt-network/poktroll/releases)
- [Blog](https://medium.com/decentralized-infrastructure)
- [Terms of service](https://pocket.network/legal/terms-of-service/)
- [Privacy policy](https://pocket.network/legal/privacy-policy/)
- [GitHub](https://github.com/pokt-network)
- [Status](https://status.pocket.network/)

## API Evangelist rating

**Unrated** — no public website could be reached for this company, so there was almost nothing to measure and nothing a reader could check.

This is not a score of zero. No rating is published for this company. If that is wrong because something public exists that we missed, say so on this repository or email [info@apievangelist.com](mailto:info@apievangelist.com) and it will be re-run — free, and no justification needed.

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Pocket Network: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/pocket-network/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
