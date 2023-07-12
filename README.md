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
* Tm-db fork from:            https://github.com/sei-protocol/tm-db/releases/tag/v0.0.4
* Ethermint fork from: https://github.com/evmos/ethermint/releases/tag/v0.22.0

文件状态描述:

- ✅ Fork，文件夹内无任何修改
- 🟥 Fork，文件夹内有部分内容修改
- ❌ Fork，有代码改动
- 🟢 无需审计

```
.
├── LICENSE.md                          🟢 无需审计: 用于版权说明
├── Makefile                            🟢 无需审计: 用于编译
├── README.md                           🟢 无需审计: 用于项目描述
├── aclmapping                          ✅ 整个目录fork https://github.com/sei-protocol/sei-chain/tree/3.0.4/aclmapping
├── app                                 🟥 整个目录Fork https://github.com/sei-protocol/sei-chain/tree/3.0.4/app , 但部分内容修改
│   ├── abci.go                             ❌ Fork 后，有代码改动 
│   ├── ante                                ✅ Fork，无任何修改 https://github.com/evmos/ethermint/tree/v0.22.0/app/ante 
│   ├── ante2                               🟧自己添加
│   │   ├── ante2.go                            ❌ Fork 后，有代码改动 
│   │   └── ante2_test.go                       ❌ Fork 后，有代码改动 
│   ├── antedecorators                      ✅ 整个目录fork https://github.com/sei-protocol/sei-chain/tree/3.0.4/app/antedecorators
│   ├── app.go                              ❌ Fork，文件内有部分内容修改
│   ├── app_test.go                         ❌ Fork，文件内有部分内容修改
│   ├── apptesting                          🟥 Fork，文件夹内有部分内容修改
│   │   └── test_suite.go                   ❌ Fork，文件内有部分内容修改
│   ├── const.go                            🟢 无需审计，无任何修改
│   ├── encoding.go                         🟢 无需审计，无任何修改
│   ├── export.go                           🟢 无需审计，无任何修改
│   ├── genesis.go                          🟢 无需审计，无任何修改
│   ├── params                              🟥 整个目录Fork https://github.com/sei-protocol/sei-chain/tree/3.0.4/app/params , 但部分内容修改
│   │   ├── amino.go                            ❌ Fork，文件内有部分内容修改
│   │   ├── config.go                           ❌ Fork，文件内有部分内容修改
│   │   ├── doc.go                              ❌ Fork，文件内有部分内容修改
│   │   ├── encoding.go                         ❌ Fork，文件内有部分内容修改
│   │   └── proto.go                            ❌ Fork，文件内有部分内容修改
│   ├── test_helpers.go                     🟢 无需审计，无任何修改
│   ├── upgrade_test.go                     🟢 无需审计，无任何修改
│   ├── upgrades.go                         🟢 无需审计，无任何修改
│   └── utils.go                            🟢 无需审计，无任何修改
├── client                              🟥 Fork 后，有代码改动      
│   ├── crypto                              🟥 Fork，文件内有部分内容修改
│   │   ├── armor.go                            ❌ Fork，文件内有部分内容修改
│   │   ├── keys                                🟥 Fork，文件内有部分内容修改
│   │   │ └── bcrypt                                ✅ Fork，无任何修改 https://github.com/golang/crypto/tree/master/bcrypt
│   │   │     ├── base64.go                         ✅ Fork，无任何修改
│   │   │     └── bcrypt.go                         ✅ Fork，无任何修改
│   │   └── xsalsa20symmetric               🟥 Fork，文件内有部分内容修改
│   │     ├── symmetric.go                      ❌ Fork，文件内有部分内容修改
│   │     └── symmetric_test.go                 ❌ Fork，文件内有部分内容修改
│   └── keys                                🟥 Fork，文件内有部分内容修改
│     ├── add.go                                ❌ Fork，文件内有部分内容修改
│     ├── codec.go                              ❌ Fork，文件内有部分内容修改
│     ├── codec_test.go                         ❌ Fork，文件内有部分内容修改
│     ├── export_evm.go                         ❌ Fork，文件内有部分内容修改
│     ├── import_evm.go                         ❌ Fork，文件内有部分内容修改
│     ├── root.go                               ❌ Fork，文件内有部分内容修改
│     └── utils.go                              ❌ Fork，文件内有部分内容修改
├── cmd                                 🟥 整个目录Fork https://github.com/sei-protocol/sei-chain/tree/3.0.4/cmd，有代码改动
│   └── fbchaind                            🟢 无需审计
│       ├── cmd                                 🟥 整个目录fork: from https://github.com/sei-protocol/sei-chain/tree/3.0.4/cmd/seid/cmd 内有部分内容修改
│       └── main.go                             ❌ Fork 后，有代码改动
├── codecov.yml                         🟢 无需审计: 用于配置文件
├── config.yml                          🟢 无需审计: 用于配置文件
├── crypto                              ✅ 整个目录fork: from https://github.com/evmos/ethermint/tree/v0.22.0/crypto
├── docker                              ✅ 整个目录fork: from https://github.com/sei-protocol/sei-chain/tree/3.0.4/docker
├── docs                                ✅ 整个目录fork: from https://github.com/sei-protocol/sei-chain/tree/3.0.4/docs
├── encoding                            ✅ 整个目录fork: from https://github.com/evmos/ethermint/tree/v0.22.0/encoding
├── ethereum                            ✅ 整个目录fork: from https://github.com/fibonacci-chain/core-protocol/tree/main/ethereum/eip712
├── go.mod                              🟢 依赖文件，无需审计
├── go.sum                              🟢 依赖文件，无需审计
├── indexer                             ✅ 整个目录fork: from https://github.com/evmos/ethermint/tree/v0.22.0/indexer
├── integration_test                    🟢 测试文件，无需审计
├── loadtest                            🟢 测试文件，无需审计
├── parallelization                     🟢 测试文件，无需审计
├── proto                               ✅ 整个目录fork: from https://github.com/sei-protocol/sei-chain/tree/3.0.4/proto
├── rpc                                 ✅ 整个目录fork: from https://github.com/evmos/ethermint/tree/v0.22.0/rpc
├── scripts                             ✅ 整个目录fork: from https://github.com/sei-protocol/sei-chain/tree/3.0.4/scripts
├── server                              ✅ 整个目录fork: from https://github.com/evmos/ethermint/tree/v0.22.0/server
├── store                               ✅ 整个目录fork: from https://github.com/sei-protocol/sei-chain/tree/3.0.4/store
├── sync                                ✅ 整个目录fork: from https://github.com/sei-protocol/sei-chain/tree/3.0.4/sync
├── target                              🟢 无需审计，配置文件夹
├── tests                               🟢 无需审计，测试文件夹
├── testutil                            🟢 无需审计，测试文件夹
├── wasmbinding                         ✅ 整个目录fork: from https://github.com/sei-protocol/sei-chain/tree/3.0.4/wasmbinding
└── x                                   🟥 整个目录Fork https://github.com/sei-protocol/sei-chain/tree/3.0.4/x , 但部分内容修改, 添加evm模块
    ├── README.md                       🟢 无需审计，说明文件
    ├── dex                             ✅ 整个目录fork: from https://github.com/sei-protocol/sei-chain/tree/3.0.4/x/dex
    ├── evm                             ✅ 整个目录fork: from https://github.com/evmos/ethermint/tree/v0.22.0/x/evm
    ├── feemarket                       ✅ 整个目录fork: from https://github.com/evmos/ethermint/tree/v0.22.0/x/feemarket
    ├── mint                            ✅ 整个目录fork: from https://github.com/sei-protocol/sei-chain/tree/3.0.4/x/mint
    ├── oracle                          ✅ 整个目录fork: from https://github.com/sei-protocol/sei-chain/tree/3.0.4/x/oracle
    ├── store                           ✅ 整个目录fork: from https://github.com/sei-protocol/sei-chain/tree/3.0.4/x/store
    └── tokenfactory                    ✅ 整个目录fork: from https://github.com/sei-protocol/sei-chain/tree/3.0.4/x/tokenfactory

```

<div align="center">
  <h4 align="center">
    Thanks for your contribution
  </h4>
  <a href="https://github.com/fibonacci-chain/core-protocol/issues">
    <img src="https://contrib.rocks/image?repo=fibonacci-chain/core-protocol" />
  </a>
</div>
