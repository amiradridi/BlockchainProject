# Dappazon
Dappazon is a clone of the amazon ecommerce application on the ethereum blockchain.
Each item has an image stored in the IPFS.

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
