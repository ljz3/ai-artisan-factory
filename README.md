# AI Artisan Factory

## Overview

This project allows users to generate art in many different styles using OpenAI's DALL·E API and mint it as an NFT either in the AI Artisal collection or as its own collection.

## Contents

- [About Me](#about-me)
- [Tech Stack](#tech-stack)
  - [Stack Decisions](#stack-decisions)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Setup](#setup)
  - [Testing](#testing)
  - [Deployment](#deployment)
- [Goerli Deployments](#goerli-deployments)
- [Work In Progress](#work-in-progress)

## About Me
Hello, my name is Kevin, and I am formerly Team Lead of Uniblock's API, No-code Smart Contracts & SDK team. I also have experience working on other large projects such as Parallel NFT, with a strong track record of architecting, implementing, and deploying various features using the latest blockchain technology. Additionally, my skills in identifying, architecting and implementing complex blockchain APIs and No-code Smart Contracts that the market demands have been honed through working closely with the rest of leadership at Uniblock.

All the technologies listed below are ones I have prior professional experience with.

### Languages
- Solidity
- Typescript
- Javascript

### Smart Contracts
- Tokens (ERC20/ERC777)
- NFTs (ERC721/ERC1155)
- DeFi (DEX/AMM)
- Factories
- Clones/Proxies
- Smart Wallets
- Multisig
- OpenZeppelin Contracts
- Merkle Trees/Proofs
- NFT Marketplace
- DAOs
- On-chain Price Oracles
- EVM Mainnets + Testnets
- IPFS
- Chainlink VRF
- Hardhat/Mocha/Chai

### Blockchain Integration
- The Graph (Blockchain Event Indexer)
- Ethers.js
- EVM RPC Nodes
- Bridging
- Etherscan API
- Coingecko API
- Moralis SDK/API
- Metamask

### Full Stack
- Nestjs
- PrismaORM
- Firebase
- PostgreSQL
- Nodejs
- Redis
- BullMQ
- Jest
- React & React Native
- API Gateway
- Google Cloud Platform (GCP)
- Load Balancing
- Nextjs
- Tailwind CSS

### Other
- Github Actions
- OpenAI/ChatGBT/Dall-E API
- Ticketing Systems (Zenhub/Trello)
- Agile Development
- Figma
- AdobeXD

## Tech Stack

### Smart Contracts
- Solidity
- Typescript
- OpenZeppelin Contracts
- IPFS
- Hardhat/Mocha/Chai

### Backend
- Firebase Cloud Functions
- Firebase Firestore
- Typescript
- OpenAI SDK
### Frontend
- Nextjs
- Typescript
- Metamask
- Ethers
- Deployment on Vercel

## Stack Decisions
- The reason for using Firebase as the backend is because it is lightweight and extremely cheap to run compared to hosting on GCP/AWS/Azure for smaller projects. Also since this project does not store a lot of data, Firestore makes sense as a database options as hosting a database on the cloud is overkill for a small project like this.
- A backend is required for this project is for security reasons. API keys can be exposed if all the API calls to pin files and generate art are done in the front end.
- The reason for using Nextjs for the frontend is because it is very quick to setup CI/CD on Vercel, all while Vercel hosts the site for free.

## Getting Started

### Prerequisites

- Node.js (Recommended version: latest)
- Solidity (version: ^0.8.17)

### Setup

Go to the root folder of the project in terminal:

1. Install dependencies with `npm install` or `yarn install`
2. Setup the environment variables by creating a `.env` file inside the root directory. Then fill out the environment variables in accordance with `.env.example`

### Testing

1. `yarn test` to compile the contracts and run the test suites for the smart contracts

### Deployment

1. `yarn compile` to compile the contracts
2. `yarn deploy:goerli` to deploy the contracts to Ethereum Goerli Testnet
3. `yarn verify:goerli` to verify the contracts on https://goerli.etherscan.io/