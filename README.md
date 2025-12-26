# Foundry Fund Me

This repository is part of my Solidity + Foundry learning journey,
inspired by the Cyfrin / Patrick Collins course.

## About

A minimal smart contract that allows users to fund the contract owner
with ETH. The ETH amount is converted to USD using a Chainlink price
feed, and a minimum USD threshold is enforced.

## Tech Stack

-   Solidity
-   Foundry (forge / anvil / cast)
-   Chainlink Price Feeds

## Project Structure

-   `src/` -- smart contracts
-   `test/` -- tests
-   `script/` -- deployment & interaction scripts
-   `Makefile` -- common commands

## Getting Started

### Build

``` bash
forge build
```

### Test

``` bash
forge test
```

### Local Chain

``` bash
make anvil
```

## Deploy (Sepolia)

Create a `.env` file with:

-   SEPOLIA_RPC_URL
-   PRIVATE_KEY
-   ETHERSCAN_API_KEY (optional)

``` bash
make deploy-sepolia
```

## Notes

-   Do not commit `.env`
-   Educational use only

## Credits

Inspired by the Cyfrin Foundry Fund Me course by Patrick Collins.