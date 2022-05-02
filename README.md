# 

## About
Extend the [WChicks token](https://github.com/SolChicks/chicks-bridge-contracts/blob/master/hardhat/contracts/WChicks.sol)

## Implement
- Smart Contract  
> Language: Solidity  
> Framework: Hardhat  
> Networks: Rinkeby(Testnet), Ethereum(Mainnet)  
> Unit Test: Hardhat, Chai

- Front End
> Language: React  
> Framework: Nextjs  
> Network: Rinkeby(Testnet)

## Installation
```shell
yarn install
```

## Usage

### 1. Environment variables
- Create a `.env` file in `pacakges/smart-contract` with its values (refer `.env.sample` file)
```
INFURA_API_KEY=[INFURA_API_KEY]
PRIVATE_KEY=[DEPLOYER_PRIVATE_KEY]
ETHERSCAN_API_KEY=[ETHER_SCAN_API_KEY]
REPORT_GAS=<true_or_false>
```
- Create a `.env` file in `pacakges/front-end` with its values (refer `.env.sample` file)
```
REACT_APP_NETWORK_URL=[NETWORK_RPC_URL]
REACT_APP_CHAIN_ID=[NETWORK_CHAIN_ID]
```

### 2. Build
Build Smart Contract and Front End Code
```shell
yarn build
```

### 3. Test
Unit Test in Smart Contract and Front End
```shell
yarn test
```

### 4. Deploy Contract
Deploy Smart Contract on ropsten testnet and publish the contract`s ABI to the Front End side.

- Run Deploy Command
```shell
yarn deploy
```

### 5. Verify Contract
Verify contract with the deployed constract address

```shell
yarn verify <DEPLOYED_ADDRESS>
```

### 5. Run Front End
```shell
yarn start
```

## Result
Deployed [WChicks Contract at 0x776C6484Df043B2E97432ae8915745542F6ac9B3 on Ropsten(Testnet)](https://ropsten.etherscan.io/address/0x776C6484Df043B2E97432ae8915745542F6ac9B3)

- If the connected account is not owner  
![Image](./screenshots/Screenshot_2022-05-03_003805.jpg)

- If the connected account is owner  
![Image](./screenshots/Screenshot_2022-05-03_003717.jpg)  
![Image](./screenshots/Screenshot_2022-05-03_003657.jpg)