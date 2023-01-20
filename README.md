<img width="1200" alt="Labs" src="https://user-images.githubusercontent.com/99700157/213291931-5a822628-5b8a-4768-980d-65f324985d32.png">

> Chainstack is the leading suite of services connecting developers with Web3 infrastructure.   

<p align="center">
  <a target="_blank" href="https://chainstack.com/build-better-with-ethereum/"><img src="https://img.shields.io/badge/Ethereum-3C3C3D?style=for-the-badge&logo=Ethereum&logoColor=white" /></a>&nbsp;
  <a target="_blank" href="https://chainstack.com/build-better-with-bnb-smart-chain/"><img src="https://tinyurl.com/mp2wu3xx" /></a>&nbsp;
</p>

<p align="center">
  • <a target="_blank" href="https://chainstack.com/">Homepage</a> •
  <a target="_blank" href="https://chainstack.com/protocols/">Supported protocols</a> •
  <a target="_blank" href="https://chainstack.com/blog/">Chainstack blog</a> •
  <a target="_blank" href="https://docs.chainstack.com/quickstart/">Chainstack docs</a> •
  <a target="_blank" href="https://docs.chainstack.com/quickstart/">Blockchain API reference</a> •
  <a target="_blank" href="https://console.chainstack.com/user/account/create">Start for free</a> •
</p>

# Querying full and archive EVM nodes with Python

This project allows the retrieval of historical data from the blockchain programmatically, switching between a full and archive node provider when necessary.

See the full tutorial on the Chainstack blog:
* [Querying full and archive Ethereum nodes with Python](https://chainstack.com/querying-full-and-archive-evm-nodes-with-python/)

## Project details

This repository holds the Python version of a tool to query common state functions. Some essential functions include getting an address balance and storage at a given position, a contract bytecode, or even the whole transactions included on a given block.

This tool queries the blockchain using the web3 and inquirer libraries for Python. 

## Quick start

### Clone this repository

```sh
git clone https://github.com/yieniggu/full-vs-archive-querys-py.git
```

### Install dependencies

```sh
pip install web3 inquirer
```

### Add a full and archive node RPC URL to utils.py

Open `utils.py` in the `src` directory and add your nodes RPC URLs:

```py
# Init full and archive provider
full_node_provider = Web3(
    Web3.HTTPProvider(
        "CHAINSTACK_FULL_NODE_URL"
    )
)
archive_node_provider = Web3(
    Web3.HTTPProvider(
        "CHAINSTACK_ARCHIVE_NODE_URL"
    )
)
```

### Run the program

```sh
python main.py
```

## Prerequisites

* Python ^3.9.16
* A full and archive node RPC endpoints.

Deploy a full and archive node with Chainstack:

1. [Sign up with Chainstack](https://console.chainstack.com/user/account/create).  
1. [Deploy a node](https://docs.chainstack.com/platform/join-a-public-network).  
1. [View node access and credentials](https://docs.chainstack.com/platform/view-node-access-and-credentials). 

## Dependencies

* web3.py ^5.31.3
* inquirer ^3.1.2

## Install

To install this project:

Clone this repository:

```sh
git clone https://github.com/yieniggu/full-vs-archive-querys-py.git
```

Install the dependencies in the project's directory:

```sh
cd query-full-and-archive-nodes-python
```

```sh
pip install web3 inquirer
```