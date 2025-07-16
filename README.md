# 🏗️ BuildChain

> A decentralized construction funding platform powered by smart contracts on the Tezos blockchain.

BuildChain enables contractors to publish real-world construction projects for commercial trades, raise funds from investors, and share profits transparently. This platform combines Web3 wallet access, milestone-based payments, and smart contract–governed logic to reduce risk, increase access to capital, and build trust in the contruction industry.

---

## 🚀 Features

- ✅ Smart contract in JsLIGO with:
  - Investor contributions with cap and share tracking
  - Contractor-controlled time-based fund releases
  - Profit distribution (e.g. 49% contractor / 51% investors)
  - Grace period (30–90 days) for client payments
  - Refund logic and verification through check images, videos, and documentation

- 🌐 Frontend (React or HTML):
  - Connect wallet via Beacon
  - Deploy contract to Tezos mainnet or Ghostnet
  - Track project status, due date, and proof of profit
  - View construction progress images (investors only)
  - $50 XTZ viewer fee credit toward investment

- 🔐 Secure investor-only content access
- 📅 Flexible timeframe support for both small and large-scale projects

---

## 📦 Project Structure

```
buildchain/
├── contract/
│   └── SmartContract.jsligo        # JsLIGO smart contract
├── deploy/
│   └── deploy.html                 # HTML + JS frontend for deploying the contract
├── README.md                       # This file
```

---

## ⚙️ Getting Started

### 🧱 Prerequisites
- [Node.js](https://nodejs.org) (if using React frontend)
- [LIGO CLI](https://ligolang.org/docs/intro/installation)
- Tezos-compatible wallet (e.g., Temple or Beacon extension)

### 🔧 Compile the Smart Contract
```bash
ligo compile contract contract/SmartContract.jsligo -o contract/SmartContract.tz
```

### 🌐 Deploy via HTML (No backend required)
1. Open `deploy/deploy.html`
2. Connect your wallet (configured to Ghostnet or Mainnet)
3. Enter project values and click **Deploy Contract**

---

## 🌍 Deployment Targets

- **Testnet**: [https://ghostnet.ecadinfra.com](https://ghostnet.ecadinfra.com)
- **Faucet for Test XTZ**: [https://faucet.ghostnet.teztnets.xyz](https://faucet.ghostnet.teztnets.xyz)

---

## 📃 License

Apache 2.0. See `LICENSE` file for details.

---

## 💡 Future Roadmap
- 🗳️ Investor voting to release funds
- 📷 Image upload to check and monitor progress of project
- 🏛️ DAO structure for project selection and arbitration
- 📱 Progressive Web App for mobile access

---

## 🤝 Contributing
We welcome community contributions. Submit PRs or open issues to suggest features, fixes, or improvements.

---

## 🙌 Credits
Built with ❤️ from Delaware using Taquito, Beacon, and JsLIGO by BRO Builder LLC.
