---
title: Introduction
---

# About Conflux eSpace

Conflux has a virtual machine that is similar to the EVM. However, there are still some considerable differences between Conflux and Ethereum. Conflux uses a different transaction format and a different rule for generating addresses from public keys. These differences often make it hard to port EVM compatible dApps to Conflux. Replacing CIP-72 and CIP-80, [CIP-90](https://github.com/Conflux-Chain/CIPs/blob/master/CIPs/cip-90.md) introduces a transaction execution environment called the Conflux eSpace. eSpace achieves full EVM compatibility without changing the existing accounts and transactions.

[CIP-90](https://github.com/Conflux-Chain/CIPs/blob/master/CIPs/cip-90.md) introduces a new fully EVM-compatible space. The new space is called Conflux eSpace, while the current space is called Conflux Core space. Conflux eSpace follows the same rule as Ethereum's EVM and supports RPCs like `eth_getBalance`. As a result, existing tooling from the Ethereum ecosystem (MetaMask, Truffle, Remix, Hardhat, web3.js, ethers.js) can be used on Conflux eSpace directly.

# Integrate with the Fluent wallet

Integrate your dapp with the Fluent wallet using the
[Fluent Ethereum provider API](reference/provider-api.md), which enables your dapp to interact
with its users' Conflux eSpace accounts.
We recommend using [@fluent-wallet/detect-provider](https://www.npmjs.com/package/@fluent-wallet/detect-provider) to easily enable your users to connect to their
Fluent wallet client from any platform.

Get started by [setting up your development environment](get-started/set-up-dev-environment.md).

:::note
- This documentation assumes intermediate knowledge of JavaScript, HTML, and CSS.
:::

## What is the Fluent Ethereum provider API?

The [Fluent Ethereum provider API](reference/provider-api.md) is a JavaScript API that Fluent
injects into websites visited by Fluent users.
Your dapp can use this API to request users' Conflux eSpace accounts, read data from blockchains the user
is connected to, and suggest that the user sign messages and transactions.

## Questions?

If you have questions about integrating your dapp with Fluent Wallet, you can interact with the Fluent
team and community on the Fluent Wallet issues on [Fluent Issues](https://github.com/Conflux-Chain/helios/issues) or [Zendesk](https://fluent-wallet.zendesk.com/hc/en-001/requests/new).
