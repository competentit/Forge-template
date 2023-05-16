 # Foundry Template:rocket:

[![Github Actions][gha-badge]][gha] [![Forge][Forge-badge]][Forge]

[gha]: https://github.com/competentit/Forge-template/actions
[gha-badge]: https://github.com/competentit/Forge-template/actions/workflows/CI.yml/badge.svg

[Forge]: https://github.com/foundry-rs/foundry
[Forge-badge]: https://img.shields.io/badge/build%2Ftest%2Fdeploy%20with-Forge-blue

---

A Forge-based template for developing Solidity smart contracts, with sensible defaults.

- [Forge](https://github.com/foundry-rs/foundry/tree/master/forge): compile, run and test smart contracts
- [Ethers](https://github.com/ethers-io/ethers.js/): renowned Ethereum library and wallet implementation
- [Solhint](https://github.com/protofire/solhint): code linter
- [Solcover](https://github.com/sc-forks/solidity-coverage): code coverage
- [Prettier Plugin Solidity](https://github.com/prettier-solidity/prettier-plugin-solidity): code formatter

## Getting Started

```
mkdir my-project
cd my-project
forge init --template https://github.com/competentit/Forge-template
git submodule update --init --recursive  // Initialize submodule dependencies
yarn install // Install development dependencies
yarn build
yarn test
yarn lint
```

## Features

### Testing Utilities

Includes a `Greeter.sol` contract with common testing methods (like creating users with an initial balance), as well as various other utility contracts.

### Preinstalled dependencies

`ds-test` for testing, `forge-std` for better cheatcode UX, and `solmate` for optimized contract implementations.

### Linting

Pre-configured `solhint` and `prettier-plugin-solidity`. Can be run by

```
yarn solhint
yarn prettier
```
