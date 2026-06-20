# 🤝 Contributing to Metaverse Rang Blockchain ABI

Thank you for your interest in contributing to the **Metaverse Rang Blockchain ABI Repository** 🚀

This repository contains **smart contract ABIs, interface definitions, and blockchain interaction schemas** used across the Metaverse Rang ecosystem (NFTs, Assets, VOD, and Metaverse services).

Your contributions help improve **on-chain interoperability, contract reliability, and Web3 integration standards**.

---

## 🌍 Code of Conduct

By participating in this project, you agree to:

- Be respectful and professional in all interactions
- Avoid offensive, toxic, or harmful language
- Focus on technical discussions and improvements
- Respect differing opinions and design decisions
- Maintain a collaborative and open-source mindset

---

## 🧠 What You Can Contribute

We welcome contributions in the following areas:

### 📜 ABI Improvements
- Adding new smart contract ABIs
- Updating existing ABI versions
- Fixing incorrect or outdated function definitions

### 🔗 Blockchain Integration
- Improving contract interface compatibility
- Supporting multi-chain ABI structures (Ethereum, Polygon, etc.)
- Adding event definitions and logs

### 🧾 Documentation
- Improving ABI explanations
- Adding usage examples
- Writing integration guides for developers

### ⚡ Optimization & Validation
- Ensuring ABI correctness against deployed contracts
- Removing redundant or invalid definitions
- Standardizing formatting and structure

---

## 📦 Getting Started

### 1. Fork the Repository

Click **Fork** on GitHub to create your own copy.

---

### 2. Clone Your Fork

```bash
git clone https://github.com/YOUR_USERNAME/Metaverse-Rang-BlockChain-ABI.git
cd Metaverse-Rang-BlockChain-ABI
```

---

### 3. Create a New Branch

Use meaningful branch names:

```bash
git checkout -b feature/add-nft-contract-abi
```

Examples:

- feature/update-nft-abi
- fix/erc721-event-definition
- refactor/abi-structure
- docs/add-integration-guide

---

### 4. Make Your Changes

Ensure:

- ABI format is valid JSON
- Functions match deployed smart contracts
- Events are properly defined
- No duplicate or conflicting entries

Example ABI structure:

```json
[
  {
    "inputs": [],
    "name": "totalSupply",
    "outputs": [
      {
        "internalType": "uint256",
        "name": "",
        "type": "uint256"
      }
    ],
    "stateMutability": "view",
    "type": "function"
  }
]
```

---

### 5. Validate Changes

Before submitting:

- Ensure JSON is valid
- Ensure ABI matches contract interface
- Test in Web3 environment (Hardhat / Foundry / Remix)
- Verify event decoding works correctly

---

## 🧪 Testing Guidelines

If your change affects ABI behavior:

- Test with `ethers.js` or `web3.js`
- Validate contract calls
- Check event parsing
- Ensure backward compatibility

Example test:

```js
const contract = new ethers.Contract(address, abi, provider);
const result = await contract.totalSupply();
console.log(result.toString());
```

---

## 🧾 Commit Convention

We use **Conventional Commits**:

```bash
feat: add new NFT marketplace ABI
fix: correct Transfer event signature
docs: improve ABI usage guide
refactor: restructure contract interfaces
chore: update ABI versioning
```

---

## 🔀 Pull Request Process

### Before opening a PR:

- Ensure ABI is valid JSON
- Ensure no breaking changes (or clearly documented)
- Ensure compatibility with existing services

---

### PR Requirements:

- Clear description of changes
- Contract address or reference (if applicable)
- Reason for update
- Related issue (if any)

Example:

```text
Closes #15
```

---

## ⚠️ ABI Quality Rules (VERY IMPORTANT)

All contributions MUST follow:

- ABI must strictly match deployed smart contract
- No experimental or fake interfaces
- No missing event definitions
- No duplicate function signatures
- Maintain Ethereum ABI standard compliance

---

## 🔐 Security Guidelines

- Never include private keys or secrets
- Do not expose sensitive contract data
- Validate all ABI inputs
- Ensure no malicious or misleading interfaces

---

## 🌐 Multi-Chain Support

If adding support for multiple chains:

- Clearly separate ABI versions
- Document chain compatibility
- Include metadata for chain IDs if needed

Example:

```json
{
  "chainId": 1,
  "contract": "ERC721",
  "abi": [...]
}
```

---

## 📡 Versioning Rules

ABI updates must follow semantic versioning:

- MAJOR → breaking ABI change
- MINOR → new functions/events added
- PATCH → fixes or corrections

---

## 🚨 Reporting Issues

If you find a problem:

Please include:

- ABI file affected
- Expected behavior
- Actual behavior
- Contract reference (if available)

---

## 🌱 Feature Requests

We welcome ideas such as:

- New contract integrations
- Cross-chain ABI compatibility
- Standardization improvements
- Event indexing enhancements

---

## 🏆 Recognition

All contributors are recognized as part of the **Metaverse Rang Blockchain Infrastructure Team**.

Your contributions help build:

- Decentralized NFT infrastructure
- Cross-chain asset standards
- Metaverse interoperability layer

---

## 🚀 Thank You

Together we are building a **standardized blockchain interface layer for the Metaverse economy** 🌐
