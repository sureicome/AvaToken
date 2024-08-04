# DegenToken Smart Contract Documentation

## Table of Contents

- [Introduction](#introduction)
- [Dependencies](#dependencies)
- [Contract Overview](#contract-overview)
- [Constructor](#constructor)
- [Structures](#structures)
- [Mappings](#mappings)
- [Functions](#functions)
- [Events](#events)
- [Security Considerations](#security-considerations)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

The `DegenToken` smart contract is a unique implementation of an ERC-20 token with added functionalities such as burning tokens, minting tokens, and offering a redemption system for token holders. This contract integrates with OpenZeppelin's libraries to leverage secure and tested components, ensuring robustness and reliability.

## Dependencies

This contract relies on OpenZeppelin's contracts library for the core ERC-20 token logic, ownership management, and burnable token extensions.

- OpenZeppelin Contracts: `@openzeppelin/contracts`
  
  Ensure you have the latest version of OpenZeppelin Contracts installed in your project.

## Contract Overview

`DegenToken` inherits from `ERC20`, `Ownable`, and `ERC20Burnable`. It introduces a novel way for token holders to redeem virtual goods by burning a portion of their token balance.

## Constructor

The constructor initializes the token name as "Degen" and symbol as "DGN". It sets the contract deployer as the owner and mints an initial supply of tokens.


## Structures

The contract uses a `struct` named `RedeemedItem` to track the items redeemed by token holders along with the timestamp of redemption.


## Mappings

A mapping tracks the redeemed items for each user, storing an array of `RedeemedItem` structs.


## Functions

- **mint**: Allows the contract owner to mint new tokens.
- **decimals**: Overrides the base ERC20 contract to return 0, indicating indivisibility.
- **getBalance**: Returns the balance of the caller.
- **transferTokens**: Transfers a specified amount of tokens to a receiver.
- **burnTokens**: Burns a specified amount of tokens from the caller's balance.
- **showStoreItems**: Lists available items for redemption.
- **redeemTokens**: Allows token holders to redeem items by burning tokens.
- **getRedeemedItem**: Retrieves a specific redeemed item by index.
- **getRedeemedItemsCount**: Returns the count of redeemed items for the caller.

## Events

The contract emits events for token transfers and approvals, inherited from the ERC20 standard.

## Security Considerations

- **Burning Mechanism**: Carefully manage the burn mechanism to avoid unintended loss of tokens.
- **Ownership Management**: Securely manage ownership and permissions to prevent unauthorized actions.
- **Gas Optimization**: Consider gas costs for users, especially for frequent interactions like redemption.

## Troubleshooting

- **Compilation Issues**: Ensure compatibility with the Solidity version and OpenZeppelin Contracts version.
- **Deployment Failures**: Verify network configuration and deployment scripts.

## Contributing

Contributions to improve the contract's functionality, security, or documentation are welcome. Please submit pull requests or issues through the GitHub repository associated with this project.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contact

For inquiries or collaboration opportunities, please contact the author through the GitHub profile linked below.

[GitHub Profile](https://github.com/yourusername)


# Project Title

Simple overview of use/purpose.

## Description

An in-depth paragraph about your project and overview of use.

## Getting Started

### Installing

* How/where to download your program
* Any modifications needed to be made to files/folders

### Executing program

* How to run the program
* Step-by-step bullets
```
code blocks for commands
```

## Help

Any advise for common problems or issues.
```
command to run if program contains helper info
```

## Authors

Contributors names and contact info

ex. Dominique Pizzie  
ex. [@DomPizzie](https://twitter.com/dompizzie)


## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details
