---
layout: post
title: "What GitHub orgs are relevant?"
date: 2018-09-25T19:32:06Z
image: /assets/img/logo.png
---

Before anything else, let's see what is out there -- what organizations on GitHub are relevant to working on Ethereum?

I know that [@ethereum](https://github.com/ethereum) is the main entry point. But:

### Are there other official @ethereum organizations on GitHub?

Using GitHub search for this is, unsurprisingly, unhelpful initially. Searching for `ethereum` brings up [over 18,000 repositories](https://github.com/search?q=ethereum&type=Repositories), and over a thousand users. Sorting by stars and using only the first couple of pages, we see a few more interesting repositories if we ignore ones in @ethereum:

- [chaozh/awesome-blockchain-cn](https://github.com/chaozh/awesome-blockchain-cn) - "收集所有区块链(BlockChain)技术开发相关资料，包括Fabric和Ethereum开发资料."
- [trufflesuite/truffle](https://github.com/trufflesuite/truffle) - "The most popular Ethereum development framework"
- [OpenZeppelin/openzeppelin-solidity](https://github.com/OpenZeppelin/openzeppelin-solidity) - "OpenZeppelin is a library for secure smart contract development"
- [paritytech/parity-ethereum](https://github.com/paritytech/parity-ethereum) - "The fast, light, and robust EVM and WASM client."
- [yeasy/blockchain_guide](https://github.com/yeasy/blockchain_guide) - "Introduce blockchain related technologies, from theory to practice with bitcoin, ethereum and hyperledger."
- [ethereumbook/ethereumbook](https://github.com/ethereumbook/ethereumbook) - "Mastering Ethereum, by Andreas M. Antonopoulos, Gavin Wood"
- [Scanate/EthList](https://github.com/Scanate/EthList) - "The Comprehensive Ethereum Reading List"
- [ConsenSys/smart-contract-best-practices](https://github.com/ConsenSys/smart-contract-best-practices) - "A guide to smart contract security best practices"
- [aquynh/capstone](https://github.com/aquynh/capstone) - "Capstone disassembly/disassembler framework: Core (Arm, Arm64, EVM, M68K, M680X, Mips, PPC, Sparc, SystemZ, TMS320C64x, X86, X86_64, XCore) + bindings (Python, Java, Ocaml, PowerShell, Visual Basic)"
- [kennethreitz/awesome-coins](https://github.com/kennethreitz/awesome-coins) - "₿ A guide (for humans!) to cryto-currencies and their algos."
- [ethereum-mining/ethminer](https://github.com/ethereum-mining/ethminer) - "Ethereum miner with OpenCL, CUDA and stratum support"
- [jpmorganchase/quorum](https://github.com/jpmorganchase/quorum) - "A permissioned implementation of Ethereum supporting data privacy"

This list is interesting; while the top-starred repos isn't exactly the best metric to use for discoverability, it matches what I know about [@ethereum](https://github.com/ethereum) that the orgs represented here aren't directly supported by the Ethereum. ParityTech might be the main exception, along with Zeppelin, ConsenSys, and Trufflesuite.

Really, the main takeaway for me here is another signal that all of the code used by the Ethereum Foundation is within @ethereum. I've already been told this by the community, so it's not massive news. But I am going to assume that if you're working with Ethereum, you'll be landing in the @ethereum organization itself quite often, as opposed to something like in Protocol Labs where you could end up wandering through @libp2p more than @ipfs in some cases.

In short, no. @ethereum is the main organization.

### How is this different from the Ethereum Foundation?

Unlike with Zcash, which [splits out the foundation](https://github.com/zcashfoundation) and [the main GitHub organization](https://github.com/zcash), the Ethereum Foundation website points directly to the @ethereum GitHub, too. The Foundation funds development work.

There's no such split on GitHub, here.


### **And where are the EIPs?**

Well, that was an easy question to answer. They're pinned on @ethereum. So, they're at [ethereum/EIPs](https://github.com/ethereum/EIPs).

### **What other organizations are relevant?**

This question was written before I answered the above. At some point, I'll find myself digging into Zeppelin, ConsenSys's work, and so on; for now, I want to focus on @ethereum and how the organization works and structures information, before moving further.

### **What are the main repositories in the @ethereum organization?**

Well, the [go-ethereum](https://github.com/ethereum/go-ethereum), [aleth](https://github.com/ethereum/aleth), and [EIPs](https://github.com/ethereum/EIPs) repos are pinned. [Solidity](https://github.com/ethereum/solidity) looks like it _ought_ to be pinned, but it isn't. I'll have to find someone to contact about that. Same with [mist](https://github.com/ethereum/mist) and [web3.js](https://github.com/ethereum/web3.js) - all three of these have over 6k stars.

Let's dive into those next.
