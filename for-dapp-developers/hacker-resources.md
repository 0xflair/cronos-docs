---
description: Quick-start resource if you are hacking and need to integrate with Cronos.
---

# 🏅 Hacker's getting started resources

## Overview of Cronos chain

[Cronos](https://cronos.org/) ([cronos.org](http://cronos.org)) is the leading Ethereum-compatible layer 1 blockchain network built on the Cosmos SDK, supported by [Crypto.com](http://crypto.com), [Crypto.org](http://crypto.org) and more than 500 app developers and partners. Today, the #CROfam ecosystem represents an addressable user base of more than 80 million people worldwide. Our mission is to make it easy and safe for the next billion crypto users to adopt Web3, with a focus on DeFi and GameFi.

[Broken link](broken-reference "mention")

## How to stand out and win in a Web3 hackathon 🥇

Check out our [blog post](https://blog.cronos.org/p/cronos-developer-series-5-tips-to-stand-out-in-a-web3-hackathon-924d774f1617).

## Hack with Cronos 🥚

Developing Dapps on Cronos is as easy as developing them on any of the major EVM-compatible chains: write and test solidity with Hardhat, deploy your contract, connect your frontend or your backend with ethers.js, and connect your wallet with MetaMask or Crypto.com Defi Wallet.

The native cryptocurrency of Cronos mainnet is CRO, while the testnet uses TCRO.

**Cronos overview & key links for developers**

* Cronos docs: [https://docs.cronos.org](https://docs.cronos.org)
* Cronos Play (for game developers): [https://cronos.org/play](https://cronos.org/play)
* [Why build on Cronos](https://cronoslabs.substack.com/p/why-build-grow-on-cronos-692da1de7885)
* Cronos overview by Eat The Blocks: [https://www.youtube.com/watch?v=NqeeKEJiPZU](https://www.youtube.com/watch?v=NqeeKEJiPZU)

**MetaMask end-user configuration**

* The [cronos.org](http://cronos.org) website has a little orange button at the top of the page, that you can click to add Cronos mainnet to your MetaMask wallet.
* For more details, see [Metamask configuration](../for-users/metamask.md)

**JSON-RPC endpoint configuration**

*   For most use cases you can use the free endpoints that are provided by Cronos Labs. Most developers use a configuration file that looks like this:

    For Hardhat:

    ```json
    {
    "cronos_mainnet": {
          "chainId": 25,
          "url": "https://evm.cronos.org/",
          "gasPrice": 5000000000000,
          "blockExplorer": "https://cronoscan.com/",
          "blockExplorerPrefix": "https://cronoscan.com/tx/"
        },
    "cronos_testnet": {
          "chainId": 338,
          "url": "https://evm-t3.cronos.org/",
          "gasPrice": 5000000000000,
          "blockExplorer": "https://cronos.org/explorer/testnet3/",
          "blockExplorerPrefix": "https://cronos.org/explorer/testnet3/tx/"
        },
    }
    ```

    or, using EIP1559 in a Node.js backend:

    ```json
    {
    "cronos_mainnet": {
          "id": 25,
          "url": "https://evm.cronos.org/",
          "maxPriorityFeePerGas": 5000000000,
          "maxFeePerGas": 6000000000000,
          "blockExplorer": "https://cronoscan.com/",
          "blockExplorerPrefix": "https://cronoscan.com/tx/"
        },
    "cronos_testnet": {
          "id": 338,
          "url": "https://evm-t3.cronos.org/",
          "maxPriorityFeePerGas": 5000000000,
          "maxFeePerGas": 6000000000000,
          "blockExplorer": "https://cronos.org/explorer/testnet3/",
          "blockExplorerPrefix": "https://cronos.org/explorer/testnet3/tx/"
        },
    }
    ```
*   Testnet CRO faucet

    [https://cronos.org/faucet](https://cronos.org/faucet)

## Tutorials 🚀

**Blog posts**

* [Deploy and verify your smart contracts](https://cronoslabs.substack.com/p/cronos-developer-series-deploy-verify-your-contracts-using-hardhat-8b6ab6928986)
* [Create & deploy a smart contract with OpenZeppelin Wizard and Remix (low code)](https://cronoslabs.substack.com/p/cronos-developer-series-create-deploy-a-smart-contract-with-openzeppelin-wizard-and-remix-5b6769fc8b93)
* [Connect your Dapp to wallets](https://cronoslabs.substack.com/p/cronos-developer-series-connect-your-dapp-with-defi-wallet-metamask-and-trust-wallet-77419fe696a5)
* [Build a simple Dapp](https://cronoslabs.substack.com/p/cronos-developer-series-build-a-simple-dapp-with-react-crypto-com-defi-wallet-and-metamask-87c37ccd589f)
* [Create a NFT collection on Cronos and IPFS](https://cronoslabs.substack.com/p/cronos-developer-series-build-a-simple-dapp-with-react-crypto-com-defi-wallet-and-metamask-87c37ccd589f)

**Video tutorials**

<table><thead><tr><th width="120">Popular</th><th width="181">Title</th><th width="254">URL</th><th width="141">Date</th></tr></thead><tbody><tr><td></td><td>Creating dapps on Cronos chain</td><td><a href="https://www.youtube.com/watch?v=XUNbR91abwY">https://www.youtube.com/watch?v=XUNbR91abwY</a></td><td>June 10, 2022</td></tr><tr><td>⭐️</td><td>Creating games with Cronos Play</td><td><a href="https://www.youtube.com/watch?v=D52Ike59cL8&#x26;t=5s">https://www.youtube.com/watch?v=D52Ike59cL8&#x26;t=5s</a></td><td>June 10, 2022</td></tr><tr><td></td><td>Cronos Play tutorial</td><td><a href="https://youtu.be/xLSgn5OZql4">https://youtu.be/xLSgn5OZql4</a></td><td>August 23, 2022</td></tr><tr><td></td><td>RockX walk through</td><td><a href="https://www.youtube.com/watch?v=gvY2vyYSZHs">https://www.youtube.com/watch?v=gvY2vyYSZHs</a></td><td>August 24, 2022</td></tr><tr><td></td><td>Covalent walk through</td><td><a href="https://www.youtube.com/watch?v=f7ZHDByytFc&#x26;t">https://www.youtube.com/watch?v=f7ZHDByytFc&#x26;t</a></td><td>August 25, 2022</td></tr><tr><td></td><td>How to win a hackathon</td><td><a href="https://www.youtube.com/watch?v=kyMg0jtuT-8&#x26;t=29s">https://www.youtube.com/watch?v=kyMg0jtuT-8&#x26;t=29s</a></td><td>August 29, 2022</td></tr><tr><td></td><td>Building games with Moralis</td><td><a href="https://www.youtube.com/watch?v=EbO03yoorps">https://www.youtube.com/watch?v=EbO03yoorps</a></td><td>August 30, 2022</td></tr><tr><td></td><td>Moralis walk through</td><td><a href="https://www.youtube.com/watch?v=9F0dweAtm_U">https://www.youtube.com/watch?v=9F0dweAtm_U</a></td><td>September 1, 2022</td></tr><tr><td></td><td>Wallet game design choices</td><td><a href="https://www.youtube.com/watch?v=KdGfDyxmTNU">https://www.youtube.com/watch?v=KdGfDyxmTNU</a></td><td>September 5, 2022</td></tr><tr><td></td><td>Build your Web3 Game with Cronos Play</td><td><a href="https://www.youtube.com/watch?v=lmM7HgXDZ2w">https://www.youtube.com/watch?v=lmM7HgXDZ2w</a></td><td>September 9, 2022</td></tr><tr><td>⭐️</td><td>Create dApps on Cronos chain</td><td><a href="https://www.youtube.com/watch?v=lKzzyUXPeRk">https://www.youtube.com/watch?v=lKzzyUXPeRk</a></td><td>December 1, 2022</td></tr></tbody></table>

## Essential developer tools 💻

Write, test and deploy smart contracts

* Smart contracts library: [OpenZeppelin](https://www.openzeppelin.com/)
* Compile & test: [Hardhat](https://hardhat.org/)

Connect your Dapp to the blockchain

* Web3 library for Javascript / Typescript: [ethers.js](https://docs.ethers.io/v5/), [web3.js](https://web3js.readthedocs.io/)
* Web3 library for Python: [web3.py](https://web3py.readthedocs.io/)
* Easy to use Web3 SDK: [Moralis](https://moralis.io/)

Create games

* Cronos Play overview: [Cronos Play](https://cronos.org/docs/play/cronos-gamefi-integraton.html)
* Javascript SDK: [Moralis](https://moralis.io/)
* Unity plugin: [docs](https://cronos.org/docs/play/getting-started.html) and [repo](https://github.com/ChainSafe/web3.unity)
* Unreal plugin: [docs](https://cronos.org/docs/play/getting-started\_unreal.html#pre-requisites), [repo](https://github.com/cronos-labs/play-unreal-plugin) and [demo](https://github.com/cronos-labs/play-unreal-demo)
* C++ SDK: [docs](https://cronos.org/docs/play/getting-started\_cpp.html#pre-requisites) and [repo](https://github.com/cronos-labs/play-cpp-sdk)
* [Full list of available dev tools and integration](useful-projects-on-cronos/overview-of-dev-tools-and-integrations.md)

## Developer support ☎️

Please visit the #cronos-mainnet-beta channel on the Cronos [Discord](https://discord.com/invite/pahqHz26q4) server.

Feedback is a gift! [Let us know](mailto:contact@cronoslabs.org) if there is anything that we can improve in this documentation.

Socials: [Twitter](https://twitter.com/cronos\_chain) | [Telegram](https://t.me/Cryptoorg\_Chain\_Announcements) | [Discord](https://discord.com/invite/pahqHz26q4) | [Youtube](https://www.youtube.com/channel/UCUvlFgAWURU\_wECYp2GpJtw/featured)

