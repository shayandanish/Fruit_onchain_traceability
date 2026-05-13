# 🍎 VerdantChain: Fruit On-Chain Traceability

**VerdantChain** is a blockchain-powered food traceability system designed to bring transparency and trust to the fruit supply chain. By leveraging Ethereum smart contracts, every step of a fruit's journey—from the farm to the consumer—is recorded immutably on-chain.

## 🚀 Live Demo
Check out the live application here:  
**[https://shayandanish.github.io/Fruit_onchain_traceability/index.html](https://shayandanish.github.io/Fruit_onchain_traceability/index.html)**

---

## ✨ Key Features

- **🌱 Farm Registration**: Farmers can register batches with harvest dates, origin, and initial quality metrics.
- **🚚 Logistics Tracking**: Transporters and warehouses append data (temperatures, facilities, vehicle names) as the fruit moves.
- **📱 Mobile Support**: Seamlessly connect MetaMask on mobile browsers (Chrome/Safari) via deep linking—no desktop required.
- **🔍 Consumer Transparency**: Anyone can scan a QR code to view the entire journey. **No wallet or app required** for viewing records.
- **🛡️ Immutable Records**: Once recorded on the blockchain, the data cannot be tampered with or deleted.
- **⚡ Real-time Verification**: Instant proof of provenance for distributors and retailers.

---

## 🛠️ Technology Stack

- **Smart Contracts**: Solidity
- **Development Environment**: Hardhat
- **Frontend**: HTML5, Vanilla CSS3 (Custom Design System), JavaScript
- **Blockchain Interaction**: Web3.js / Ethers.js
- **Deployment**: Vercel / GitHub Pages

---

## 📂 Project Structure

```text
├── backend/            # Hardhat project, Solidity contracts, and deployment scripts
├── frontend/           # Main application logic and UI components
│   ├── index.html      # Main Dashboard
│   ├── qrcode.html     # QR Scanner Interface
│   └── abi.js          # Contract ABI and Address configuration
├── index.html          # Project Landing Page
└── contract/           # Smart contract source files
```

---

## ⚙️ How It Works

1. **Harvest**: The farmer registers a new batch on the blockchain, generating a unique Batch ID.
2. **Transit**: Logistics providers update the batch status at each checkpoint (Warehouse, Transport, Retail).
3. **Scan**: The final consumer scans a QR code (linked to the Batch ID) to see the full timeline of the fruit they are buying.

---

## 🔧 Local Development

### Prerequisites
- Node.js & npm
- MetaMask browser extension

### Setup
1. **Clone the repository**:
   ```bash
   git clone https://github.com/shayandanish/Fruit_onchain_traceability.git
   ```
2. **Install Backend Dependencies**:
   ```bash
   cd backend
   npm install
   ```
3. **Deploy Locally**:
   ```bash
   npx hardhat node
   npx hardhat run scripts/deploy.js --network localhost
   ```
4. **Run Frontend**:
   Simply open `index.html` in your browser or use a Live Server extension.

---

## 📄 License
This project is licensed under the MIT License.

---

Created with ❤️ by [Shayan Danish](https://github.com/shayandanish)