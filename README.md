© 2021 UHH Cryptocurrency

# UHHT Hip Hop Titanium ERC20 TOKEN

[Link](https://uhhcrypto.com/erc20-uhht)

![UHHTHipHopTitanium](UHHTHipHopTitanium.jpg)
_UHHT  Hip Hop Titanium holders will receive all the benefits included in the entire UHH Crypto Suite (UHH, UHHP, UHHB, UHHV)_

The popular cryptocurrency and blockchain system Ethereum is based on the use of tokens, which can be bought, sold, or traded. Ethereum was launched in 2015, and since then it has become one of the driving forces behind the popularity of cryptocurrency. In the Ethereum system, tokens represent a diverse range of digital assets, such as vouchers, IOUs, or even real-world, tangible objects. Ethereum tokens are smart contracts that make use of the Ethereum blockchain. ERC-20 is similar, in some respects, to bitcoin, Litecoin, and any other cryptocurrency; ERC-20 tokens are blockchain-based assets that have value and can be sent and received. The primary difference is that instead of running on their own blockchain, ERC-20 tokens are issued on the Ethereum network.

### What is an ERC20 token?
An ERC20 token is a blockchain-based asset with similar functionality to bitcoin, ether, and bitcoin cash: it can hold value and be sent and received. The major difference between ERC20 tokens and other cryptocurrencies is that ERC20 tokens are created and hosted on the Ethereum blockchain, whereas bitcoin and bitcoin cash are the native currencies of their respective blockchains. ERC20 tokens are stored and sent using Ethereum addresses and transactions, and use gas to cover transaction fees.

More than 200,000 ERC-20-compatible tokens exist on Ethereum's main network. The ERC-20 commands vital importance; it defines a common list of rules that all Ethereum tokens must adhere to. Some of these rules include how the tokens can be transferred, how transactions are approved, how users can access data about a token, and the total supply of tokens. 

ERC20 is an official protocol for proposing improvements to the Ethereum (ETH) network. ERC stands for Ethereum Request for Comment, and 20 is the proposal identifier. This is a common standard for creating tokens on the Ethereum blockchain. This token standard defines a set of rules that apply to all ERC20 tokens that allow them to interact seamlessly with one another. Wallets and exchanges use the standard to integrate various ERC20 tokens onto their platforms and facilitate exchanges between ERC20 tokens and other cryptocurrencies.

### Benefits of UHHT tokens

Holders of UHHT will have the opportunity to win a chance for VIP access to various Hip Hop events, including concerts, clubs, specials events, i.e. album listening parties, award shows, movie premieres, etc. Its also about free hip hip merchandise, exclusive pre-releases and DJ mixes.

### Source Code 

```
Source Code

/**
*Submitted for verification at Etherscan.io on 2020-11-21
*/

// File: @openzeppelin/contracts/GSN/Context.sol

// SPDX-License-Identifier: MIT

pragma solidity ^0.7.0;

/*
* @dev Provides information about the current execution context, including the
* sender of the transaction and its data. While these are generally available
* via msg.sender and msg.data, they should not be accessed in such a direct
* manner, since when dealing with GSN meta-transactions the account sending and
* paying for execution may not be the actual sender (as far as an application
* is concerned).
*
* This contract is only required for intermediate, library-like contracts.
*/
abstract contract Context {
function _msgSender() internal view virtual returns (address payable) {
return msg.sender;
}

function _msgData() internal view virtual returns (bytes memory) {
this; // silence state mutability warning without generating bytecode - see https://github.com/ethereum/solidity/issues/2691
return msg.data;
}
}

// File: @openzeppelin/contracts/access/Ownable.sol



pragma solidity ^0.7.0;

/**
* @dev Contract module which provides a basic access control mechanism, where
* there is an account (an owner) that can be granted exclusive access to
* specific functions.
*
* By default, the owner account will be the one that deploys the contract. This
* can later be changed with {transferOwnership}.
*
* This module is used through inheritance. It will make available the modifier
* `onlyOwner`, which can be applied to your functions to restrict their use to
* the owner.
*/
abstract contract Ownable is Context {
address private _owner;

event OwnershipTransferred(address indexed previousOwner, address indexed newOwner);

/**
* @dev Initializes the contract setting the deployer as the initial owner.
*/
constructor () {
address msgSender = _msgSender();
_owner = msgSender;
emit OwnershipTransferred(address(0), msgSender);
}

/**
* @dev Returns the address of the current owner.
*/
function owner() public view returns (address) {
return _owner;
}

/**
* @dev Throws if called by any account other than the owner.
*/
modifier onlyOwner() {
require(_owner == _msgSender(), "Ownable: caller is not the owner");
_;
}

/**
* @dev Leaves the contract without owner. It will not be possible to call
*
```
