# Pocket Network (pocket-network)
Pocket Network is the decentralized RPC layer of Web3 — a permissionless, fully open data delivery protocol built on Cosmos SDK and CometBFT (the Shannon upgrade, June 2025). 5,000+ independent supplier nodes serve relays across 60-69+ blockchains, metered in compute units at $1/billion and settled on-chain in POKT under deflationary tokenomics (PIP-41, 97.5% mint ratio). Grove (grove.city) operates the largest gateway on the network — `rpc.grove.city` — and maintains PATH, the open-source Go gateway any operator can run.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Web3, Blockchain, RPC, Decentralized Infrastructure, Pocket Network, Grove, PATH, Shannon, Cosmos, POKT

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## What Is It

| Layer | Open Source | Hosted | Role |
|---|---|---|---|
| Shannon Protocol | [pokt-network/poktroll](https://github.com/pokt-network/poktroll) | `shannon-grove-api.mainnet.poktroll.com` | Cosmos SDK + CometBFT chain — applications, suppliers, gateways, services, sessions, proofs, tokenomics |
| PATH Gateway | [buildwithgrove/path](https://github.com/buildwithgrove/path) | `rpc.grove.city` | Go gateway that routes JSON-RPC, REST, and WS relays to Shannon suppliers with QoS scoring |
| Grove Portal | proprietary | `portal.grove.city` | Dashboard for portal applications, relay analytics, billing |
| RelayMiner | bundled in `poktroll` | self-hosted by suppliers | Supplier-side daemon that proxies relays to the underlying chain node |

## APIs

### Pocket Network PATH Gateway API
Send JSON-RPC, REST, or WebSocket relays through Grove's hosted PATH gateway on `rpc.grove.city`. Each chain is exposed as a subdomain (e.g. `eth.rpc.grove.city/v1/{appId}` for authenticated portal traffic, `eth.rpc.grove.city/v1` for free public). Self-hosters can run the same PATH binary against any Shannon Application/Gateway key pair.

**Human URL:** [https://path.grove.city/](https://path.grove.city/)

- [Documentation — PATH Introduction](https://path.grove.city/develop/path/introduction)
- [Documentation — PATH Cheat Sheet](https://path.grove.city/develop/path/cheatsheet)
- [OpenAPI](openapi/pocket-network-path-gateway-api-openapi.yml)
- [JSON Schema — Relay](json-schema/pocket-network-relay-schema.json)
- [JSON-LD Context](json-ld/pocket-network-context.jsonld)
- [Naftiko Capability — PATH Relays](capabilities/path-gateway-relays.yaml)
- [Source Code — buildwithgrove/path](https://github.com/buildwithgrove/path)

### Pocket Network Shannon RPC API
The Shannon chain Cosmos REST surface. Standard `/cosmos/*` modules plus Pocket-specific `/pocket/application/v1`, `/pocket/supplier/v1`, `/pocket/gateway/v1`, `/pocket/service/v1`, `/pocket/session/v1`, `/pocket/proof/v1`, and `/pocket/tokenomics/v1`.

**Human URL:** [https://dev.poktroll.com/](https://dev.poktroll.com/)

- [Documentation — Shannon Developer Docs](https://dev.poktroll.com/)
- [Documentation — Shannon Upgrade](https://docs.pokt.network/pokt-protocol/the-shannon-upgrade)
- [OpenAPI](openapi/pocket-network-shannon-rpc-api-openapi.yml)
- [JSON Schema — Shannon Actor](json-schema/pocket-network-shannon-actor-schema.json)
- [Naftiko Capability — Blocks](capabilities/shannon-blocks.yaml)
- [Naftiko Capability — Applications](capabilities/shannon-applications.yaml)
- [Naftiko Capability — Suppliers](capabilities/shannon-suppliers.yaml)
- [Naftiko Capability — Gateways](capabilities/shannon-gateways.yaml)
- [Naftiko Capability — Services](capabilities/shannon-services.yaml)
- [Naftiko Capability — Tokenomics](capabilities/shannon-tokenomics.yaml)
- [Source Code — pokt-network/poktroll](https://github.com/pokt-network/poktroll)

### Pocket Network CometBFT RPC API
The CometBFT (Tendermint) JSON-RPC surface on port 26657 — consensus-level queries (`status`, `net_info`, `block`, `block_results`, `tx`), mempool inspection, and synchronous transaction broadcast.

**Human URL:** [https://dev.poktroll.com/](https://dev.poktroll.com/)

- [Documentation — CometBFT RPC](https://docs.cometbft.com/v0.38/rpc/)
- [OpenAPI](openapi/pocket-network-cometbft-rpc-api-openapi.yml)
- [Naftiko Capability — CometBFT Status](capabilities/cometbft-status.yaml)

## Supported Chains (selected)

EVM mainnets and L2s: **Ethereum, Polygon, BSC, Avalanche, Gnosis, Celo, Fantom, Harmony, Moonbeam, Moonriver, Fuse, IoTeX, Oasys, Kaia, Berachain, Sonic, Ink, XRPL EVM, Arbitrum, Optimism, Base, zkSync Era, zkLink Nova, Scroll, Linea, Mantle, Blast, Boba, Metis, Taiko, Unichain, opBNB, Fraxtal, Polygon zkEVM**.

Cosmos and non-EVM: **Osmosis, Juno, Akash, Kava, Persistence, Stargaze, AtomOne, Cheqd, Chihuahua, Fetch.ai, Hyperliquid, Jackal, Pocket Network, Seda, Sei, Shentu, Solana**.

See [Supported Chains on Grove](https://grove.city/chains) for the live list.

## Pricing

| Plan | Price | Notes |
|---|---|---|
| Grove Public Endpoints | Free | No API key, per-IP throttled, 69+ chains, best-effort QoS |
| Grove Portal — Pay-As-You-Go | $1 / 1M relays (RELAY2025) | Authenticated Application IDs, analytics, custom rate limits |
| Grove Enterprise | Custom | Dedicated PATH, archive/debug/trace support, SLA |
| Pocket Network Wholesale | $1 / 1B compute units | Protocol-level pricing settled in POKT on-chain |

See [plans/pocket-network-plans-pricing.yml](plans/pocket-network-plans-pricing.yml), [rate-limits/pocket-network-rate-limits.yml](rate-limits/pocket-network-rate-limits.yml), and [finops/pocket-network-finops.yml](finops/pocket-network-finops.yml) for machine-readable details.

## Governance and Economics

- **Pocket Network Foundation (PNF)** — non-profit steward of the protocol and the F-Chains public-data program.
- **Grove** — for-profit operator of the dominant gateway on the network and maintainer of PATH.
- **POKT token** — Cosmos asset (denom `upokt`); deflationary post-PIP-41 (97.5% mint ratio).
- **Service fees** — denominated in compute units pegged to USD; 1 CU = $0.000000001.
- **Shannon upgrade** — June 2025 Morse → Shannon migration made Pocket a native Cosmos chain with permissionless service registration.

## Tooling and SDKs

- [poktrolld CLI](https://github.com/pokt-network/poktroll) — Cosmos SDK tx/query/keys binary
- [Homebrew tap](https://github.com/pokt-network/homebrew-pocketd) — `brew tap pokt-network/poktroll && brew install poktrolld`
- [Shannon SDK (Go)](https://github.com/pokt-network/shannon-sdk)
- [Shannon Transaction Builder (Python)](https://github.com/pokt-network/shannon-tx-builder)
- [poktroll-clients-py (Python)](https://github.com/pokt-network/poktroll-clients-py)
- [pocket-js (JavaScript Protocol Library)](https://github.com/pokt-network/pocket-js)
- [Pocketdex (SubQuery indexer)](https://github.com/pokt-network/pocketdex)
- [Pocket Explorer](https://github.com/pokt-network/pocket-explorer)

## Status

- [Pocket Network Status](https://status.pocket.network/)
- [Grove Status](https://status.grove.city/)
- [Pocket Network Explorer (mainnet)](https://explorer.pocket.network/pocket-mainnet)

## Repository Artifacts

| Folder | Contents |
|---|---|
| `openapi/` | OpenAPI 3.1 specs for PATH, Shannon REST, CometBFT RPC |
| `capabilities/` | Naftiko capability YAML files for each business surface |
| `json-schema/` | JSON Schemas for Relay and Shannon actor objects |
| `json-ld/` | JSON-LD context for Pocket Network vocabulary |
| `examples/` | Sample request/response payloads |
| `rules/` | Spectral ruleset enforcing API Evangelist conventions |
| `vocabulary/` | Vocabulary YAML for the Pocket Network domain |
| `plans/` | API Commons Plans pricing |
| `rate-limits/` | API Commons Rate Limits |
| `finops/` | FOCUS-aligned FinOps definition |

## Review

See [review.yml](review.yml) for the API Evangelist Tier-1 review.

## Maintainer

- **FN:** Kin Lane
- **Email:** info@apievangelist.com
- **X:** @apievangelist
- **URL:** [https://apievangelist.com](https://apievangelist.com)
