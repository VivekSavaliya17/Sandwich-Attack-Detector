UniswapV2 Sandwich Attack Detector

A backend–frontend based security tool designed to detect sandwich attacks occurring on Uniswap V2 decentralized exchange transactions.
This project analyzes Ethereum transactions to identify malicious front-run and back-run patterns used by MEV bots to exploit users.


Project Overview

A sandwich attack is a type of Miner Extractable Value (MEV) exploit where an attacker :

1. Front-runs a victim’s transaction
2. Lets the victim’s trade execute
3. Back-runs another transaction to profit from price manipulation


This project aims to :

1. Detect such patterns in Uniswap V2 swaps
2. Flag suspicious transactions
3. Provide a basic visualization through a frontend interface


Features :

1. Detects front-run & back-run transaction patterns
2. Uses Ethereum transaction data
3. Backend logic to analyze Uniswap V2 swaps
4. React-based frontend for interaction
5. Local execution without Docker
6. Suitable for research & academic projects


Tech Stack :

Backend - 

 - Node.js
 - Express.js
 - Web3 / Ethers.js
 - Ethereum transaction analysis logic

Frontend - 

 - React 
 - JavaScript
 - HTML / CSS


Project Structure :

```
Sandwich-Attack-Detector/
│
├── backend/
│   ├── server.js
│   ├── routes/
│   ├── controllers/
│   ├── package.json
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│
└── README.md
```


Installation & Setup :

Prerequisites - 

 - Node.js (v16+ recommended)
 - npm
 - Git
 - Internet connection (for Ethereum RPC)


Clone the Repository :

```
git clone https://github.com/Pooja-1504/Sandwich-Attack-Detector.git
cd Sandwich-Attack-Detector
```

Running the Backend :

```
cd backend
npm install
npm run dev
```

Backend runs on:

```
http://localhost:5000
```

Running the Frontend :

Open a new terminal:

```
cd frontend
npm install
npm start
```

Frontend runs on:

```
http://localhost:3000
```

Workflow :

1. User interacts with the frontend
2. Frontend sends requests to backend API
3. Backend analyzes Uniswap V2 transactions
4. Suspicious sandwich attack patterns are detected
5. Results are displayed on the frontend


Use Cases :

* Academic research on MEV attacks
* Learning Ethereum transaction analysis
* Cybersecurity & blockchain projects
* Demonstration for hackathons & viva exams


Limitations :

* Focused only on **Uniswap V2**
* Detection is heuristic-based
* Not optimized for mainnet-scale real-time monitoring
* No automated prevention (detection only)


Author :

Vivek Savaliya
Cyber Security Enthusiast

🔗 GitHub: https://github.com/VivekSavaliya17/Sandwich-Attack-Detector


License :

This project is for **educational and research purposes only.
Not intended for production or financial trading systems.
