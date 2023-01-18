# Dappazon
Dappazon is a blockchain-based marketplace inspired by Amzon.com that enables crypto payments and intermediary-free exchange of goods between a seller and buyers. Buyers can view the origins and history of goods stored on the blockchain, which builds trust in the seller and makes the deals more transparent.
The system will provide an automated transfer of ownership along with immutable purchase history records.
Each item has an image stored in the IPFS.


## Project architecture
<p align="center">
  <img src="./project documentation/project architecture.png" width="700" title="Project architecture" alt="Project architecture">
</p>


## Blockchain interaction with IPFS
In addition to blockchain, we are using IPFS (interplanetary file system) to host the products’ pictures and we store references to those pictures on the blockchain.
<p align="center">
  <img src="./project documentation/ipfs.png" width="700" title="Blockchain interaction with IPFS" alt="Blockchain interaction with IPFS">
</p>


## Technology Stack & Tools

- Solidity (Writing Smart Contracts)
- Javascript (React & Testing)
- [Hardhat](https://hardhat.org/) (Development Framework)
- [Ethers.js](https://docs.ethers.io/v5/) (Blockchain Interaction)
- [React.js](https://reactjs.org/) (Frontend Framework)
- [Metamask](https://metamask.io/) (trailblazing tool enabling user interactions and experience on Web3)

## Requirements For Initial Setup
You have two options: 
- Install [NodeJS](https://nodejs.org/en/)
- Install [Docker](https://www.docker.com/)

## Setting Up
### 1. Clone/Download the Repository
If you want to use docker run the following command:
```shell
docker run -it --rm -v ${PWD}:/work -w /work -p 8545:8545 -p 3000:3000 --entrypoint /bin/bash node:14.16.0
```

### 2. Install Dependencies:
```shell 
npm install
```

### 3. Run tests
```shell 
npx hardhat test 
```

### 4. Start Hardhat node
```shell
npx hardhat node
```

### 5. Run deployment script
In a separate terminal execute:
```shell 
npx hardhat run ./scripts/deploy.js --network localhost
```

### 6. Start frontend
```shell
npm run start
```
