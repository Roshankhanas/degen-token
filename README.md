# Blanket Subscription Smart Contract

Welcome to the Blanket Subscription smart contract repository! This repository contains a Solidity smart contract named `BlanketSubscription` designed to manage a subscription-based system for redeeming blankets using a custom ERC20 token.

## Overview

The `BlanketSubscription` contract allows users to redeem different types of blankets using the custom ERC20 token (`Blanket Token` or `BLK`). Users can redeem blankets of various types, including Cotton, Wool, Fleece, Silk, and Cashmere, by spending a specific amount of tokens. Additionally, users are rewarded with tokens when they redeem blankets.

## Contract Details

### BlanketSubscription.sol

The `BlanketSubscription` contract inherits functionalities from the OpenZeppelin ERC20 implementation and the Ownable contract. It includes the following features:

- **Subscription Rewards:** Users are rewarded with tokens when they redeem blankets. The reward amount is half of the cost of the redeemed blanket.
- **Blanket Redemption:** Users can redeem blankets of different types by spending a specific amount of tokens.
- **Token Minting and Burning:** The contract owner can mint and burn tokens, providing flexibility in managing token supply.

## Contract Functions

- **`mintTokens(address to, uint256 total)`:** Allows the contract owner to mint tokens and allocate them to a specific address.
- **`burnTokens(address from, uint256 total)`:** Allows the contract owner to burn tokens from a specific address.
- **`transferTokens(address from, address to, uint256 total)`:** Allows the contract owner to transfer tokens between addresses.
- **`redeemBlanket(uint8 blanketNumber)`:** Allows users to redeem blankets by spending tokens. Users can choose from five types of blankets, and the cost varies depending on the blanket type.

## Usage

To utilize the `BlanketSubscription` contract:

1. **Deploy Contract:** Deploy the `BlanketSubscription` contract to the Ethereum blockchain.
2. **Token Management:** Mint an initial supply of `Blanket Token` using the `mintTokens` function and distribute tokens as needed.
3. **Subscription Process:** Users can interact with the contract to redeem blankets of their choice using the `redeemBlanket` function.
4. **Reward Claim:** Users automatically receive rewards in the form of tokens when they redeem blankets.

## License

This code is licensed under the MIT License. Refer to the `LICENSE` file within the repository for detailed information regarding the usage and distribution of this codebase.

