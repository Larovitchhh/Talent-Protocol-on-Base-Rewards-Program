# Talent-Protocol-on-Base-Rewards-Program
Talent Protocol on Base: Rewards Program
Talent Protocol on Base: Rewards Program 
Header
Empowering builders with on-chain reputation and rewards on Base Network.
Welcome to Talent Protocol on Base: Rewards Program, a decentralized platform that integrates Talent Protocol’s on-chain reputation system with the Base Network to reward builders for their contributions. This repository contains the smart contracts, front-end components, and API integrations to power a rewards program where developers, creators, and innovators earn $TALENT tokens and ETH for building on Base. With Talent Protocol’s Builder Score and Base’s scalable infrastructure, we’re creating a vibrant ecosystem for talent discovery and recognition.
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![GitHub issues](https://img.shields.io/github/issues/yourusername/talent-protocol-base-rewards)
![GitHub stars](https://img.shields.io/github/stars/yourusername/talent-protocol-base-rewards)
 About the Project
Talent Protocol is a web3 professional network that aggregates verified reputation data under one on-chain identity, enabling builders to showcase their skills and earn recognition. On Base, a Layer 2 Ethereum scaling solution, Talent Protocol powers a rewards program to incentivize developers to build, contribute, and grow the ecosystem. The Builder Rewards program, sponsored by Base, distributes ETH weekly to active developers, while $TALENT tokens reward community engagement and reputation-building activities.

 Features
Builder Score Integration: Display your on-chain reputation score, calculated from contributions on GitHub, Base, and Talent Protocol’s API.

$TALENT Token Rewards: Earn $TALENT for referring users, building credentials, or boosting your Builder Score.

ETH Builder Rewards: Weekly ETH distributions to top Base developers, no applications required—just build

On-Chain Resumes: Create verifiable resumes using Talent Protocol’s smart contracts, integrated with Base’s Basenames.

Talent Mate AI: Interact with Talent Protocol’s AI agent on Base to analyze contributions and earn $TALENT rewards.

 Goals
Reward high-potential builders for their contributions to Base’s ecosystem.

Enhance trust and visibility through interoperable reputation data.

Foster a decentralized community of developers and innovators.

 Getting Started
Follow these steps to set up and run the project locally.
Prerequisites
Node.js (v16 or higher)

Yarn or npm

Hardhat for Ethereum smart contract development

MetaMask or another Ethereum wallet

A Base testnet account (e.g., Base Sepolia)

Alchemy or another Base RPC provider

Installation
Clone the Repository
bash

git clone https://github.com/yourusername/talent-protocol-base-rewards.git
cd talent-protocol-base-rewards

Install Dependencies
bash

yarn install

Or, if using npm:
bash

npm install

Configure Environment Variables
Create a .env file in the root directory and add:
env

PRIVATE_KEY=your_ethereum_wallet_private_key
ALCHEMY_API_KEY=your_alchemy_api_key
BASESCAN_API_KEY=your_basescan_api_key
TALENT_API_KEY=your_talent_api_key

Obtain a Talent API key from Talent Protocol’s developer portal.

Note: Never commit your .env file. Ensure it’s in .gitignore.

Compile Smart Contracts
bash

npx hardhat compile

Run the Front-End
bash

cd frontend
yarn start

The front-end will be available at http://localhost:3000.

Deployment
To deploy the smart contracts to Base testnet (e.g., Base Sepolia):
bash

npx hardhat run scripts/deploy.js --network base_sepolia

The $TALENT token contract is deployed on Base at: 0x9a33406165f562E16C3abD82fd1185482E01b49a.

 Usage
Create Your Talent Passport:
Connect your Ethereum wallet to the front-end.

Use the Talent Passport app to build your on-chain resume with skills, projects, and credentials.

Mint your Builder Score on-chain to boost visibility.

Earn Builder Rewards:
Build dApps or contribute to Base’s ecosystem (e.g., deploy contracts, participate in hackathons).

Every Monday, Talent Protocol distributes ETH to active developers based on on-chain activity, sourced from GitHub and Talent’s API. No forms required

Earn $TALENT Tokens:
Refer Users: Invite builders to Talent Protocol and earn $TALENT based on their Builder Score.

Boost Builder Score: Deposit $TALENT to increase your score (up to 4 points) or access premium features like custom Talent Names.

Interact with Talent Mate: Reply to talentmate.eth on Base to get your contributions analyzed and potentially earn $TALENT.

Build Credentials: Develop custom credentials for Talent Protocol and earn a revenue share if widely adopted.

Claim Basename Perks:
If your Builder Score is >50 and on-chain, claim a free Basename through the Builder Perks program.

Example
Interact with the platform using Talent Protocol’s JavaScript SDK:
javascript

const { TalentProtocol } = require('@talentprotocol/sdk');
const talent = new TalentProtocol('your-ethereum-address', 'your-talent-api-key');

async function createResume() {
  const resume = await talent.createResume({
    name: 'John Doe',
    skills: ['Solidity', 'React', 'Base'],
    projects: ['Base dApp Marketplace']
  });
  console.log('Resume created:', resume);
}

async function checkRewards() {
  const rewards = await talent.getBuilderRewards();
  console.log('Available rewards:', rewards);
}

createResume();
checkRewards();

