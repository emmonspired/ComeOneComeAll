# ComeOneComeAll
[`#HowToBUIDL` (2/n) :: Your First Contract Come One Come All!](https://medium.com/coinmonks/howtobuidl-2ofn-come-one-come-all-8a3e0ee706b1)
By the end of this post, you’ll write your very first SmartContract called the GreatestShow.

Come one! Come all! Come join the great Digital Railroad! There is no barrier to entry, as long as you participate within the framework of rules known as decentralized consensus. This means you’ll work for it. It won’t come easy but at least you’ve taken the 1st step. Come build the digital railroads of tomorrow! Three meals a day! Roof over your head! Fair and ample wages! Come, make your fortune! Not everyone will be up for the challenge. I guess I’ll leave that up to you. Opportunity awaits you.
If you haven’t, be sure to catch [BUIDL :: Dev Environment Setup](https://medium.com/coinmonks/howtobuidl-series-1-of-n-bf51e248243d) before reading.

## Contracts
Please see the [contracts/](contracts) directory.

## Overview
There is one primary contracs: `GreatestShow.sol`

### GreatestShow 
This contract constructor accepts a string for the name of the ringMaster. Sufficient gas should be supplied.
1. set/get Available Seat Count
1. Define Performance struct and maintain Performance[] performances as well as getPerformance
1. Maintain a mapping(address => uint256) internal tickets;
1. Provide a function () payable public fallback function to assign msg.sender a number of tickets based on msg.value.

## Develop
Contracts are written in [Solidity][solidity] and tested using [Truffle][truffle] and [testrpc][testrpc]. Library contracts sourced from [OpenZeppelin.org][openzeppelin].

### Dependencies
```bash
# Install Truffle, testrpc, and dependency packages:
$ npm install
$ truffle compile
```
