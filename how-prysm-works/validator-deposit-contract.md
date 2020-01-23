---
description: >-
  This section outlines the responsibilities and functions of Prysm's validator
  deposit contract.
---

# Validator Deposit Contract

## This documentation portal is depreciated and no longer maintained. Please visit [docs.prylabs.network](https://docs.prylabs.network) for the most recent iteration.

The **validator deposit contract** is a core component of the Prysm client, and is responsible for handling both the input and verification of the initial 32 ETH deposit required to initialise a node and fully participate in the Ethereum 2.0 network.

A [validator](validator-clients.md) is queued in the full [Proof-of-Stake](../glossaries/terminology.md#proof-of-stake-pos) system once a 32 ETH deposit is made from the existing Ethereum blockchain into a **validator deposit contract** and the node has fully spun up. By ensuring that all initial deposits come from the [ETH1](../glossaries/terminology.md#eth1) chain, Ethereum 2.0 is able to leverage the security pool and value of existing Ether to secure the network upon launch. Prysm nodes automatically listen for deposit logs from this contract on the [ETH1](../glossaries/terminology.md#eth1) chain and detect when a validator is ready for activation.

For more information and current developments, see the official [Ethereum 2.0 deposit contract specification](https://github.com/ethereum/eth2.0-specs/blob/dev/specs/core/0_deposit-contract.md).

