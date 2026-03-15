# 🎵 MANGA MUSIC

<div align="center">

![MANGA MUSIC Banner](assets/manga_music_cover.jpg)

<br/>

[![Solana](https://img.shields.io/badge/Blockchain-Solana-9945FF?style=for-the-badge&logo=solana&logoColor=white)](https://solana.com)
[![License](https://img.shields.io/badge/License-MIT-e8003d?style=for-the-badge)](LICENSE)
[![Built by](https://img.shields.io/badge/Built%20by-@solasidofun-1d9bf0?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/solasidofun)
[![Status](https://img.shields.io/badge/Status-Beta-ffe033?style=for-the-badge&logoColor=black)](https://mangamusic.xyz)
[![Hugging Face](https://img.shields.io/badge/Demo-Hugging%20Face-ff9d00?style=for-the-badge&logo=huggingface&logoColor=white)](https://huggingface.co)

<br/>

> **The First AI-Powered Music Generator on the Solana Blockchain.**
> Type a prompt. Get a track. Own it forever as an NFT.

<br/>

[🚀 Live Demo](https://mangamusic.xyz) · [📖 Docs](#documentation) · [🐦 Twitter](https://twitter.com/solasidofun) · [💬 Discord](#community) · [🗺️ Roadmap](#roadmap)

</div>

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [How It Works](#how-it-works)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Roadmap](#roadmap)
- [Tokenomics](#tokenomics)
- [Smart Contracts](#smart-contracts)
- [API Reference](#api-reference)
- [Contributing](#contributing)
- [Security](#security)
- [Community](#community)
- [License](#license)

---

## 🎌 Overview

**MANGA MUSIC** is a Web3 platform that combines cutting-edge AI music generation with the Solana blockchain, wrapped in a bold manga-inspired aesthetic. Users can describe any musical vibe in natural language — in English or Japanese — and receive a fully composed, AI-generated track in seconds. Every track is minted as an NFT, giving creators full ownership and on-chain royalty rights.

```
User types:  "lofi hip-hop, rainy night, 90s nostalgic vibes"
AI composes: Full track with instruments, BPM, structure & sound design
User owns:   NFT on Solana — royalties, resale rights, forever
```

### Why MANGA MUSIC?

| Problem | Our Solution |
|---|---|
| Music creation requires expensive studios & producers | AI generates tracks from a single text prompt |
| Artists lose royalties through traditional platforms | On-chain smart contract enforces automatic royalties |
| Web3 music UX is complex and intimidating | Manga-inspired UI that's simple and fun |
| High blockchain fees eat creator revenue | Solana transactions cost ~$0.00025 each |
| Global creators face language barriers | Full bilingual support: English + Japanese |

---

## ✨ Features

### 🤖 AI Music Generator
- Generate full tracks from any text prompt in seconds
- Supports complex multi-genre descriptions
- Outputs: Title, Genre, BPM, Mood, Instruments, Structure, Sound Design
- Powered by Claude AI (Anthropic)

### 🌏 Bilingual Interface
- Full support for **English** and **Japanese** prompts
- Language-aware AI responses
- UI fully translated — toggle with one click
- More languages planned post-launch

### 🔑 NFT Minting & Ownership
- Every generated track mints as a unique NFT on Solana
- Full IP rights transferred to creator's wallet
- On-chain metadata: title, genre, BPM, creator address
- Compatible with major Solana NFT marketplaces

### 💰 On-Chain Royalty System
- Automated royalty distribution via smart contracts
- Earn every time your track is played, sold, or licensed
- Transparent royalty history on-chain
- Configurable royalty percentage per track

### ⚡ Solana-Powered
- Transactions confirm in under 1 second
- Gas fees of ~$0.00025 per transaction
- 65,000 TPS capacity — never congested
- Wallet support: **Phantom**, **Solflare**, **Backpack**

### 🎛 Creator Dashboard *(Phase 2)*
- Track all your generated and minted music
- Earnings & royalty analytics
- Portfolio management
- Social sharing tools

---

## 🎵 How It Works

```
┌─────────────────────────────────────────────────────────────────┐
│                       MANGA MUSIC FLOW                          │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  1. CONNECT WALLET                                              │
│     └─ Phantom / Solflare / Backpack                            │
│                                                                 │
│  2. WRITE YOUR PROMPT                                           │
│     └─ "dark synthwave, rain on neon streets, 140 BPM"          │
│                                                                 │
│  3. PAY 0.01 SOL                                                │
│     └─ Approve micro-transaction in wallet                      │
│                                                                 │
│  4. AI COMPOSES                                                 │
│     └─ Claude AI generates full track description               │
│                                                                 │
│  5. MINT AS NFT                                                 │
│     └─ Track minted to your wallet on Solana                    │
│                                                                 │
│  6. EARN ROYALTIES                                              │
│     └─ Smart contract auto-distributes on every play/sale       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## 🛠 Tech Stack

### Frontend
| Technology | Purpose |
|---|---|
| HTML5 / CSS3 / Vanilla JS | Landing page & demo interface |
| Hugging Face Spaces | Static hosting & deployment |
| Google Fonts (Syne, DM Mono) | Manga-aesthetic typography |
| Anthropic Claude API | AI music generation engine |

### Blockchain
| Technology | Purpose |
|---|---|
| **Solana** | Primary blockchain |
| **Anchor Framework** | Smart contract development |
| **Metaplex** | NFT minting standard |
| **Phantom / Solflare SDK** | Wallet connectivity |
| **Orynth DEX** | Phase 1 token listing |

### Backend *(Phase 2)*
| Technology | Purpose |
|---|---|
| Node.js + Express | API server |
| Anthropic Claude API | AI music generation |
| Solana Web3.js | Blockchain interactions |
| IPFS / Arweave | Decentralized file storage |
| PostgreSQL | User & track database |

---

## 🚀 Getting Started

### Prerequisites

```bash
node >= 18.0.0
npm >= 9.0.0
# Phantom or Solflare wallet browser extension
# Solana Devnet SOL (for testing)
```

### Quick Start (Frontend Only)

```bash
# Clone the repository
git clone https://github.com/solasidofun/manga-music.git
cd manga-music

# Open the landing page directly — no build required
open index.html

# Or serve locally
npx serve .
```

### Full Development Setup

```bash
# Clone the repo
git clone https://github.com/solasidofun/manga-music.git
cd manga-music

# Install dependencies
npm install

# Copy environment variables
cp .env.example .env

# Configure your .env file
ANTHROPIC_API_KEY=your_anthropic_api_key
SOLANA_RPC_URL=https://api.devnet.solana.com
SOLANA_NETWORK=devnet
WALLET_PRIVATE_KEY=your_wallet_private_key

# Start development server
npm run dev
```

### Deploy to Hugging Face Spaces

1. Create a new Space on [huggingface.co](https://huggingface.co/spaces)
2. Select **Static** template
3. Upload `index.html` to the repository
4. Your app is live instantly — no build step needed ✅

```bash
# Or deploy via Git
git clone https://huggingface.co/spaces/YOUR_USERNAME/manga-music
cp index.html manga-music/
cd manga-music
git add . && git commit -m "Deploy MANGA MUSIC"
git push
```

### Get Devnet SOL for Testing

```bash
# Install Solana CLI
sh -c "$(curl -sSfL https://release.solana.com/stable/install)"

# Create a wallet
solana-keygen new

# Get devnet SOL (free)
solana airdrop 2 --url devnet
```

---

## 📁 Project Structure

```
manga-music/
│
├── 📄 index.html                    # Main landing page (single file, deploy-ready)
│
├── 📁 assets/                       # Brand & marketing assets
│   ├── manga_music_logo.jpg         # Logo (800×800)
│   ├── manga_music_cover.jpg        # Cover / banner (1500×500)
│   ├── manga_product_1_prompt.jpg   # Product image — Prompt UI
│   ├── manga_product_2_nft.jpg      # Product image — NFT Ownership
│   ├── manga_product_3_howto.jpg    # Product image — How It Works
│   ├── manga_music_roadmap.png      # Official roadmap (1200×1800)
│   └── promo/                       # 10 promotional PNG images
│       ├── promo_01_announcement.png
│       ├── promo_02_how_it_works.png
│       ├── promo_03_phase1_orynth.png
│       ├── promo_04_phase2_features.png
│       ├── promo_05_nft_ownership.png
│       ├── promo_06_why_solana.png
│       ├── promo_07_phase3_audit.png
│       ├── promo_08_phase4_cex.png
│       ├── promo_09_airdrop_cta.png
│       └── promo_10_final_hype.png
│
├── 📁 contracts/                    # Solana smart contracts (Anchor)
│   ├── programs/
│   │   └── manga-music/
│   │       └── src/
│   │           ├── lib.rs           # Main program entry
│   │           ├── mint.rs          # NFT minting logic
│   │           └── royalty.rs       # On-chain royalty system
│   ├── tests/
│   │   └── manga-music.ts
│   └── Anchor.toml
│
├── 📁 src/                          # Frontend source (Phase 2)
│   ├── components/
│   │   ├── PromptInput.js
│   │   ├── WalletConnect.js
│   │   ├── TrackResult.js
│   │   └── NFTCard.js
│   ├── utils/
│   │   ├── solana.js                # Solana Web3 helpers
│   │   ├── anthropic.js             # Claude AI integration
│   │   └── ipfs.js                  # IPFS upload helpers
│   └── i18n/
│       ├── en.json                  # English translations
│       └── ja.json                  # Japanese translations
│
├── 📁 api/                          # Backend API (Phase 2)
│   ├── routes/
│   │   ├── generate.js              # AI generation endpoint
│   │   ├── mint.js                  # NFT minting endpoint
│   │   └── tracks.js                # Track management
│   └── server.js
│
├── 📄 .env.example                  # Environment variables template
├── 📄 package.json
├── 📄 Anchor.toml
├── 📄 LICENSE
└── 📄 README.md                     # This file
```

---

## 🗺️ Roadmap

<div align="center">

![MANGA MUSIC Roadmap](assets/manga_music_roadmap.png)

</div>

### Phase 1 — Listing on Orynth `Q3 2025`
- [ ] Token Generation Event (TGE)
- [ ] Initial listing on **Orynth DEX**
- [ ] Liquidity pool setup & lock
- [ ] Community airdrop campaign
- [ ] Whitepaper v1.0 release
- [ ] Landing page live on Hugging Face

### Phase 2 — Full Feature Launch `Q4 2025`
- [ ] AI Music Generator goes live
- [ ] Prompt-to-Music engine (EN + JA)
- [ ] NFT minting per generated track
- [ ] Wallet integration (Phantom / Solflare)
- [ ] Creator dashboard & analytics
- [ ] On-chain royalty distribution system

### Phase 3 — Security Audit `Q1 2026`
- [ ] Smart contract audit by Tier-1 security firm
- [ ] AI model security review
- [ ] Bug bounty program launch
- [ ] On-chain royalty contract audit
- [ ] Public audit report release

### Phase 4 — CEX Listing `Q2 2026`
- [ ] Tier-2 exchange applications & listings
- [ ] Tier-1 exchange listing
- [ ] Market-maker partnership
- [ ] Cross-chain bridge integration
- [ ] Global marketing campaign
- [ ] Ecosystem expansion grants

---

## 💎 Tokenomics

> ⚠️ Full tokenomics details will be released in the Whitepaper v1.0 ahead of Phase 1.

| Allocation | Percentage | Details |
|---|---|---|
| 🌊 Liquidity Pool | 30% | Locked at launch |
| 🎁 Community Airdrop | 20% | Phase 1 campaign |
| 🏗 Development | 20% | 24-month vesting |
| 🤝 Partnerships | 15% | Strategic partners |
| 👥 Team | 10% | 12-month cliff + 24-month vest |
| 🛡 Reserve | 5% | Emergency & security fund |

**Token Utility:**
- Pay for AI track generation (discount vs SOL)
- Governance voting on platform features
- Staking for royalty revenue share
- Access to premium AI models & features
- NFT marketplace fee discounts

---

## 📜 Smart Contracts

### Deployed Addresses

| Contract | Network | Address |
|---|---|---|
| MANGA MUSIC Token | Devnet | `Coming in Phase 1` |
| NFT Minting Program | Devnet | `Coming in Phase 2` |
| Royalty Distributor | Devnet | `Coming in Phase 2` |
| Liquidity Pool | Orynth DEX | `Coming in Phase 1` |

### Contract Overview

#### `mint.rs` — NFT Minting
```rust
// Mints a generated track as NFT with on-chain metadata
pub fn mint_track(
    ctx: Context<MintTrack>,
    title: String,
    genre: String,
    bpm: u16,
    ipfs_uri: String,
    royalty_bps: u16,  // basis points, e.g. 500 = 5%
) -> Result<()>
```

#### `royalty.rs` — Royalty Distribution
```rust
// Automatically distributes royalties on secondary sales
pub fn distribute_royalty(
    ctx: Context<DistributeRoyalty>,
    sale_amount: u64,
) -> Result<()>
```

---

## 🔌 API Reference

### AI Music Generation

**POST** `/api/generate`

```json
// Request
{
  "prompt": "lofi hip-hop, rainy night café, 90s nostalgic vibes",
  "language": "en",   // "en" or "ja"
  "wallet": "YOUR_WALLET_ADDRESS"
}

// Response
{
  "success": true,
  "track": {
    "title": "Neon Rain Lofi #047",
    "genre": "Lo-Fi Hip-Hop",
    "bpm": 78,
    "mood": "Nostalgic, Melancholic",
    "instruments": ["Piano", "Vinyl Crackle", "Lo-Fi Drums", "Bass"],
    "structure": "Intro → Verse → Chorus → Bridge → Outro",
    "soundDesign": "Warm tape saturation with subtle reverb...",
    "generationId": "gen_abc123"
  }
}
```

### NFT Minting

**POST** `/api/mint`

```json
// Request
{
  "generationId": "gen_abc123",
  "wallet": "YOUR_WALLET_ADDRESS",
  "royaltyPercent": 5
}

// Response
{
  "success": true,
  "nft": {
    "mintAddress": "SOLANA_MINT_ADDRESS",
    "metadataUri": "https://arweave.net/...",
    "explorerUrl": "https://explorer.solana.com/..."
  }
}
```

### Track Library

**GET** `/api/tracks/:wallet`

```json
// Response
{
  "tracks": [
    {
      "mintAddress": "...",
      "title": "Neon Rain Lofi #047",
      "genre": "Lo-Fi Hip-Hop",
      "createdAt": "2025-10-15T08:30:00Z",
      "royaltiesEarned": "0.42 SOL"
    }
  ],
  "total": 12
}
```

---

## 🤝 Contributing

We welcome contributions from the community! Here's how to get involved:

### Development Contributions

```bash
# 1. Fork the repository
# 2. Create your feature branch
git checkout -b feature/your-feature-name

# 3. Make your changes and commit
git commit -m "feat: add your feature description"

# 4. Push to your fork
git push origin feature/your-feature-name

# 5. Open a Pull Request
```

### Contribution Guidelines

- Follow existing code style and naming conventions
- Write clear commit messages using [Conventional Commits](https://conventionalcommits.org)
- Add tests for new features where applicable
- Update documentation for any API changes
- All PRs require at least one reviewer approval

### Ways to Contribute

| Type | Description |
|---|---|
| 🐛 Bug Reports | Open an issue with detailed reproduction steps |
| 💡 Feature Requests | Open an issue with the `enhancement` label |
| 🌐 Translations | Add new language support in `src/i18n/` |
| 📖 Documentation | Improve README, docs, or code comments |
| 🎨 Design | Submit UI/UX improvements via issue |
| 🔒 Security | See [Security Policy](#security) below |

### Good First Issues

Look for issues tagged with `good first issue` or `help wanted` in the [Issues tab](https://github.com/solasidofun/manga-music/issues).

---

## 🔒 Security

### Reporting Vulnerabilities

**DO NOT** open public GitHub issues for security vulnerabilities.

Instead, please report security issues via:
- **Email:** security@mangamusic.xyz
- **Twitter DM:** [@solasidofun](https://twitter.com/solasidofun)

We aim to respond within **48 hours** and will credit responsible disclosures.

### Bug Bounty *(Phase 3)*

A formal bug bounty program will launch in Phase 3 after the security audit. Rewards will range from **$100 to $10,000 USD** in MANGA MUSIC tokens depending on severity.

| Severity | Reward Range |
|---|---|
| 🔴 Critical | $5,000 — $10,000 |
| 🟠 High | $1,000 — $5,000 |
| 🟡 Medium | $250 — $1,000 |
| 🟢 Low | $100 — $250 |

### Security Practices

- Smart contracts will be audited by a Tier-1 security firm (Phase 3)
- All API keys are server-side only — never exposed to frontend
- Wallet connections are read-only until user explicitly approves transactions
- No private keys or seed phrases are ever collected

---

## 🌐 Community

<div align="center">

| Platform | Link | Purpose |
|---|---|---|
| 🐦 Twitter / X | [@solasidofun](https://twitter.com/solasidofun) | News & announcements |
| 💬 Discord | Coming soon | Community & support |
| 📱 Telegram | Coming soon | Quick updates |
| 🌐 Website | [mangamusic.xyz](https://mangamusic.xyz) | Main platform |
| 🤗 Hugging Face | Demo Space | Live demo |

</div>

### Stay Updated

Follow [@solasidofun](https://twitter.com/solasidofun) on X for:
- 🚀 Phase announcements
- 🎁 Airdrop eligibility updates
- 🎵 New feature demos
- 🗺️ Roadmap progress

---

## 🖼️ Brand Assets

All brand assets are available in the `/assets` directory:

| Asset | File | Size | Usage |
|---|---|---|---|
| Logo | `manga_music_logo.jpg` | 800×800 | Profile pictures, icons |
| Cover | `manga_music_cover.jpg` | 1500×500 | Twitter/X banner |
| Product 1 | `manga_product_1_prompt.jpg` | 1080×1080 | Social media posts |
| Product 2 | `manga_product_2_nft.jpg` | 1080×1080 | NFT promotion |
| Product 3 | `manga_product_3_howto.jpg` | 1080×1080 | Tutorial posts |
| Roadmap | `manga_music_roadmap.png` | 1200×1800 | Roadmap sharing |
| Promo 01–10 | `promo_0X_*.png` | 1080×1080 | Campaign posts |

> ✅ Brand assets may be used for community promotion with credit to **@solasidofun**.
> ❌ Do not alter the logo or use assets to misrepresent the project.

---

## 📊 Stats

<div align="center">

![GitHub Stars](https://img.shields.io/github/stars/solasidofun/manga-music?style=social)
![GitHub Forks](https://img.shields.io/github/forks/solasidofun/manga-music?style=social)
![GitHub Issues](https://img.shields.io/github/issues/solasidofun/manga-music)
![GitHub PRs](https://img.shields.io/github/issues-pr/solasidofun/manga-music)

</div>

---

## 📄 Documentation

| Document | Status | Link |
|---|---|---|
| Whitepaper v1.0 | 🟡 In Progress | Coming Phase 1 |
| API Docs | 🟡 In Progress | Coming Phase 2 |
| Smart Contract Docs | 🟡 In Progress | Coming Phase 2 |
| Security Audit Report | ⚪ Planned | Coming Phase 3 |
| Integration Guide | ⚪ Planned | Coming Phase 2 |

---

## ⚖️ License

```
MIT License

Copyright (c) 2025 MANGA MUSIC / @solasidofun

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

See [LICENSE](LICENSE) for full text.

---

## ⚠️ Disclaimer

> MANGA MUSIC is an experimental Web3 project currently in **beta / development phase**. 
> Token and NFT values are speculative. This is not financial advice.
> Always do your own research (DYOR) before participating in any crypto project.
> Never invest more than you can afford to lose.

---

<div align="center">

**Built with ❤️ and manga energy by [@solasidofun](https://twitter.com/solasidofun)**

<br/>

```
╔═══════════════════════════════════════╗
║      MANGA MUSIC · ON SOLANA          ║
║   Type a prompt. Get a track.         ║
║   Own it forever.                     ║
╚═══════════════════════════════════════╝
```

⭐ **Star this repo if you believe in the future of AI music on Web3!** ⭐

</div>
