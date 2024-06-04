## Quickstart

```
yarn
yarn hardhat
```

# Usage

Deploy:

```
yarn hardhat run scripts/deploy.js
```

## Testing

```
yarn hardhat test
```

### Test Coverage

```
yarn hardhat coverage
```

## Estimate gas

You can estimate how much gas things cost by running:

```
yarn hardhat test
```

And you'll see and output file called `gas-report.txt`

## Local Deployment 

If you'd like to run your own local hardhat network, you can run:

```
yarn hardhat node
```

And then **in a different terminal**

```
yarn hardhat run scripts/deploy.js --network localhost
```

And you should see transactions happen in your terminal that is running `yarn hardhat node`

## Deployment to a testnet or mainnet

1. Setup environment variables

You'll want to set your `SEPOLIA_RPC_URL` and `PRIVATE_KEY` as environment variables. You can add them to a `.env` file

2. Get testnet ETH

Head over to [faucets.chain.link](https://faucets.chain.link/) and get some tesnet ETH. You should see the ETH show up in your metamask.

3. Deploy

```
yarn hardhat run scripts/deploy.js --network sepolia
```