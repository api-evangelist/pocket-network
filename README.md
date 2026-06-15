# Pocket Network (pocket-network)

Pocket Network is the decentralized RPC layer of Web3 — a permissionless, fully open data delivery protocol built on Cosmos SDK and CometBFT (the Shannon upgrade, June 2025). 5,000+ independent supplier nodes serve relays across 60-69+ blockchains, metered in compute units at $1/billion and settled on-chain in POKT under deflationary tokenomics (PIP-41, 97.5% mint ratio). Grove (grove.city) is the for-profit infrastructure company that operates the largest gateway on the network — rpc.grove.city — and maintains PATH, the open-source Go gateway any operator can run to expose Pocket Network as a single HTTP endpoint. Grove offers free no-API-key per-IP public endpoints per chain (eth.rpc.grove.city, solana.rpc.grove.city, etc.) plus paid portal applications with relay analytics and SLAs. Together they form the canonical decentralized alternative to Alchemy / Infura / QuickNode for serving JSON-RPC, REST, and WebSocket traffic to any public blockchain.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Web3
- Blockchain
- RPC
- Decentralized Infrastructure
- Pocket Network
- Grove
- PATH
- Shannon
- Cosmos
- POKT

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Pocket Network PATH Gateway API

PATH is the open-source Go gateway (github.com/buildwithgrove/path) that exposes Pocket Network Shannon as a single HTTP surface. It proxies JSON-RPC, REST, and WebSocket relays to Shannon suppliers, scores them via QoS, and signs each relay with the operator's gateway and application keys. Grove operates the largest hosted PATH deployment on rpc.grove.city across 69+ chains, both as authenticated portal endpoints and as no-key public endpoints per chain (e.g. eth.rpc.grove.city, solana.rpc.grove.city).

- **Human URL:** [https://path.grove.city/](https://path.grove.city/)

#### Tags

- Pocket Network
- Grove
- PATH
- RPC
- Relays

#### Properties

- [Documentation](https://path.grove.city/develop/path/introduction)
- [Documentation](https://path.grove.city/develop/path/cheatsheet)
- [OpenAPI](openapi/pocket-network-path-gateway-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pocket-network-path-gateway-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pocket-network-path-gateway-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/pocket-network-relay-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/pocket-network-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Source Code](https://github.com/buildwithgrove/path)

### Pocket Network Shannon RPC API

The Shannon chain is a Cosmos SDK + CometBFT chain (github.com/pokt-network/poktroll) that supplanted Morse in June 2025. The REST surface exposes the standard Cosmos modules (bank, staking, base) alongside Pocket-specific modules — application, supplier, gateway, service, session, proof, and tokenomics. Service fees are denominated in compute units (1 USD = 1B CU) and post-PIP-41 a 97.5% mint ratio makes POKT deflationary. Grove operates a public Shannon mainnet REST endpoint at shannon-grove-api.mainnet.poktroll.com.

- **Human URL:** [https://dev.poktroll.com/](https://dev.poktroll.com/)

#### Tags

- Pocket Network
- Shannon
- Cosmos
- Blockchain

#### Properties

- [Documentation](https://dev.poktroll.com/)
- [Documentation](https://docs.pokt.network/pokt-protocol/the-shannon-upgrade)
- [OpenAPI](openapi/pocket-network-shannon-rpc-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pocket-network-shannon-rpc-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pocket-network-shannon-rpc-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/pocket-network-shannon-actor-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Source Code](https://github.com/pokt-network/poktroll)

### Pocket Network CometBFT RPC API

The CometBFT (Tendermint) JSON-RPC surface exposed by every Shannon full node on port 26657. Covers consensus-level queries (status, net_info, blocks, block_results, tx), mempool inspection, and synchronous transaction broadcast. Grove operates a public Shannon mainnet CometBFT RPC at shannon-grove-rpc.mainnet.poktroll.com.

- **Human URL:** [https://dev.poktroll.com/](https://dev.poktroll.com/)

#### Tags

- Pocket Network
- Shannon
- CometBFT
- Tendermint
- Consensus

#### Properties

- [Documentation](https://docs.cometbft.com/v0.38/rpc/)
- [OpenAPI](openapi/pocket-network-cometbft-rpc-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pocket-network-cometbft-rpc-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pocket-network-cometbft-rpc-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Source Code](https://github.com/pokt-network/poktroll)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://pocket.network)
- [Portal](https://grove.city)
- [Documentation](https://path.grove.city/)
- [Documentation](https://docs.pokt.network/)
- [Documentation](https://docs.grove.city/)
- [Documentation](https://dev.poktroll.com/)
- [Status Page](https://status.pocket.network/)
- [Status Page](https://status.grove.city/)
- [Documentation](https://explorer.pocket.network/pocket-mainnet)
- [Documentation](https://wallet.pocket.network/)
- [Forum](https://forum.pokt.network/)
- [Forum](https://discord.gg/pocket-network)
- [GitHub Organization](https://github.com/pokt-network)
- [GitHub Organization](https://github.com/buildwithgrove)
- [Source Code](https://github.com/pokt-network/poktroll)
- [Source Code](https://github.com/buildwithgrove/path)
- [Source Code](https://github.com/pokt-network/path)
- [SDK](https://github.com/pokt-network/shannon-sdk)
- [SDK](https://github.com/pokt-network/poktroll-clients-py)
- [SDK](https://github.com/pokt-network/shannon-tx-builder)
- [SDK](https://github.com/pokt-network/pocket-js)
- [Tool](https://github.com/pokt-network/homebrew-pocketd)
- [Tool](https://github.com/pokt-network/pocketdex)
- [Tool](https://github.com/pokt-network/pocket-explorer)
- [Changelog](https://github.com/pokt-network/poktroll/releases)
- [Blog](https://medium.com/decentralized-infrastructure)
- [Blog](https://pocket.network/blog/)
- [Getting Started](https://pocket.network/pocket-developer-guide/)
- [Documentation](https://pocket.network/shannon-upgrade-faq/)
- [Documentation](https://pocket.network/decentralized-data-stack/)
- [Documentation](https://grove.city/chains)
- [Documentation](https://grove.city/partners)
- [Pricing](https://grove.city/pricing)
- [Privacy Policy](https://pocket.network/legal/privacy-policy/)
- [Terms of Service](https://pocket.network/legal/terms-of-service/)
- [Plans](plans/pocket-network-plans-pricing.yml)
- [Rate Limits](rate-limits/pocket-network-rate-limits.yml)
- [Fin Ops](finops/pocket-network-finops.yml)
- [Spectral Rules](rules/pocket-network-rules.yml)
- [Vocabulary](vocabulary/pocket-network-vocabulary.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
