# ERC20 and Vault Contracts

## Overview
This repository contains Solidity smart contracts for an ERC20 token and a Vault contract. The ERC20 token contract implements the ERC20 standard interface for fungible tokens on the Ethereum blockchain. The Vault contract provides a secure storage mechanism for the ERC20 tokens.

## Contracts

### ERC20 Token Contract
- **Name:** ERC20Token.sol
- **Purpose:** This contract implements the ERC20 standard interface for a fungible token. It allows users to transfer tokens between addresses, approve others to spend tokens on their behalf, and retrieve the token balance of any address.

### Vault Contract
- **Name:** Vault.sol
- **Purpose:** The Vault contract serves as a secure storage facility for the ERC20 tokens. It provides functionalities to deposit and withdraw tokens securely. Only authorized users can access the tokens stored in the vault.

## Deployment

### ERC20 Token Deployment
To deploy the ERC20 token contract:
1. Compile the ERC20Token.sol contract.
2. Deploy the compiled contract to an Ethereum network of your choice (e.g., Ropsten, Rinkeby, Mainnet).

### Vault Deployment
To deploy the Vault contract:
1. Compile the Vault.sol contract.
2. Deploy the compiled contract to an Ethereum network.
3. Provide necessary parameters such as the ERC20 token address to link the vault with the token.

## Usage

### ERC20 Token
Once deployed, the ERC20 token contract provides the following functionalities:
- `transfer(address _to, uint256 _amount)`: Transfer tokens to a specified address.
- `approve(address _spender, uint256 _amount)`: Approve a spender to transfer tokens on behalf of the owner.
- `transferFrom(address _from, address _to, uint256 _amount)`: Transfer tokens on behalf of a designated owner.
- `balanceOf(address _owner)`: Get the token balance of a specified address.

### Vault
Once deployed, the Vault contract offers the following functionalities:
- `deposit(uint256 _amount)`: Deposit ERC20 tokens into the vault.
- `withdraw(uint256 _amount)`: Withdraw ERC20 tokens from the vault.
- `getBalance()`: Get the balance of ERC20 tokens stored in the vault.

## License
This project is licensed under the [MIT License](LICENSE).

