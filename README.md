# PolyBot - Autonomous Polymarket Trading Terminal

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Tech Stack](https://img.shields.io/badge/stack-MERN-informational)
![Web3](https://img.shields.io/badge/Web3-Polymarket-purple)

## 📖 Overview
PolyBot is a high-performance, user-hosted algorithmic trading bot designed specifically for Web3 prediction markets via Polymarket. Built entirely on the MERN stack, it operates exclusively on the client's local machine or personal cloud. This decentralized architecture guarantees absolute privacy, ultra-low latency, and total user custody over their funds, API keys, and proprietary trading logic.

The system acts as a rapid-execution bridge between off-chain market data and on-chain trade execution, ingesting real-time data streams via WebSockets and receiving precise trade signals via TradingView webhooks.

## ✨ Core Features
* **100% Local Execution:** No centralized company servers. Total privacy and ownership of your API keys and trading logic.
* **Ultra-Low Latency:** Utilizes WebSockets and Node.js `worker_threads` to process live data and execute trades instantly on the Polymarket CLOB.
* **TradingView Integration:** Seamlessly accepts POST webhook signals directly from your custom TradingView alerts.
* **Advanced Analytics Dashboard:** Real-time React frontend featuring:
  * Live P&L charting (TradingView Lightweight Charts)
  * Segmented trade distribution (Recharts pie charts)
  * Calendar-based profit/loss heatmap (Nivo)
  * Real-time metrics: Sharpe ratio, profitable trade ratio, open position value, and total fees spent.

## 🛠️ Technology Stack
* **Frontend:** React.js, Zustand (State Management), Socket.io-client
* **Backend:** Node.js, Express.js, WebSockets (`ws`), Worker Threads
* **Database:** MongoDB (Local instance), Mongoose
* **Web3 Integration:** `ethers.js` (v6), `@polymarket/clob-client`

## 🚀 Getting Started

### Prerequisites
* Node.js (v18+)
* Local MongoDB instance or Docker Desktop
* A funded Polymarket (Polygon) wallet and API credentials
* TradingView account (for webhook signals)

### Installation (Local Development)
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/tirth707/poly-bot.git](https://github.com/tirth707/poly-bot.git)
   cd poly-bot
