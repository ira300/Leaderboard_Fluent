# 🧾 Leaderboard Fluent

Smart contract to maintain a leaderboard on the Fluent devtnet. Players can submit scores with a small fee, and the highest scorers stay at the top!

---

## 🚀 Technologies Used

- [Hardhat](https://hardhat.org/)
- [Ethers.js](https://docs.ethers.org/)
- [Solidity ^0.8.19](https://docs.soliditylang.org/)
- [Fluent devnet](https://blockscout.dev.gblend.xyz)
- [dotenv](https://www.npmjs.com/package/dotenv)

---

## ⚙️ Installation

### 1. Clone the repository

```
git clone https://github.com/ira300/Leaderboard_Fluent
cd Leaderboard_Fluent
```
---

### 2. Install dependencies
```
npm install
```

---
### 3. Set up environment variables
Edit your hardhat.config.js file by placing your private key

```
nano hardhat.config.js
```
---
### hardhat.config.js
````
module.exports = {
  networks: {
    zerog: {
      url: "https://rpc.dev.gblend.xyz/",
      chainId: 20993,
      accounts: [`Your Private Key`], 
    },
  },
````
---
PRIVATE_KEY=your_private_key_here
⚠️ Never share your private key! Use a test account wallet for safety.

---

### 📦 Compile the contracts
```
npx hardhat compile
```
---
🚀 Deploy to Fluent testnet
```
npx hardhat run scripts/deploy.js --network fluent_devnet1
```
