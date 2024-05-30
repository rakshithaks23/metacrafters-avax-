# ERC20 and Vault README

## Overview

This repository contains two main components:
1. **ERC20 Token**: A standard implementation of an ERC20 token contract.
2. **Vault**: A smart contract for managing ERC20 tokens, including deposit, withdrawal, and other token management functionalities.

## ERC20 Token

The ERC20 token contract adheres to the ERC20 standard, providing basic functionalities such as transferring tokens, approving tokens for spending, and querying balances. 

### Features

- **Minting**: The ability to create new tokens.
- **Burning**: The ability to destroy tokens.
- **Transfer**: Allows the transfer of tokens between addresses.
- **Allowance**: Enables a user to allow another user to transfer tokens on their behalf.
- **Balance Query**: Check the token balance of an address.

### Functions

- `totalSupply()`: Returns the total supply of the token.
- `balanceOf(address account)`: Returns the token balance of the specified address.
- `transfer(address recipient, uint256 amount)`: Transfers `amount` tokens to the `recipient` address.
- `approve(address spender, uint256 amount)`: Approves the `spender` to spend `amount` tokens on behalf of the caller.
- `transferFrom(address sender, address recipient, uint256 amount)`: Transfers `amount` tokens from `sender` to `recipient` using the allowance mechanism.
- `allowance(address owner, address spender)`: Returns the remaining number of tokens that `spender` is allowed to spend on behalf of `owner`.

## Vault

The Vault contract provides a secure way to manage ERC20 tokens, including functionalities for deposits, withdrawals, and checking balances.

### Features

- **Deposit**: Users can deposit ERC20 tokens into the vault.
- **Withdrawal**: Users can withdraw their tokens from the vault.
- **Balance Tracking**: The vault keeps track of each user's deposited balance.

### Functions

- `deposit(uint256 amount)`: Allows a user to deposit `amount` tokens into the vault.
- `withdraw(uint256 amount)`: Allows a user to withdraw `amount` tokens from the vault.
- `balanceOf(address account)`: Returns the balance of tokens deposited by the `account`.
