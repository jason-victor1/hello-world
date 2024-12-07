# Hello World Smart Contract

This repository contains a simple "Hello World" smart contract that I wrote in Solidity.

## Description

The `HelloWorld` contract is a basic example of a smart contract on the Ethereum blockchain. It demonstrates the fundamental structure and syntax of a Solidity contract. This contract includes a single function that returns a static string "Hello World".

## Contract Code

The contract code is as follows:

```solidity
// SPDX-License-Identifier: MIT

pragma solidity ^0.8.28;

contract HelloWorld {
    function hello () external pure returns(string memory) {
        return "Hello World";
    }
}
```

### Explanation:

- **SPDX-License-Identifier**: Specifies the license type. Here it is MIT.
- **pragma solidity ^0.8.26**: Specifies the Solidity compiler version to use. The `^` symbol indicates that the contract is compatible with compiler versions 0.8.26 and above but below 0.9.0.
- **contract HelloWorld**: Defines a new contract named `HelloWorld`.
- **function hello() external pure returns (string memory)**: Defines a function named `hello` that is `external` (can be called from other contracts and transactions) and `pure` (does not modify or read from the blockchain state). It returns a string stored in memory.
- **`return "Hello World";`**: Specifies the return value of the `hello` function. The string `"Hello World"` is a literal and is returned as the output of the function.




