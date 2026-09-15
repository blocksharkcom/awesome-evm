# Awesome EVM [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of open-source projects across the EVM (Ethereum Virtual Machine) ecosystem — smart-contract libraries, DEXes, bridges, L2 rollup stacks, block explorers, indexers, node clients, wallets, account abstraction, lending, oracles, MEV, restaking, NFT infrastructure, audit tooling, and more.

If a project is open-source, mature, and part of how production EVM chains and dApps are actually built today, it belongs here.

---

**Maintained by [Blockshark](https://blockshark.com) — custom EVM engineering, smart-contract reviews, and managed crypto infrastructure.**

[**blockshark.com**](https://blockshark.com) · [**Telegram: @blocksharkcom**](https://t.me/blocksharkcom)

If you're building on EVM and need a custom integration, a security review, a bespoke deployment pipeline, or a white-label DeFi product, [get in touch](https://blockshark.com/contact). We ship.

---

## Contents

- [Smart Contracts & Libraries](#smart-contracts--libraries)
- [DEX & AMM](#dex--amm)
- [Bridges & Cross-Chain Messaging](#bridges--cross-chain-messaging)
- [L2 Rollup Stacks](#l2-rollup-stacks)
- [Block Explorers](#block-explorers)
- [Indexers & Data](#indexers--data)
- [Execution Clients](#execution-clients)
- [Consensus Clients](#consensus-clients)
- [Wallets](#wallets)
- [Account Abstraction (ERC-4337)](#account-abstraction-erc-4337)
- [Lending & Money Markets](#lending--money-markets)
- [Stablecoin Protocols](#stablecoin-protocols)
- [Oracles](#oracles)
- [DEX Aggregators](#dex-aggregators)
- [NFT Infrastructure](#nft-infrastructure)
- [MEV & Searcher Tooling](#mev--searcher-tooling)
- [Restaking](#restaking)
- [Privacy](#privacy)
- [Identity & Social](#identity--social)
- [DAOs & Governance](#daos--governance)
- [Developer Tooling](#developer-tooling)
- [Audit & Security](#audit--security)
- [Token Standards](#token-standards)
- [Contributing](#contributing)

---

## Smart Contracts & Libraries

- [OpenZeppelin Contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) — Battle-tested library of reusable Solidity components for access control, tokens, governance, and proxies.
- [OpenZeppelin Contracts Upgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable) — Upgradeable variants of the above for proxy-based architectures.
- [Solady](https://github.com/Vectorized/solady) — Gas-optimized Solidity snippets with a focus on assembly and clarity. Production-grade.
- [Solmate](https://github.com/transmissions11/solmate) — Modern, opinionated and gas-optimised contract building blocks.
- [PRBMath](https://github.com/PaulRBerg/prb-math) — Solidity library for fixed-point arithmetic with extensive trigonometric and signed-integer support.
- [DSMath](https://github.com/dapphub/ds-math) — Safe math library; minimal but historically important.
- [Solidity-Utils](https://github.com/1inch/solidity-utils) — 1inch's collection of Solidity utility libraries.
- [WETH9](https://github.com/gnosis/canonical-weth) — The canonical Wrapped Ether contract source.

## DEX & AMM

- [Uniswap V2 Core](https://github.com/Uniswap/v2-core) — The original constant-product AMM. Forked into thousands of DEXes.
- [Uniswap V2 Periphery](https://github.com/Uniswap/v2-periphery) — Router and helper contracts for V2.
- [Uniswap V3 Core](https://github.com/Uniswap/v3-core) — Concentrated-liquidity AMM with per-position tick ranges.
- [Uniswap V3 Periphery](https://github.com/Uniswap/v3-periphery) — Router, position manager, and quoter for V3.
- [Uniswap V4 Core](https://github.com/Uniswap/v4-core) — Singleton pool architecture with hooks for arbitrary pool logic.
- [Uniswap V4 Periphery](https://github.com/Uniswap/v4-periphery) — Routers and example hooks for V4.
- [Uniswap X](https://github.com/Uniswap/UniswapX) — Permit2-based intent settlement protocol.
- [PancakeSwap Smart Contracts](https://github.com/pancakeswap/pancake-smart-contracts) — V2-style AMM and surrounding farms; the canonical BNB Chain DEX fork target.
- [PancakeSwap V3](https://github.com/pancakeswap/pancake-v3-contracts) — PancakeSwap's concentrated-liquidity port.
- [SushiSwap](https://github.com/sushiswap/sushiswap) — Multi-chain AMM with permissionless pool creation.
- [Curve Finance Contracts](https://github.com/curvefi/curve-contract) — StableSwap invariant for low-slippage stablecoin and pegged-asset trading.
- [Curve V2 (Cryptoswap)](https://github.com/curvefi/curve-crypto-contract) — Curve's variant for uncorrelated asset pairs.
- [Balancer V2](https://github.com/balancer/balancer-v2-monorepo) — Generalised AMM supporting weighted, stable, and custom pool types.
- [Balancer V3](https://github.com/balancer/balancer-v3-monorepo) — Latest iteration with vault-based hook architecture.
- [Trader Joe V2.1 (Liquidity Book)](https://github.com/traderjoe-xyz/joe-v2) — Bin-based concentrated liquidity AMM.
- [Maverick Protocol](https://github.com/maverickprotocol/maverick-v1-interfaces) — Dynamic-distribution AMM.
- [DODO V2](https://github.com/DODOEX/dodo-smart-contract) — Proactive market-maker (PMM) algorithm.
- [Algebra Protocol](https://github.com/cryptoalgebra/AlgebraV1) — Open V3 fork used across many smaller DEXes (QuickSwap, Camelot, etc.).
- [Velodrome](https://github.com/velodrome-finance/contracts) — ve(3,3) Solidly-style DEX on Optimism.
- [Solidly Labs](https://github.com/solidlylabs/solidly-v3) — Canonical reference implementation of the ve(3,3) model.

## Bridges & Cross-Chain Messaging

- [Hyperlane Monorepo](https://github.com/hyperlane-xyz/hyperlane-monorepo) — Permissionless interoperability framework with sovereign security modules per route.
- [LayerZero V2](https://github.com/LayerZero-Labs/LayerZero-v2) — Cross-chain messaging protocol with DVN-based security.
- [LayerZero Endpoint V1](https://github.com/LayerZero-Labs/LayerZero) — V1 reference for legacy integrations.
- [Wormhole](https://github.com/wormhole-foundation/wormhole) — Generic message-passing protocol across 30+ chains.
- [Axelar CGP](https://github.com/axelarnetwork/axelar-cgp-solidity) — General Message Passing contracts on EVM.
- [Connext (Everclear)](https://github.com/connext/monorepo) — Modular bridge with cross-chain intents.
- [deBridge Contracts](https://github.com/debridge-finance/debridge-contracts-v1) — Bridge protocol with native cross-chain swaps.
- [Across Protocol](https://github.com/across-protocol/contracts) — Optimistic UMA-backed bridge for capital-efficient transfers.
- [Stargate Finance](https://github.com/stargate-protocol/stargate) — LayerZero-built bridge with shared liquidity pools.
- [Synapse Protocol](https://github.com/synapsecns/synapse-contracts) — Multi-chain bridge with nUSD/nETH unified liquidity.
- [Hop Protocol](https://github.com/hop-protocol/contracts) — Rollup-to-rollup bridge using hToken model.
- [Socket (Bungee)](https://github.com/SocketDotTech/socket-DL) — Bridge aggregation with route-selection logic.
- [Chainlink CCIP](https://github.com/smartcontractkit/ccip) — Chainlink's cross-chain interoperability protocol.

## L2 Rollup Stacks

- [OP Stack (Optimism)](https://github.com/ethereum-optimism/optimism) — Modular rollup stack used by Optimism, Base, Mode, Worldchain, Zora, and many others.
- [Arbitrum Nitro](https://github.com/OffchainLabs/nitro) — Arbitrum One and Arbitrum Orbit codebase.
- [Polygon zkEVM Node](https://github.com/0xPolygonHermez/zkevm-node) — Polygon zkEVM execution and prover.
- [Polygon CDK](https://github.com/0xPolygon/cdk) — Polygon's Chain Development Kit for spinning up zk rollups.
- [zkSync Era](https://github.com/matter-labs/zksync-era) — Matter Labs' zkEVM rollup.
- [ZK Stack](https://github.com/matter-labs/zk_evm) — Matter Labs' framework for permissionless ZK chains.
- [Scroll](https://github.com/scroll-tech/scroll) — Native zkEVM rollup.
- [Linea](https://github.com/Consensys/linea-monorepo) — Consensys' zkEVM L2.
- [Taiko](https://github.com/taikoxyz/taiko-mono) — Type-1 (Ethereum-equivalent) zkEVM rollup.
- [Astar zkEVM](https://github.com/AstarNetwork/astar-frame) — Polkadot-aligned Polygon zkEVM stack.
- [Mantle](https://github.com/mantlenetworkio/mantle) — OP Stack fork with modular data availability.
- [Fraxtal Network](https://github.com/FraxFinance/fraxtal-public) — Frax-built OP Stack L2.
- [Manta Network Pacific](https://github.com/Manta-Network/manta-pay) — Privacy-focused rollup.

## Block Explorers

- [Blockscout](https://github.com/blockscout/blockscout) — The most widely deployed open-source EVM explorer; supports virtually any EVM chain.
- [Otterscan](https://github.com/otterscan/otterscan) — Local-first, performance-optimised explorer that pairs with Erigon.
- [Etherscan-style Public Indexer (lite)](https://github.com/blockscout/blockscout-rs) — Rust microservices that supplement Blockscout.

## Indexers & Data

- [The Graph (graph-node)](https://github.com/graphprotocol/graph-node) — Subgraph indexing protocol.
- [Subsquid SDK](https://github.com/subsquid/squid-sdk) — High-throughput indexing framework with TypeScript.
- [Ponder](https://github.com/ponder-sh/ponder) — Modern open-source indexer with hot-reload and SQL queries.
- [Envio HyperIndex](https://github.com/enviodev/hyperindex) — Real-time indexer with HyperSync backend.
- [Apibara](https://github.com/apibara/dna) — Streaming indexer with Direct Node Access.
- [Sentio](https://github.com/sentioxyz) — Observability and indexing platform (parts open).
- [Goldsky CLI / Subgraphs](https://github.com/goldsky-io) — Hosted subgraph and mirror infrastructure (SDK open).
- [Streamingfast Substreams](https://github.com/streamingfast/substreams) — Streaming indexing built on Firehose.
- [Tenderly Web3 Actions Examples](https://github.com/Tenderly/web3-actions-examples) — Open templates for serverless on-chain triggers.

## Execution Clients

- [Geth (go-ethereum)](https://github.com/ethereum/go-ethereum) — Reference Go implementation. Largest mainnet share.
- [Erigon](https://github.com/erigontech/erigon) — Highly efficient archive node implementation.
- [Reth](https://github.com/paradigmxyz/reth) — Paradigm's Rust execution client; modular, fast, production-ready.
- [Nethermind](https://github.com/NethermindEth/nethermind) — .NET execution client with strong L2 support.
- [Besu](https://github.com/hyperledger/besu) — Hyperledger's Java client; popular for enterprise and private chains.

## Consensus Clients

- [Prysm](https://github.com/prysmaticlabs/prysm) — Most-deployed Go consensus client.
- [Lighthouse](https://github.com/sigp/lighthouse) — Rust consensus client.
- [Teku](https://github.com/Consensys/teku) — Java consensus client by Consensys.
- [Lodestar](https://github.com/ChainSafe/lodestar) — TypeScript consensus client.
- [Nimbus](https://github.com/status-im/nimbus-eth2) — Nim consensus client; ultra-low resource use.

## Wallets

- [MetaMask Extension](https://github.com/MetaMask/metamask-extension) — Browser extension; the most-used self-custodial EVM wallet.
- [MetaMask Mobile](https://github.com/MetaMask/metamask-mobile) — React Native mobile wallet.
- [Rabby](https://github.com/RabbyHub/Rabby) — Pre-transaction simulation and security focus.
- [Frame](https://github.com/floating/frame) — Desktop signer that runs alongside any browser.
- [Rainbow Wallet](https://github.com/rainbow-me/rainbow) — Mobile wallet with strong UX for NFTs and DeFi.
- [WalletConnect Monorepo](https://github.com/WalletConnect/walletconnect-monorepo) — Wallet ↔ dApp communication standard.
- [AppKit (formerly Web3Modal)](https://github.com/WalletConnect/web3modal) — Pre-built wallet connection UI.
- [RainbowKit](https://github.com/rainbow-me/rainbowkit) — React wallet connection library.
- [ConnectKit](https://github.com/family/connectkit) — Family's polished wallet connector.
- [Safe Wallet UI](https://github.com/safe-global/safe-wallet-web) — Multisig wallet front-end.

## Account Abstraction (ERC-4337)

- [eth-infinitism/account-abstraction](https://github.com/eth-infinitism/account-abstraction) — Reference EntryPoint and SimpleAccount implementations.
- [Safe Smart Account](https://github.com/safe-global/safe-smart-account) — Gnosis Safe v1.4 contracts.
- [Safe Modules](https://github.com/safe-global/safe-modules) — Modular extensions including 4337.
- [Kernel (ZeroDev)](https://github.com/zerodevapp/kernel) — Modular smart-account kernel.
- [Biconomy Smart Account](https://github.com/bcnmy/scw-contracts) — ERC-4337 wallet contracts.
- [Pimlico Permissionless](https://github.com/pimlicolabs/permissionless.js) — Modular 4337 client and bundler SDK.
- [Stackup Bundler](https://github.com/stackup-wallet/stackup-bundler) — Production-grade open-source 4337 bundler in Go.
- [Skandha](https://github.com/etherspot/skandha) — TypeScript bundler.
- [Alchemy Account Kit](https://github.com/alchemyplatform/aa-sdk) — Embedded smart-account SDK.
- [Modular Account (Alchemy)](https://github.com/alchemyplatform/modular-account) — ERC-6900 modular wallet implementation.

## Lending & Money Markets

- [Aave V3](https://github.com/aave/aave-v3-core) — Cross-chain money market with isolated lending pools.
- [Aave V4 (draft)](https://github.com/aave-dao/aave-v4) — V4 development repo.
- [Compound V3 (Comet)](https://github.com/compound-finance/comet) — Single-borrow-asset, multi-collateral lending.
- [Morpho Blue](https://github.com/morpho-org/morpho-blue) — Permissionless minimal-trust lending primitive.
- [Morpho Optimizer](https://github.com/morpho-org/morpho-optimizers) — Peer-to-peer matching layer over Aave/Compound.
- [Spark](https://github.com/marsfoundation/sparklend-v1-core) — MakerDAO-aligned Aave-V3 fork.
- [Euler V2](https://github.com/euler-xyz/euler-vault-kit) — Modular vault kit for permissionless lending markets.
- [Silo Finance](https://github.com/silo-finance/silo-contracts-v2) — Risk-isolated lending markets per asset.

## Stablecoin Protocols

- [MakerDAO DSS](https://github.com/makerdao/dss) — Multi-collateral DAI core contracts.
- [Sky (formerly Maker)](https://github.com/sky-ecosystem) — Latest Sky Protocol contracts.
- [Liquity V2](https://github.com/liquity/bold) — BOLD stablecoin with delegated rates.
- [Frax Finance](https://github.com/FraxFinance/frax-solidity) — Fractional-algorithmic stablecoin and frxETH.
- [Reflexer (RAI)](https://github.com/reflexer-labs/geb) — Non-pegged reflex-index stablecoin.
- [Inverse Finance (DOLA)](https://github.com/InverseFinance) — DOLA stablecoin and DBR borrowing.
- [crvUSD](https://github.com/curvefi/curve-stablecoin) — Curve's LLAMMA-based stablecoin.
- [Ondo USDY](https://github.com/ondoprotocol) — Yield-bearing tokenised cash equivalents.

## Oracles

- [Chainlink](https://github.com/smartcontractkit/chainlink) — The most-used decentralized oracle network.
- [Pyth Network SDK](https://github.com/pyth-network/pyth-sdk-solidity) — Low-latency pull-based price feeds.
- [RedStone](https://github.com/redstone-finance/redstone-oracles-monorepo) — Modular oracle with on-demand price delivery.
- [API3](https://github.com/api3dao/airnode) — First-party data feeds via Airnode.
- [UMA](https://github.com/UMAprotocol/protocol) — Optimistic oracle for arbitrary off-chain data.
- [Chronicle](https://github.com/chronicleprotocol) — Maker-aligned oracle network.
- [DIA](https://github.com/diadata-org) — Open-source data layer with custom price methodologies.

## DEX Aggregators

- [1inch Limit Order Protocol](https://github.com/1inch/limit-order-protocol) — Gas-efficient on-chain limit order book.
- [1inch Aggregation Router V6](https://github.com/1inch/swap-contracts) — Pathfinder router contracts.
- [0x Protocol](https://github.com/0xProject/protocol) — Settlement protocol and exchange proxy.
- [Cow Protocol](https://github.com/cowprotocol/contracts) — Coincidence-of-wants batch auction settlement.
- [KyberSwap Aggregator](https://github.com/KyberNetwork/kyberswap-dex-lib) — Open-source dex math library powering the aggregator.

## NFT Infrastructure

- [Seaport](https://github.com/ProjectOpenSea/seaport) — OpenSea's marketplace settlement contracts.
- [Reservoir Indexer](https://github.com/reservoirprotocol/indexer) — Universal NFT API indexer.
- [Zora Protocol](https://github.com/ourzora/zora-protocol) — Mint/curation contracts for NFT creators.
- [Manifold Creator Core](https://github.com/manifoldxyz/creator-core-solidity) — Modular ERC-721/1155 creator contracts.
- [Sound Protocol](https://github.com/soundxyz/sound-protocol) — On-chain music NFT primitives.
- [Foundation Drop](https://github.com/f8n/fnd-protocol) — Foundation's auction and drop contracts.
- [Highlight Protocol](https://github.com/highlightxyz/protocol) — Series-based NFT distribution.
- [LooksRare V2](https://github.com/LooksRare/contracts-exchange-v2) — Open marketplace exchange contracts.

## MEV & Searcher Tooling

- [Flashbots MEV-Boost](https://github.com/flashbots/mev-boost) — PBS implementation for proposer-builder separation.
- [mev-share-client](https://github.com/flashbots/mev-share-client-ts) — Client SDK for the MEV-Share network.
- [mev-inspect-py](https://github.com/flashbots/mev-inspect-py) — Historical MEV analysis tool.
- [Suave](https://github.com/flashbots/suave) — Single Unified Auctioning Execution Layer.
- [rbuilder](https://github.com/flashbots/rbuilder) — Open-source block builder in Rust.
- [Ultra-sound builder (relay)](https://github.com/flashbots/mev-boost-relay) — Reference relay implementation.

## Restaking

- [EigenLayer Contracts](https://github.com/Layr-Labs/eigenlayer-contracts) — Original restaking primitive.
- [Symbiotic Core](https://github.com/symbioticfi/core) — Permissionless restaking framework.
- [Karak Protocol](https://github.com/karak-network) — Multi-asset restaking layer.

## Privacy

- [Aztec Packages](https://github.com/AztecProtocol/aztec-packages) — zk-rollup with native programmable privacy via Noir.
- [Noir](https://github.com/noir-lang/noir) — Domain-specific language for zk-SNARKs (used by Aztec).
- [Privacy Pools](https://github.com/0xbow-io/privacy-pools-core) — Compliant zero-knowledge withdrawal pools.
- [Railgun](https://github.com/Railgun-Privacy/contract) — Smart-contract-level transaction privacy.

## Identity & Social

- [ENS Contracts](https://github.com/ensdomains/ens-contracts) — Ethereum Name Service registry and resolver.
- [Ethereum Attestation Service (EAS)](https://github.com/ethereum-attestation-service/eas-contracts) — On-chain attestation primitive.
- [Lens Protocol V3](https://github.com/lens-protocol/lens-v3) — Decentralized social graph.
- [Farcaster Contracts](https://github.com/farcasterxyz/contracts) — Identity and storage contracts.
- [Sign Protocol](https://github.com/sign-protocol) — Omni-chain attestation protocol.

## DAOs & Governance

- [OpenZeppelin Governor](https://github.com/OpenZeppelin/openzeppelin-contracts/tree/master/contracts/governance) — Modular on-chain governance framework.
- [Aragon OSx](https://github.com/aragon/osx) — Modular DAO framework.
- [Snapshot](https://github.com/snapshot-labs/snapshot) — Off-chain gasless voting.
- [Tally](https://github.com/withtally/tally-app) — Front-end for on-chain DAOs.
- [Compound Governor Bravo](https://github.com/compound-finance/compound-protocol) — The classic Bravo governance contracts.
- [Safe Governance](https://github.com/safe-global/safe-modules/tree/main/modules/4337) — Multisig + module-based governance.
- [Hats Protocol](https://github.com/Hats-Protocol/hats-protocol) — Programmable roles for DAOs.

## Developer Tooling

- [Foundry](https://github.com/foundry-rs/foundry) — Modern Solidity development toolkit (forge, cast, anvil, chisel).
- [Hardhat](https://github.com/NomicFoundation/hardhat) — TypeScript-based dev environment with rich plugin ecosystem.
- [Remix](https://github.com/ethereum/remix-project) — Browser-based IDE for Solidity.
- [viem](https://github.com/wevm/viem) — Modern TypeScript Ethereum client; replaces ethers in most new code.
- [wagmi](https://github.com/wevm/wagmi) — React hooks for Ethereum, built on viem.
- [ethers.js](https://github.com/ethers-io/ethers.js) — Classic JS/TS Ethereum library, V6.
- [web3.js](https://github.com/web3/web3.js) — The original Ethereum JS library, V4.
- [web3.py](https://github.com/ethereum/web3.py) — Python Ethereum client.
- [ScaffoldETH 2](https://github.com/scaffold-eth/scaffold-eth-2) — Full-stack dApp starter.
- [Drizzle (Wagmi)](https://github.com/wevm/wagmi/tree/main/packages/cli) — Code generation for contracts.
- [Tevm](https://github.com/evmts/tevm-monorepo) — In-browser EVM execution for tests and forks.
- [Anvil](https://github.com/foundry-rs/foundry/tree/master/crates/anvil) — Foundry's local node.
- [Hardhat Network Helpers](https://github.com/NomicFoundation/hardhat/tree/main/packages/hardhat-network-helpers) — Test utilities for Hardhat.

## Audit & Security

- [Slither](https://github.com/crytic/slither) — Static analysis framework for Solidity. Industry standard.
- [Echidna](https://github.com/crytic/echidna) — Property-based fuzz tester.
- [Medusa](https://github.com/crytic/medusa) — Cross-platform Go fuzzer.
- [Mythril](https://github.com/Consensys/mythril) — Symbolic-execution analyzer.
- [Aderyn](https://github.com/Cyfrin/aderyn) — Rust-based Solidity static analyzer.
- [Halmos](https://github.com/a16z/halmos) — Symbolic testing on top of Foundry.
- [Wake](https://github.com/Ackee-Blockchain/wake) — Static analysis + testing framework.
- [Solhint](https://github.com/protofire/solhint) — Solidity linter.
- [solidity-coverage](https://github.com/sc-forks/solidity-coverage) — Code coverage for Hardhat/Truffle.
- [Mythx-cli](https://github.com/Consensys/mythx-cli) — Cloud-based analysis CLI.
- [Olympix](https://github.com/olympixai/oly-extension) — VS Code extension surfacing vulnerabilities inline.

## Token Standards

- [EIPs Repository](https://github.com/ethereum/EIPs) — Canonical home of every Ethereum Improvement Proposal.
- [ERC-20 Reference](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol)
- [ERC-721 Reference](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC721/ERC721.sol)
- [ERC-1155 Reference](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC1155/ERC1155.sol)
- [ERC-4626 Tokenised Vaults](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/extensions/ERC4626.sol)
- [ERC-4337 Account Abstraction](https://github.com/eth-infinitism/account-abstraction)
- [ERC-2535 Diamonds](https://github.com/mudgen/diamond-3-hardhat) — Multi-facet proxy reference implementation.
- [ERC-6909 Multi-Token Standard](https://github.com/Vectorized/solady/blob/main/src/tokens/ERC6909.sol)
- [ERC-7579 Modular Smart Accounts](https://github.com/erc7579/erc7579-implementation)
- [HostDeFi](https://hostdefi.com) — free token-safety scanner grading tokens A+–F from on-chain checks (mint/freeze authority, liquidity, holder concentration) across Solana + 7 EVM chains. Keyless REST API, hosted MCP, x402 endpoints.

---

## Contributing

Pull requests are very welcome. Please make sure your addition is:

1. **Open source** with a permissive or copyleft license (MIT, Apache-2.0, GPL family, BSL, etc.).
2. **Actively maintained** — commits in the last 12 months, or production-deployed and stable.
3. **EVM-relevant** — runs on, integrates with, or directly tools an EVM chain.
4. **Useful beyond a single team** — has documentation, multiple users, or is the reference implementation of a standard.

To add a project, open a PR that edits this README in alphabetical order within the relevant category. One-line description, focused on what the project does, not adjectives.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full guidelines.

---

## About Blockshark

[Blockshark](https://blockshark.com) builds production EVM infrastructure on demand.

- **Custom smart-contract development** — bespoke protocols, integrations, audited code.
- **Security review** — independent contract audit, dependency hygiene, deployment review.
- **Managed deployments** — production hosting with monitoring, queues, incident response.
- **White-label crypto products** — exchange interfaces, bridge front-ends, lending dashboards, NFT marketplaces.

Get in touch:

- Website: [**blockshark.com**](https://blockshark.com)
- Telegram: [**@blocksharkcom**](https://t.me/blocksharkcom)

---

## License

This list is licensed under [CC0-1.0](LICENSE) — public domain dedication. Use it however you like.
