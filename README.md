![w3b3_agent](https://github.com/user-attachments/assets/428c6e5c-b382-4feb-8123-40f53a0fc0fe)

<p align="center">
      <b>🤖 WEB3_AGENT - AI POWERD WEB3 IMAGE GENERATOR AGENT BOT</b>
</p>
<p align="center">
    <img src="https://img.shields.io/badge/Open%20Source-Yes-cyan?style=flat-square">
<img src="https://img.shields.io/badge/Version-0.1-green?style=for-the-badge"><img src="https://img.shields.io/github/license/bild96/smart-agent?style=for-the-badge&color=blue">
</p>
<p align="center">
    Documentation: <a href="https://docs.galadriel.com" target="_blank">docs.galadriel.com</a>
</p>

## Overview

w3b3_Agent is a Galadriel the first L1 for AI.

It captures the fusion of AI, blockchain, and real-time digital art creation.

Ethereum enabled writing smart contracts to build dApps. Similarly, Galadriel enables developers to build AI apps & agents like smart contracts — decentralized and on-chain. We support a range of AI usage: from simple LLM features in existing dApps to highly capable AI agents like on-chain AI hedge funds, in-game AI NPCs and AI-generated NFTs.

Galadriel is built on a parallel-execution EVM stack which enables high throughput and low latency while providing a familiar experience to Solidity developers. It brings AI inference on-chain in a low-cost, low-latency manner through teeML (Trusted Execution Environment Machine Learning) which allows querying open and closed-source LLM models in a verifiable way.

## 🏁 Quickstart

This quickstart covers two things:
* Deploying an AI app to the Galadriel devnet
* Calling your deployed AI app and viewing the results

## 🔥 Prerequisites
 A Galadriel devnet [account](https://docs.galadriel.com/setting-up-a-wallet). We recommend creating a new EVM account for development purposes.
    Some [devnet tokens](https://docs.galadriel.com/faucet) on the account you are using.
    node and npm installed on your machine.

## Deploying a contract on Galadriel devnet:
1. devnet tokens
Get yourself some devnet tokens from the [faucet](https://docs.galadriel.com/faucet).
2. Clone repository
Clone the repo that contains Galadriel example contracts and the oracle implementation.
```
git clone https://github.com/bild96/w3b3_agent.git
cd w3b3_agent/contracts
```
3. Setup environment
Use the ||template.env|| file to create a ||.env|| file:

# Starting in repo root
```
cp template.env .env
```
Then, modify the ||.env|| file:
- Set ||PRIVATE_KEY_GALADRIEL|| to the private key of the account you want to use for deploying the contracts to Galadriel devnet.
- Set ||ORACLE_ADDRESS|| to the [current devnet oracle address](https://docs.galadriel.com/oracle-address) provided by Galadriel team: 0x4168668812C94a3167FCd41D12014c5498D74d7e.

4. Install dependencies
   Install the dependencies using npm:
```
   # In repo root -> /contracts
   npm install
 ```
5. Deploy contract to devnet
   The [quickstart contract](https://github.com/galadriel-ai/contracts/blob/main/contracts/contracts/Quickstart.sol) can be deployed with a [simple script](https://github.com/galadriel-ai/contracts/blob/main/contracts/scripts/deployQuickstart.ts):
  ```
npm run deployQuickstart
```
The output of the script will show the deployed contract address. Store this and export it in terminal to call the contract later:

# Replace with your own contract address
```

export QUICKSTART_CONTRACT_ADDRESS=0x...
```

## 💡 Calling your contract
Prerequisites:
- You’ve deployed the quickstart contract in the previous step, and stored the contract address.
  Execute the following command to run a [script](https://github.com/galadriel-ai/contracts/blob/main/contracts/scripts/deployQuickstart.ts) that calls the

 
 # deployed contract:

   ```
  npm run callQuickstart
  ```

The script will interactively ask for the input (DALL-E prompt: what image should be generated) and then call the contract with the input. The output, when ready, will be printed to the console.
If this step fails, make sure you have set the ||QUICKSTART_CONTRACT_ADDRESS|| environment variable to the address of your deployed contract.

🎉 You’re done! You’ve successfully created and called your own Web3 image generator agent bot.

## ⛏️ Built With <a name = "tech_stack"></a>
<img alt="Dockerfile" src="https://img.shields.io/badge/Dockerfile-%23000.svg?&style=for-the-badge&logo=Dockerfile&logoColor=white"/>
<img alt="Solidity" src="https://img.shields.io/badge/Solidity-%23E34F26.svg?&style=for-the-badge&logo=Solidity&logoColor=white"/><img alt="python" src="https://img.shields.io/badge/python-%231572B6.svg?&style=for-the-badge&logo=python&logoColor=yellow"/><img alt="Typescript" src="https://img.shields.io/badge/typescript-%23563D7C.svg?&style=for-the-badge&logo=typescript&logoColor=white"/>

## ✍️ Authors <a name = "authors"></a>

 🧑‍💻 [Bild96](https://x.com/bild96)


## 🎉 Acknowledgments <a name = "acknowledgments"></a>
 🏗️ [ETHonline2024 © 2024](https://ethglobal.com)
  <h1 align="left">
  <a href="https://discord.gg/ethglobal"><img src="static/Join-Discord.png" width="380" alt="Join Discord"></a>
 </h1>
 
#### 🪙 Want to show support? Just spread the word and smash the ⭐ star button
###### Donate ETH: ***0xfd7a470001364d707c81074142b6aC9248B0b0cc***
