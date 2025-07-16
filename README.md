# 🏗 BuildChain – Decentralized Construction Funding on Tezos

**BuildChain** is a decentralized smart contract and front-end application built on the Tezos blockchain. It enables verified contractors to raise community-based funding for trades on commercial construction projects while providing investors with transparent ROI sharing, milestone tracking, and proof-based fund unlocking.

---

## 🔧 Features

### 🧱 Smart Contract (JsLIGO)
- Investor funds are locked and transparently tracked on-chain.
- Contractors can withdraw an initial 30%, followed by time-based installments.
- Investors are credited for access fees if they proceed to invest.
- Profit is split: 49% to the contractor, 51% among investors based on contribution.
- Contractor must deposit profits back into the contract post-completion.
- Configurable project timeframe (30–90 days typical).
- Optional investor voting mechanism for milestone-based fund unlocking (future).

### 🌐 Web Interface (HTML/JS)
- **Connect Wallet** via Beacon
- **Fund Project** in ꜩ
- **Pay Viewer Fee** to view sensitive files
- **Mark Project as Complete** (Contractor only)
- **Deposit Profits** post-completion
- **Investor Dashboard** to track profit share
- **Project Listing Page** for public browsing
- **Project Detail Page** showing ROI, timelines, and access to invest

---

## 📁 Project Structure

```
UI/
├── interaction.html         # Full smart contract interaction panel
├── project-details.html     # Detailed view of one construction project
├── projects.html            # Public listing of active projects
├── deploy.html              # Smart contract deploy UI
```

---

## 🚀 Getting Started

### 1. Install Dependencies (Optional)
If you want to build or compile contracts locally:
```bash
npm install -g @ligolang/ligo
```

### 2. Compile JsLIGO to Michelson
```bash
ligo compile contract BuildChain.jsligo -o buildchain.tz
```

### 3. Deploy to Tezos Ghostnet
Use the `deploy.html` page or deploy manually:
```bash
tezos-client originate contract buildchain transferring 0 from <your-wallet> running buildchain.tz --init '<storage>' --burn-cap 1
```

---

## 🧪 Testing with Ghostnet

Change the contract address inside the front-end files:
```js
let contractAddress = "KT1..."; // Replace with your deployed Ghostnet contract address
```

Use [Temple Wallet](https://templewallet.com/) or Beacon-compatible wallet with testnet ꜩ.

---

## 💡 The Game-Changer: Trade-Based Funding
Unlike traditional real estate investments that lock up your money for months or years, BuildChain focuses on individual trades within large commercial projects.

Example:
- A 12-unit apartment building takes 8–12 months to build.
- But the concrete slab? That’s done in 7 days.
- Once the slab is poured and inspected, the builder gets paid within the next 30 days.
- And so do you.

🕒 Shorter timelines = faster returns.

## 💡 Use Case Example
- A contractor needs $10,000 to build a commercial concrete slab for a new coffee shop in town. The funds needed covers material, labor, and operation expenses. The bid was approved for $15000.
- 10 investors each contribute $1,000.
- Investor pays 50 ꜩ to access documents (credited back if they invest). This allow access to private information; such as; contract agreement, Licenses, schedule, blueprints, location, and client, goverment and/or private investor.
- Contractor receives 30% upfront to start pre-work, operation and/or finance material needed, then weekly payouts to cost labor.
- Project completes in one week and $5,000 in profit is deposited as soon as client make the payment (30 to 45 days).
- Contractor receives 49% ($2,450), and investors share 51% ($2,550) proportionally, meaning each investor receives $1250 after the job is completed and payment is made from client.
- Investor can benefit from commercial trade jobs, with a high ROI in a short period of time.

---

## 📜 License

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

---

## 🙌 Acknowledgments

- [Taquito](https://tezostaquito.io/) for Tezos JS toolkit  
- [Beacon Wallet SDK](https://docs.walletbeacon.io/)  
- Tezos Ghostnet for testnet support  
- JsLIGO by [LIGOlang](https://ligolang.org)

---

## 🔐 Security Notes

- Do not store confidential documents on-chain.
- Viewer fee prevents abuse and filters non-serious participants.
- Use IPFS or encrypted S3 to host sensitive docs.

---

## 📫 Contact

Have questions or want to partner with us?  
Reach out at **frans@brobuilder.llc**

## 🙌 Credits
Built with ❤️ from Delaware U.S. using Taquito, Beacon, and JsLIGO by BRO Builder LLC.
