# Hi, I'm Alex

**Product-Minded Fullstack Developer** | Building products, not just writing code

![Solidity](https://img.shields.io/badge/-Solidity-363636?style=flat-square&logo=solidity&logoColor=white)
![Rust](https://img.shields.io/badge/-Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Solana](https://img.shields.io/badge/-Solana-9945FF?style=flat-square&logo=solana&logoColor=white)
![Anchor](https://img.shields.io/badge/-Anchor-654FF0?style=flat-square)
![Foundry](https://img.shields.io/badge/-Foundry-1C1C1C?style=flat-square&logo=ethereum&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![tRPC](https://img.shields.io/badge/-tRPC-2596BE?style=flat-square&logo=trpc&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Tailwind](https://img.shields.io/badge/-Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

> 8+ years in development, 5+ in Web3 across EVM and Solana. I think about what to build before writing the first line of code.

---

## Featured Projects

### [Missing Days](https://missing-days.vercel.app)
A BasePaint profile for any address: which daily canvases it owns, which days are missing from each set, which of those gaps are scarce, and what it painted. No wallet connect, no keys, no backend, every number read from BasePaint's public indexer.

`Next.js 16` `React 19` `viem` `Vercel` `BasePaint Indexer` `CC0`

- **Winner, BasePaint Year 3 Hackathon, category FOR COLLECTORS** (32 projects, 8 judges)
- [Live](https://missing-days.vercel.app) | [GitHub](https://github.com/devacc8/missing-days) | [Winners announcement](https://x.com/basepaint_xyz/status/2089728694852190523)
- Judges: "Clean, simple and instantly useful to visualize and complete a collection."
- Released CC0 so it can fold back into BasePaint itself

### [BasePaint Market](https://basepaint.market)
First atomic 365-NFT bundle marketplace on Base L2. Trustless approval-based listings (no escrow), full-stack implementation from Solidity to frontend.

`Solidity` `Next.js 14` `Node.js` `PostgreSQL` `RainbowKit` `wagmi` `viem` `Docker` `Base L2`

- 3,700+ automated tests across the stack
- 9.0/10 security audit score, 0 critical issues
- Built end-to-end: smart contracts, backend, frontend, audit

### [SkillTax](https://skilltax.gg)
Trustless peer-to-peer skill-wagering on Solana. Two players stake USDC on their own 1v1 match (Brawl Stars, Chess.com, Lichess), a worker verifies the result through the game's API, and an Anchor escrow pays the winner automatically. No house, no screenshots, no disputes.

`Solana` `Anchor` `Rust` `Next.js 15` `tRPC` `Privy` `Supabase`

- Winner takes 95%, resolved on-chain. The contract has no instruction to ban winning players
- Passkey onboarding in about 2 seconds: no seed phrase, no wallet extension
- Platform-sponsored gas, so players only ever need USDC, never SOL
- No token, on purpose: pure USDC escrow with no platform coin
- Colosseum Frontier Hackathon 2026 MVP (Solana devnet)

### [CoinPeek](https://chromewebstore.google.com/detail/coinpeek-bitcoin-price-ba/konlmcdlofpoegdkbjocdfojejmfkfbo)
Chrome extension that keeps the Bitcoin price in the toolbar badge, plus ETH prices, gas fees for both networks, and a BTC/ETH/USD converter. Updates every minute from a Manifest V3 service worker and caches the last known prices for offline use.

`JavaScript` `Chrome APIs` `Manifest V3` `CoinGecko` `Blocknative` `mempool.space`

- Live in the Chrome Web Store, about 50KB, MIT licensed
- 5 API integrations with 3 fallback APIs, so one provider outage does not blank the badge
- Open source: [GitHub](https://github.com/devacc8/coinpeek)

### [AvaxLens](https://avaxlens.vercel.app)
Free smart contract analytics for Avalanche C-Chain. Paste any contract address and get transaction volume, gas usage, function breakdown, decoded revert reasons, top callers and an AI security audit with a risk grade. No signup, no API key, no cost.

`Next.js 16` `TypeScript` `Tailwind CSS 4` `Recharts` `viem` `Avalanche`

- Six dashboard tabs over up to 10,000 transactions, decoded server-side with viem from Routescan and Snowtrace data
- Analytics pre-computed to about 2KB of JSON per contract, so charts render in seconds with no client-side parsing
- Built for Avalanche Build Games 2026, development by me with a partner on design and documentation
- Rate limiting, CSP and HSTS headers, LRU caches on ABI, analytics and transaction data
- [GitHub](https://github.com/devacc8/avaxlens)

### [DSH Billing Badge](https://github.com/devacc8/dsh-billing-badge)
Billing season and account balance for [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness), the open-source agent harness where everything is a plugin. A pill in the composer statistics row shows a peak or off-peak dot with a countdown to the next switch, and opens a panel that splits the balance into granted and topped up in the currency the API reports.

`JavaScript` `ESM` `DeepSeek Harness` `npm` `MIT`

- Published on npm, so it installs with `dsh plugin --profile web add dsh-billing-badge`
- The API key stays in the host process, the single route rejects cross-origin callers, and nothing is written to disk
- 30 tests, GitHub Actions on Node 20 and 22, no dependencies
- Reads `is_available` from the top level of the official balance response, so the panel warns only when the API really reports an insufficient balance
- [GitHub](https://github.com/devacc8/dsh-billing-badge) | [npm](https://www.npmjs.com/package/dsh-billing-badge)

### [DSH File Explorer](https://github.com/devacc8/dsh-file-explorer)
A vendored, hardened fork of a community file explorer for the DeepSeek Harness web GUI: a file tree with a tabbed preview, search, sorting and in-panel editing.

`TypeScript` `DeepSeek Harness` `Security hardening` `MIT`

- Every path, reads included, is confined to a registered workspace root; external programs launch argv-only
- English UI, theme-matched panel, file-type colours, indent guides, per-workspace memory of expanded folders and scroll position
- Three fixes that are not fork-specific were sent upstream as pull requests
- [GitHub](https://github.com/devacc8/dsh-file-explorer)

---

## Achievements

| | |
|---|---|
| **BasePaint Hackathon Winner** | Year 3 (2026), category FOR COLLECTORS, Missing Days |
| **PoolTogether Special Prize** | ETHOnline 2020, Chainlink-sponsored ETHGlobal hackathon |
| **Open Source Contributor** | PRs merged to Talent Protocol, Base ecosystem |
| **Published Extension** | CoinPeek approved in Chrome Web Store |
| **3,700+ Tests** | BasePaint Market, 9.0/10 audit score |

---

## GitHub Activity

![GitHub Contribution Graph](https://ghchart.rshah.org/c87941/devacc8)

---

## Connect

[![Website](https://img.shields.io/badge/-vegaforge.dev-c87941?style=flat-square&logo=google-chrome&logoColor=white)](https://vegaforge.dev)
[![X](https://img.shields.io/badge/-@vvegalex-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/vvegalex)
[![Email](https://img.shields.io/badge/-devacc8@pm.me-8B89CC?style=flat-square&logo=protonmail&logoColor=white)](mailto:devacc8@pm.me)

---

> "The old model where PM designs and developer codes no longer works. Teams need people who understand both what to build and how."
