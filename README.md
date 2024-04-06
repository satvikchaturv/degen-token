# DegenToken Contract

## Overview
DegenToken is a Solidity smart contract that implements a basic ERC20 token with additional functionalities such as minting, burning, transferring tokens, redeeming jackets, and managing jacket inventory. It serves as a demonstration of token management and inventory tracking on the Ethereum blockchain.

## Features
- **ERC20 Token**: Implements the ERC20 standard for fungible tokens.
- **Minting**: Allows the owner to mint new tokens and distribute them to designated addresses.
- **Burning**: Enables token holders to burn their tokens, reducing the total supply.
- **Transferring**: Facilitates the transfer of tokens between addresses.
- **Jacket Redemption**: Users can redeem jackets using their tokens, with each jacket having a specific price and stock quantity.
- **Jacket Inventory Management**: The contract owner can add or modify the stock of jackets available for redemption.

## Contract Structure
- **ERC20**: Inherits from OpenZeppelin's ERC20 contract to implement the basic token functionalities.
- **Ownable**: Inherits from OpenZeppelin's Ownable contract to provide access control functionalities.
- **ERC20Burnable**: Inherits from OpenZeppelin's ERC20Burnable contract to enable token burning functionalities.

## Functions
- `mintTokens`: Allows the owner to mint new tokens and assign them to a specified address.
- `burnTokens`: Allows token holders to burn a certain amount of their tokens.
- `transferTokens`: Enables token holders to transfer tokens to another address.
- `redeemJacket`: Allows users to redeem jackets using their tokens, deducting the token amount from their balance and updating the jacket inventory.
- `getUserTokenBalance`: Retrieves the token balance of the caller.
- `addJacketStock`: Allows the owner to add stock to a particular type of jacket.
- `modifyJacketStock`: Allows the owner to modify the stock of a particular type of jacket.

## Usage
1. Deploy the contract to the Ethereum blockchain.
2. Mint initial tokens to designated addresses using `mintTokens` function.
3. Users can interact with the contract to burn, transfer, and redeem tokens for jackets.
4. The owner can manage the inventory by adding or modifying the stock of jackets.

## Security Considerations
- Ensure proper access control to critical functions.
- Validate user inputs to prevent potential vulnerabilities.
- Implement proper error handling and revert conditions.

## Disclaimer
This contract is provided as-is for demonstration purposes only. Use it at your own risk and ensure proper auditing and testing before deploying it in a production environment.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
