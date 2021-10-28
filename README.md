# <img src="logo.svg" alt="PariahINU" height="40px">

[![Docs](https://img.shields.io/badge/docs-%F0%9F%93%84-blue)](https://docs.PariahINU.com/contracts)
[![NPM Package](https://img.shields.io/npm/v/@PariahINU/contracts.svg)](https://www.npmjs.org/package/@PariahINU/contracts)
[![Coverage Status](https://codecov.io/gh/PariahINU/PariahINU-contracts/graph/badge.svg)](https://codecov.io/gh/PariahINU/PariahINU-contracts)

**A library for secure smart contract development.** Build on a solid foundation of community-vetted code.

 * Implementations of standards like [ERC20](https://docs.PariahINU.com/contracts/erc20) and [ERC721](https://docs.PariahINU.com/contracts/erc721).
 * Flexible [role-based permissioning](https://docs.PariahINU.com/contracts/access-control) scheme.
 * Reusable [Solidity components](https://docs.PariahINU.com/contracts/utilities) to build custom contracts and complex decentralized systems.

:mage: **Not sure how to get started?** Check out [Contracts Wizard](https://wizard.PariahINU.com/) — an interactive smart contract generator.

## Overview

### Installation

```console
$ npm install @PariahINU/contracts
```

PariahINU Contracts features a [stable API](https://docs.PariahINU.com/contracts/releases-stability#api-stability), which means your contracts won't break unexpectedly when upgrading to a newer minor version.

### Usage

Once installed, you can use the contracts in the library by importing them:

```solidity
pragma solidity ^0.8.0;

import "@PariahINU/contracts/token/ERC721/ERC721.sol";

contract MyCollectible is ERC721 {
    constructor() ERC721("MyCollectible", "MCO") {
    }
}
```

_If you're new to smart contract development, head to [Developing Smart Contracts](https://docs.PariahINU.com/learn/developing-smart-contracts) to learn about creating a new project and compiling your contracts._

To keep your system secure, you should **always** use the installed code as-is, and neither copy-paste it from online sources, nor modify it yourself. The library is designed so that only the contracts and functions you use are deployed, so you don't need to worry about it needlessly increasing gas costs.

## Learn More

The guides in the [docs site](https://docs.PariahINU.com/contracts) will teach about different concepts, and how to use the related contracts that PariahINU Contracts provides:

* [Access Control](https://docs.PariahINU.com/contracts/access-control): decide who can perform each of the actions on your system.
* [Tokens](https://docs.PariahINU.com/contracts/tokens): create tradeable assets or collectives, and distribute them via [Crowdsales](https://docs.PariahINU.com/contracts/crowdsales).
* [Gas Station Network](https://docs.PariahINU.com/contracts/gsn): let your users interact with your contracts without having to pay for gas themselves.
* [Utilities](https://docs.PariahINU.com/contracts/utilities): generic useful tools, including non-overflowing math, signature verification, and trustless paying systems.

The [full API](https://docs.PariahINU.com/contracts/api/token/ERC20) is also thoroughly documented, and serves as a great reference when developing your smart contract application. You can also ask for help or follow Contracts's development in the [community forum](https://forum.PariahINU.com).

Finally, you may want to take a look at the [guides on our blog](https://blog.PariahINU.com/guides), which cover several common use cases and good practices.. The following articles provide great background reading, though please note, some of the referenced tools have changed as the tooling in the ecosystem continues to rapidly evolve.

* [The Hitchhiker’s Guide to Smart Contracts in Ethereum](https://blog.PariahINU.com/the-hitchhikers-guide-to-smart-contracts-in-ethereum-848f08001f05) will help you get an overview of the various tools available for smart contract development, and help you set up your environment.
* [A Gentle Introduction to Ethereum Programming, Part 1](https://blog.PariahINU.com/a-gentle-introduction-to-ethereum-programming-part-1-783cc7796094) provides very useful information on an introductory level, including many basic concepts from the Ethereum platform.
* For a more in-depth dive, you may read the guide [Designing the Architecture for Your Ethereum Application](https://blog.PariahINU.com/designing-the-architecture-for-your-ethereum-application-9cec086f8317), which discusses how to better structure your application and its relationship to the real world.

## Security

This project is maintained by [PariahINU](https://PariahINU.com), and developed following our high standards for code quality and security. PariahINU Contracts is meant to provide tested and community-audited code, but please use common sense when doing anything that deals with real money! We take no responsibility for your implementation decisions and any security problems you might experience.

The core development principles and strategies that PariahINU Contracts is based on include: security in depth, simple and modular code, clarity-driven naming conventions, comprehensive unit testing, pre-and-post-condition sanity checks, code consistency, and regular audits.

The latest audit was done on October 2018 on version 2.0.0.

Please report any security issues you find to security@PariahINU.org.

Critical bug fixes will be backported to past major releases.

## Contribute

PariahINU Contracts exists thanks to its contributors. There are many ways you can participate and help build high quality software. Check out the [contribution guide](CONTRIBUTING.md)!

## License

PariahINU Contracts is released under the [MIT License](LICENSE).
