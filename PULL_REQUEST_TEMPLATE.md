# 🚀 Pull Request – Metaverse Rang Blockchain ABI

Thank you for contributing to the **Metaverse Rang Blockchain ABI Repository** 🌐

Please complete this template to help reviewers validate ABI correctness, compatibility, and blockchain integrity.

---

## 📌 Description

Provide a clear description of your changes:

- What ABI or contract interface was modified?
- What problem does this solve?
- Why is this change necessary?

---

## 🔗 Related Issue

- Closes #ISSUE_NUMBER
- Related to #ISSUE_NUMBER

If no issue exists, describe context briefly.

---

## 🧩 Type of Change

Please select the type of change:

- [ ] 🆕 New ABI / Contract Interface
- [ ] 🐛 Bug Fix (ABI correction)
- [ ] 🔄 ABI Update (version change)
- [ ] ⚡ Optimization / Cleanup
- [ ] 📚 Documentation update
- [ ] 🔗 Multi-chain support addition
- [ ] ♻️ Refactor (structure improvement)

---

## 📜 ABI / Contract Details

### Contract Name:
```
e.g. NFTMarketplace / ERC721 / AssetRegistry
```

### Contract Address (if applicable):
```
0x...
```

### Network:
- [ ] Ethereum
- [ ] Polygon
- [ ] BSC
- [ ] Other: ________

---

## 🧾 Changes Summary

Explain what changed in the ABI:

- Functions added/removed/modified:
- Events added/updated:
- Input/output changes:

---

## 📦 ABI Diff (Optional but Recommended)

```diff
+ added function: mintNFT(address to, uint256 tokenId)
- removed function: oldMint()
```

---

## 🧪 Validation Checklist

Please confirm:

- [ ] ABI is valid JSON
- [ ] ABI matches deployed smart contract
- [ ] Events are correctly defined
- [ ] No duplicate function signatures
- [ ] No breaking changes without version bump
- [ ] Tested with ethers.js / web3.js

---

## 🔍 Testing

Describe how you validated the ABI:

- [ ] Hardhat tests
- [ ] Foundry tests
- [ ] Remix testing
- [ ] Manual Web3 interaction
- [ ] No testing required (documentation update only)

### Example test:

```js
const contract = new ethers.Contract(address, abi, provider);
const result = await contract.totalSupply();
console.log(result.toString());
```

---

## ⚠️ Breaking Changes

- [ ] No breaking changes
- [ ] Yes (describe below)

If yes:

- What breaks?
- Migration steps?

---

## 🔐 Security Checklist

- [ ] No private keys or secrets exposed
- [ ] ABI does not expose sensitive logic
- [ ] Input/output validation consistent
- [ ] No malicious or incorrect interface definitions

---

## 📡 Versioning

- [ ] Patch (fix)
- [ ] Minor (new feature)
- [ ] Major (breaking change)

Describe version impact:

---

## 🧠 Architecture Notes

- [ ] Follows ABI standard (Ethereum / EVM compatible)
- [ ] Compatible with existing services
- [ ] No unnecessary duplication
- [ ] Maintains schema consistency

---

## 💬 Additional Notes

Add any extra context or technical explanations:

---

## 🙏 Reviewer Focus

Please prioritize review on:

- [ ] ABI correctness
- [ ] Blockchain compatibility
- [ ] Event consistency
- [ ] Security implications
- [ ] Backward compatibility

---

## 🚀 Summary

Short description of this PR:

> This PR updates / adds / fixes ...
```
