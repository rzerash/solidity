# solidity   
# SuperModel Token Contract

This repository contains an Ethereum smart contract written in Solidity for the "SuperModel Token (SMT)". The contract includes functionalities to mint and burn tokens.

## Overview

The SuperModelToken contract allows the creation (minting) and destruction (burning) of tokens. It includes:
- A public variable for the token name (name), symbol (symbol), and total supply (totalSupply).
- A mapping of addresses to their respective token balances (balances).
- Functions to mint and burn tokens affecting the total supply and the balance of the address involved.

## Contract Functions

- mint(address addr, uint amount): Mints amount of tokens to address addr, increasing the total supply.
- burn(address addr, uint amount): Burns amount of tokens from address addr, decreasing the total supply. Requires that addr has a sufficient balance.

## How to Deploy

1. Use an Ethereum development environment like Remix IDE.
2. Load the contract code into the environment.
3. Compile the contract using the Solidity compiler.
4. Deploy the contract to an Ethereum network (testnet or mainnet).

## How to Interact

After deploying:
- Call mint with an address and amount to mint tokens.
- Call burn with an address and amount to burn tokens, ensuring the address has enough balance.

## Requirements

Ensure you have:
- An Ethereum wallet with some ETH for deployment and transactions.
- A connection to an Ethereum network (via MetaMask or similar).

## Example Usage

```solidity
// Minting 1000 SMT tokens to address 0x...
contract.mint("0x...", 1000);

// Burning 500 SMT tokens from address 0x...
contract.burn("0x...", 500);
