# Fibonacci Chain

![FIBOLOGO.png](docs%2FFIBOLOGO.png)

Fibonacci is a forward-looking, high-performance public blockchain with the ability to be composable and iterative, and it is fully compatible with both EVM and WASM.

# fbchain
**fbchain** is a blockchain built using Cosmos SDK and Tendermint. It is built using the Cosmos SDK and Tendermint core

Leveraging its highly scalable underlying framework, Fibonacci is dedicated to building a customized SocialFi ecosystem for the social sector and creator economy.

# Documentation
For the most up to date documentation please visit https://fibochain.org

# Fibonacci Chain Ecosystem
Fibonacci Chain Network is an L1 blockchain with a built-in on-chain orderbook that allows smart contracts easy access to shared liquidity. Fibonacci Chain architecture enables composable apps that maintain modularity.

Fibonacci Chain Network serves as the matching core of the ecosystem, offering superior reliability and ultra-high transaction speed to ecosystem partners, each with their own functionality and user experience. Anyone can create a DeFi application that leverages Fibonacci Chain's liquidity and the entire ecosystem benefits.

Developers, traders, and users can all connect to Fibonacci Chain as ecosystem partners benefiting from shared liquidity and decentralized financial primitives.

# Testnet
## Get started
**How to validate on the Fibonacci Chain Testnet**
*This is the Fibonacci Chain Testnet-1 (fibonacci-testnet-1)*

## Hardware Requirements
**Minimum**
* 32 GB RAM
* 1 TB NVME SSD
* 16 Cores (modern CPU's)

## Operating System 

> Linux (x86_64) or Linux (amd64) Recommended Arch Linux

**Dependencies**
> Prerequisite: go1.18+ required.
* Arch Linux: `pacman -S go`
* Ubuntu: `sudo snap install go --classic`

> Prerequisite: git. 
* Arch Linux: `pacman -S git`
* Ubuntu: `sudo apt-get install git`

> Optional requirement: GNU make. 
* Arch Linux: `pacman -S make`
* Ubuntu: `sudo apt-get install make`


# Fibonacci Chaind Dependencies report

* Cosmos sdk fork from: https://github.com/sei-protocol/sei-cosmos/releases/tag/v0.2.47
* Tendermint fork from:  https://github.com/sei-protocol/sei-tendermint/releases/tag/v0.2.24
* Wasmd fork from:         https://github.com/sei-protocol/sei-wasmd/releases/tag/v0.0.2
* Ibc-go/v3  fork from:     https://github.com/sei-protocol/sei-ibc-go/releases/tag/v3.1.0
* Iavl fork from:                https://github.com/sei-protocol/sei-iavl/releases/tag/v0.1.4
* Tm-db for from:            https://github.com/sei-protocol/tm-db/releases/tag/v0.0.4

```text
The following is the relevant directory of our forked project

├─aclmapping                            fork from https://github.com/sei-protocol/sei-chain
├─app                                   [x]
├─client                                [x]
├─cmd                                   [x]
├─crypto                                fork from https://github.com/evmos/ethermint
├─docker                                fork from https://github.com/evmos/ethermint
├─docs                                  fork from https://github.com/evmos/ethermint
├─encoding                              fork from https://github.com/evmos/ethermint
├─ethereum                              fork from https://github.com/evmos/ethermint
├─indexer                               fork from https://github.com/evmos/ethermint
├─integration_test                      [x]
├─loadtest                              [x]
├─parallelization                       [x]
├─proto                                 fork from https://github.com/evmos/ethermint
├─rpc                                   [x]
├─scripts                               [x]
├─server                                fork from https://github.com/evmos/ethermint
├─store                                 [x]
├─sync                                  [x]
├─target                                [x]
├─tests                                 [x]
├─testutil                              [x]
├─types                                 [x]
├─utils                                 [x]
├─wasmbinding                           fork from https://github.com/sei-protocol/sei-chain     
├─x
│ ├─dex                                 [x]
│ ├─epoch                               fork from https://github.com/sei-protocol/sei-chain
│ ├─evm                                 fork from https://github.com/evmos/ethermint
│ ├─feemarket                           form from https://github.com/evmos/ethermint
│ ├─mint                                [x]
│ ├─oracle                              fork from https://github.com/sei-protocol/sei-chain
│ ├─store                               fork from https://github.com/sei-protocol/sei-chain
└───tokenfactory                        fork from https://github.com/sei-protocol/sei-chain
```