# Geth with Sepolia Testnet

Interact with Ethereum smart contracts, deploy your own, or test applications on the Sepolia testnet using your local Geth node.

## Prerequisites

Before you start, make sure that [Geth](https://geth.ethereum.org/docs/getting-started/installing-geth) is installed. After installation, verify it is working by running:

```bash
geth version
```

## Quickstart

Run `geth --sepolia` to connect your client to the Sepolia blockchain and begin syncing with peers or `geth --sepolia --http --http.api eth,net,web3` to interact with your node via RPC.

- `--http` enables HTTP-RPC access.
- `--http.api eth,net,web3` enables the HTTP-RPC interface and specifies which APIs are available over it.

### Accounts

Create, import, or list accounts:

```bash
# Create a new account
geth account new --datadir ./data

# Import an existing account
geth account import <path-to-keyfile> --datadir ./data

# List existing accounts
geth account list --datadir ./data
```

### Interacting with the network

To deploy contracts or send transactions, you need Ethereum testnet tokens from a Sepolia faucet.

From the console, you can interact with Ethereum using web3 commands, check balances, deploy contracts, and more.

For more information, see:

- [Interacting with Geth](https://geth.ethereum.org/docs/interacting-with-geth)
- [Ethereum JSON-RPC API](https://ethereum.org/developers/docs/apis/json-rpc)

You can also use frameworks like Hardhat or Truffle with your Geth node to automate contract deployment.
