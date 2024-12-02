## Features

- **ERC-20 Token Contract**: Implements a Solidity smart contract that adheres to the ERC-20 token standard, featuring fundamental token management capabilities.
- **Standards Compliance**: Ensures full compliance with the ERC-20 specification, including required functions and events.
- **Code Quality**: Follows best practices for secure and efficient smart contract development.

## Getting Started

1. Clone the repository.
2. Open the project in your preferred development environment.
3. Compile the smart contracts using tools like Remix or Foundry.
4. Deploy the contracts to an Ethereum testnet of your choice (e.g., Sepolia, Goerli).
5. Interact with the deployed contracts via a suitable frontend or directly using Web3.js.

## ERC-20 Contract Overview

This repository includes a smart contract implementing the ERC-20 token standard. Below are the contract's key functionalities:

### Features

- **Data Structure**:
  - `Token Name`: The name of the token.
  - `Token Symbol`: The token's ticker symbol.
  - `Total Supply`: The maximum supply of tokens initialized during deployment.

- **Core Functions**:
  - `balanceOf(address account)`: Returns the token balance of the specified address.
  - `transfer(address recipient, uint256 amount)`: Transfers a specified number of tokens to the recipient's address.
  - `approve(address spender, uint256 amount)`: Allows a spender to withdraw a specified number of tokens.
  - `transferFrom(address sender, address recipient, uint256 amount)`: Executes a transfer on behalf of the sender, given a valid allowance.
  - `allowance(address owner, address spender)`: Returns the remaining number of tokens that the spender is permitted to withdraw from the owner.

- **Events**:
  - `Transfer(address indexed from, address indexed to, uint256 value)`: Emitted on successful token transfers.
  - `Approval(address indexed owner, address indexed spender, uint256 value)`: Emitted when a withdrawal allowance is set.

- **Initialization**:
  - The contract initializes with the entire supply allocated to the creator's address upon deployment.

- **Security**:
  - Includes mechanisms to prevent overflows, underflows, and invalid operations (e.g., insufficient balance or unauthorized transfer attempts).

- **Testing**:
  - The contract has been thoroughly tested in an Ethereum development environment to ensure reliability and correctness.

## Contributions

Contributions to this project are welcome. Feel free to open issues or submit pull requests.

## License

This project is licensed under the [MIT License](LICENSE).
