---
title: Glossary
---

# SecureRPC

# **Introduction to SecureRPC**

SecureRPC is a Remote Procedure Call (RPC) endpoint that protects users from predatory MEV like front-running and sandwich attacks, as well as against failed and reverted transactions. SecureRPC privately routes transactions to trusted block builders and validators, bypassing the public mempool. Users can [add SecureRPC to their DeFi wallet](https://www.notion.so/How-to-add-SecureRPC-to-MetaMask-db10a330d9ce4c95a3ebda11cc9f391f?pvs=21) to protect their transactions.

## **What is a Web3 RPC?**

SecureRPC is a trusted Web3 RPC, which is a specific type of Remote Procedure Call (RPC) endpoint that is used to interact with a blockchain network, specifically those that use the Ethereum protocol and the Web3 library. It allows a client to send requests to a blockchain node (such as a Geth or parity node) over HTTP or IPC, and receive responses in JSON format.

Web3 RPC provides a number of methods for interacting with the blockchain, such as querying the state of accounts, sending transactions, and interacting with smart contracts.

Web3 RPC is commonly used by DApps (Decentralized Applications) to interact with the Ethereum blockchain, it allows them to read data from the blockchain and also write to the blockchain via transactions.

## **What is the public mempool?**

The mempool, short for “memory pool,” is a holding area for transactions that have been broadcast to the network but have not yet been included in a block. When a user initiates a transaction, it is broadcast to the network and picked up by nodes. These nodes will validate the transaction and then add it to their own mempool.

The public mempool refers to the mempool as seen by all the nodes in the network, which contain all the transactions that have been broadcast to the network but not yet included on chain. Validators/block builders use the transactions in the mempool to select which transactions they want to include in the next block. The transactions that are not included in a block will stay in the mempool until they get included or dropped due to the size limitation.

In a public mempool, the transactions are usually prioritized based on the fee attached to them, with the highest fee transactions being prioritized over the lower fee transactions. This is because validators and block builders typically choose to include transactions with higher fees in order to maximize their rewards.

## **MEV Searchers**

MEV searchers can also use SecureRPC for bundle / transaction submission. The endpoint above supports the following MEV methods:

- `eth_sendRawTransaction`
- `manifold_sendBundle`
- `eth_sendBundle`
- `manifold_sendMegabundle`
- `eth_sendMegabundle`
- `manifold_sendPrivateRawTransaction`
- `eth_sendPrivateRawTransaction`
