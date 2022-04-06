# Web Extension Integration

## Introduction

Crypto.com | Wallet Extension - A non-custodial wallet to store, earn, and grow your crypto

Crypto.com | Wallet Extension provides a simple and secure way for users to connect their Crypto.com DeFi Wallet with Ethereum-compatible DApps via their browser.

- **For DApp builders**, integrating with Wallet Extension allows them to offer a streamlined user experience to the millions of Crypto.com DeFi Wallet users, as well as encourage increased adoption and usage.

- **For users**, this means that they can connect to DApps simply by clicking the Wallet Extension logo, scanning the QR code with their DeFi Wallet, and approving the connection. The user experience is familiar for those who are already using Wallet Connect with the DeFi Wallet, yet it feels more native and simple. Over time, additional user-friendly features will be built into Wallet Extension.

Crypto.com DeFi Wallet is a non-custodial wallet that gives users full control of their crypto and private keys. Through Wallet Extension, it offers smooth navigation with DApps. Private keys are encrypted locally on the user’s mobile phone, and protected by Biometric Authentication and 2-Factor Authentication. For transactions made on desktop, users must confirm the transaction via the DeFi Wallet mobile app.

The Crypto.com Wallet Extension currently supports the following networks:

**Mainnet**:

- Cronos Mainnet Beta;
- Ethereum Mainnet;
- Crypto.org Chain.

**Testnet**:

- Cronos Testnet;
- Croeseid Testnet;
- Ethereum Testnet (Ropsten, Kovan, Ribkeby, Goerli);

Integrations with additional chains are planned for the near future.

## Integrating with Defi Connect

Integrate your DApp with Defi Connect to provide a seamless and native experience for your end users to sign transactions.

### Install

#### Via yarn
```bash
yarn add "deficonnect"
```

#### Via npm
```bash
npm install "deficonnect"
```

### Usage
:::tip Note
` DeFiWeb3Connector`  has implement ` AbstractConnector`  from ` web3-react` 
:::

#### For `web3-react` 
if you use web3-react, it is easy to integrate:
```tsx
import { DeFiWeb3Connector } from 'deficonnect'

const connector = new DeFiWeb3Connector({
  supportedChainIds: [1],
  rpc: { 1: 'https://mainnet.infura.io/v3/INFURA_API_KEY' },
  pollingInterval: 15000,
})
connector.activate()
```

#### Normally
```tsx
import { DeFiWeb3Connector } from "deficonnect";
import Web3 from "web3";

const connector = new DeFiWeb3Connector({
  supportedChainIds: [1],
  rpc: {
    1: "https://mainnet.infura.io/v3/INFURA_API_KEY",
    25: "https://evm.cronos.org/", // cronos mainet
  },
  pollingInterval: 15000,
});
connector.activate();
const provider = await connector.getProvider();
const web3 = new Web3(provider);
```
## Example Apps
The following git folder will provide you with some basic deficonnect integrations via react and web3modal. 
:::tip Note
You need to replace `INFURA_API_KEY` with a key generated at [Infura](https://infura.io/) 
:::

### Git clone `deficonnect-examples`
  ```bash
  $ git clone git@github.com:crypto-org-chain/dev-utils.git
  ```

## DApp Listing Form

Complete the form below to be featured on our DeFi Wallet DApp listing:

[DApp Listing Form](https://crypto-com.typeform.com/to/bRvudlYV)
