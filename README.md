# Raffle Project

This project implements a decentralized raffle system using Chainlink VRFv2.5 for verifiable randomness.

## Features

- Enter raffle with ETH
- Automated winner selection using Chainlink VRF and Automation
- Configurable entrance fee and raffle interval
- Fully decentralized and transparent

## Technologies

- Solidity ^0.8.19
- Chainlink VRFv2.5
- Foundry for development and testing

## Setup

1. Clone the repository
2. Install dependencies:
   ```bash
   make install
   ```

## Building

To build the project, run:

```bash
make build
```

## Testing

Run tests with:

```bash
make test
```

To create a gas snapshot:

```bash
make snapshot
```

## Deployment

To deploy the contract:

```bash
make deploy
```

For network-specific deployment (e.g., Sepolia), use:

```bash
make deploy ARGS="--network sepolia"
```

## Chainlink VRF Setup

1. Create a VRF Subscription:
   ```bash
   make createSubscription
   ```

2. Fund the subscription:
   ```bash
   make fundSubscription
   ```

3. Add the contract as a consumer:
   ```bash
   make addConsumer
   ```

## Development Commands

- Format code: `make format`
- Update dependencies: `make update`
- Run local Anvil chain: `make anvil`

## Environment Setup

Create a `.env` file in the root directory with the following variables:

```
SEPOLIA_RPC_URL=your_sepolia_rpc_url
ETHERSCAN_API_KEY=your_etherscan_api_key
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.
