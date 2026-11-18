<div align="center">

# 🌌 Metaverse-Rang-BlockChain-ABI
### **Smart Contract Suite & ABI Documentation — Production-Grade Ecosystem**

[![Solidity](https://img.shields.io/badge/Solidity-%5E0.8.24-383838?style=for-the-badge&logo=solidity&logoColor=white)](https://soliditylang.org/)
[![OpenZeppelin](https://img.shields.io/badge/OpenZeppelin_v5-Secure-4E5EE4?style=for-the-badge&logo=openzeppelin&logoColor=white)](https://openzeppelin.com/)
[![Foundry / Hardhat](https://img.shields.io/badge/Tested_with-Foundry_%2F_Hardhat-FF5722?style=for-the-badge&logo=fire&logoColor=white)](https://getfoundry.sh/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

</div>

---

## 📖 Table of Contents
- Project Overview
- Smart Contract Suite (11 Core Contracts)
- Installation & Setup
- System Architecture
- Security & Optimizations
- Testing & Gas Reporting
- Deployment
- Contributing
- License
- Contact & Support

---

## 🌟 Project Overview

**Metaverse-Rang-BlockChain-ABI** is a comprehensive, production-grade repository containing ABIs, artifacts, and documentation for the entire 11-contract ecosystem developed for the Metaverse Rang and Paradise Supply Chain (PSC) architecture. 

This suite integrates blockchain gaming mechanics, 13-level access control systems, Soulbound token structures, multi-tier ERC-1155 digital assets, decentralized exchange (DEX) pair factories, vesting schedules, and Merkle Tree whitelist verifications built on **Solidity 0.8.24** and **OpenZeppelin v5**.

### 🎯 Project Goals
- Provide production-ready, highly secure ABIs and smart contract interfaces for frontend integration (React/Next.js/Wagmi).
- Implement industry best practices including **`Ownable2Step`** security and **Custom Errors** for optimal gas efficiency.
- Seamlessly bridge gamified progression systems, token distribution, and supply chain tracking.

---

## 📦 Smart Contract Suite (11 Core Modules)

The ecosystem consists of 11 core production contracts tailored for high-performance Web3 operations:

1. **`LevelRewardNFT.sol`** — ERC-721 token managing reward badges and tiered achievements across levels with secure minter controls.
2. **`LevelKeyNFT.sol`** — Soulbound ERC-721 access keys enforcing non-transferable wallet-to-wallet restrictions for platform rooms and features.
3. **`LevelAssets1155.sol`** — Multi-tier ERC-1155 digital assets and items supporting both Soulbound and Transferable policies per asset category.
4. **`MerkleWhitelist.sol`** — Gas-efficient Merkle Tree verification engine handling secure whitelisting and distribution gates.
5. **`BatchUserStorage.sol`** — High-performance bulk data storage management for users and internal multi-token balances.
6. **`ProductionLevelSystem.sol`** — Core progression logic engine handling 13 levels, 7 steps per level, and XP requirements.
7. **`ThirteenLevelAccess.sol`** — Central access hub managing player registration, ETH payments for level upgrades, and room entry validation.
8. **`WhitelistWithLevels.sol`** — Initial registration gateway mapping user IDs, custom codes, and initial levels.
9. **`ThirteenLevelAccessWithWhitelist.sol`** — Integration bridge connecting whitelist data directly to automated NFT reward and key distribution.
10. **`WhitelistWithLevelsAdvanced.sol`** — Advanced whitelist implementation supporting dynamic wallet assignment to immutable user profiles.
11. **`UserStorage.sol`** — Comprehensive data container storing user profiles, multi-wallet balances (PSC, Blue, Red, Yellow, IRR, Satisfaction, Effect), and 3D Gem metadata (`.png` / `.fbx`).
12. **`ThirteenLevelAccessKey_Deployable.sol`** — Unified, heavily optimized single-contract variant designed to bypass mainnet bytecode limits while retaining full 13-level functionality.

---

## 🛠️ Installation & Setup

### Prerequisites
- Node.js >= 18.0.0
- npm >= 9.0.0
- Hardhat >= 2.19.0 / Foundry

### Installation Steps
```bash
# 1. Clone the repository
git clone [https://github.com/ParsaAbolhasani/Metaverse-Rang-BlockChain-ABI.git](https://github.com/ParsaAbolhasani/Metaverse-Rang-BlockChain-ABI.git)
cd Metaverse-Rang-BlockChain-ABI

# 2. Install dependencies
npm install

# 3. Compile contracts and generate ABIs/Artifacts
npx hardhat compile

🏗️ System Architecture & Security
Key Security Measures Implemented

    Ownable2Step: Upgraded from standard Ownable to prevent accidental ownership transfers to zero or incorrect addresses.

    Custom Errors: Replaced string-based reverts with gas-efficient custom errors across all 11 contracts.

    Soulbound Enforcement: Modern OpenZeppelin v5 _update hooks strictly prohibit unauthorized wallet-to-wallet transfers for access keys and specific assets.

    Reentrancy Protection: Integrated nonReentrant guards on all payment processing and asset-claiming pathways.

🚢 Deployment

To execute the master deployment script and automatically wire contract permissions (such as assigning minter roles to access controllers):
npx hardhat run scripts/deploy-psc-ecosystem.js --network sepolia

👨‍💻 Author & Core Team

    Lead Developer & Architect: Parsa Abolhasani Rad 
    Role: Senior Full-Stack Blockchain Developer & Web3 Engineer
    Affiliation: Member of the Senior Council / Association of Iranian Blockchain
    GitHub Profile: @ParsaAbolhasani

📄 License

This project is licensed under the MIT License. See the LICENSE file for details.
