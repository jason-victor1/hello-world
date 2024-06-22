# Hello World Smart Contract

This repository contained a simple "Hello World" smart contract that I wrote in Solidity.

## Description

The `HelloWorld` contract was a basic example of a smart contract on the Ethereum blockchain. It demonstrated the fundamental structure and syntax of a Solidity contract. This contract included a single function that returned a static string "Hello World".

## Contract Code

The contract code was as follows:

```solidity
// SPDX-License-Identifier: MIT

pragma solidity ^0.8.26;

contract HelloWorld {
    function hello () external pure returns(string memory) {
        return "Hello World";
    }
}
```

### Explanation:

- **SPDX-License-Identifier**: Specified the license type. Here it was MIT.
- **pragma solidity ^0.8.25**: Specified the Solidity compiler version to use. The `^` symbol indicated that the contract was compatible with compiler versions 0.8.25 and above but below 0.9.0.
- **contract HelloWorld**: Defined a new contract named `HelloWorld`.
- **function hello() external pure returns (string memory)**: Defined a function named `hello` that was `external` (could be called from other contracts and transactions) and `pure` (did not modify or read from the blockchain state). It returned a string stored in memory.

## Functions

### `hello()`

- **Description**: This function was a simple example of a Solidity function that returned a static string. When called, it would return the string "Hello World".
- **Visibility**: `external` - The function could be called from other contracts or from transactions, but not from within the same contract.
- **State Mutability**: `pure` - The function did not read from or modify the blockchain state. It purely computed and returned a value.
- **Returns**: `string memory` - The function returned a string stored in memory.
