# Hardhat tutorial

## Disclaimer
This is just a project based on the [Hardhat tutorial](https://hardhat.org/tutorial).

### Setting up the project
To setup the project you only need to get your ethereum private key from your wallet (I've used [Metamask](https://metamask.io/)) and an [Alchemy API key](https://www.alchemy.com/). You can then put them in the ```.env``` file

#### .env file
```
PRIVATE_KEY="Your private key"
ALCHEMY_API_KEY="Your alchemy api key"
```

## Commands

### Test

```bash
npx hardhat test
```

##### Expected output

```
    Deployment
      ✔ Should set the right owner
      ✔ Should assign the total supply of tokens to the owner
    Transactions
      ✔ Should transfer tokens between accounts (98ms)
      ✔ Should fail if sender doesn’t have enough tokens (114ms)
      ✔ Should update balances after transfers (94ms)


  5 passing (3s)
```

### Deploy

```bash
npx hardhat run scripts/deploy.js --network rinkeby
```

#### Expected output

```
Deploying contracts with the account: 0xA853Ad7156aaC80A5Ff6F8dcC32146d18f01E441
Account balance: 291748494394015405
Token address: 0xda1C99b29aDFdCdC57F5d4a47c8084a2A7eA0b5e
```

### About the project
It is a simple project where a token is created with a contract. The project includes tests and functions to transfer tokens and getting and address balance
