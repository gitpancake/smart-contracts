# Smart Contracts

A clean Hardhat Ignition project for smart contract development.

## Quick Start

```bash
# Install dependencies
npm install

# Compile contracts
npm run compile

# Run tests
npm test

# Deploy to local network
npx hardhat ignition deploy ignition/modules/Lock.ts --network localhost

# Deploy to testnet (sepolia)
npx hardhat ignition deploy ignition/modules/Lock.ts --network sepolia
```

## Scripts

- `npm run compile` - Compile contracts
- `npm run test` - Run tests
- `npm run coverage` - Generate test coverage report
- `npm run gas-report` - Generate gas usage report
- `npm run clean` - Clean build artifacts
- `npm run lint` - Lint TypeScript and Solidity files
- `npm run format` - Format code

## Environment Variables

Copy `.env.example` to `.env` and configure:

- `SEPOLIA_RPC_URL` - RPC URL for Sepolia testnet
- `MAINNET_RPC_URL` - RPC URL for Ethereum mainnet
- `PRIVATE_KEY` - Your wallet private key (without 0x prefix)
- `ETHERSCAN_API_KEY` - For contract verification
- `COINMARKETCAP_API_KEY` - For gas reporting
- `REPORT_GAS` - Set to true to enable gas reporting

## Project Structure

- `contracts/` - Solidity smart contracts
- `ignition/modules/` - Hardhat Ignition deployment modules
- `test/` - Contract tests
- `scripts/` - Utility scripts