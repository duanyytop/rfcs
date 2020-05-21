---
Number: "0024"
Category: Standards Track
Status: Proposal
Author: Cipher Wang, Dylan Duan
Organization: Nervos Foundation
Created: 2020-05-21
---

# CKB System Contract

## Abstract

This document shows a series of Nervos CKB system smart contracts information, including a brief introduction and _code_hash_, _out_point_(_tx_hash_ and _index_) in mainnet Lina and testnet Aggron so far.

## Motivation

Nervos Foundation providers a series of Nervos CKB system smart contracts, including _SECP256K1/blake160_, _SECP256K1/multisig_ and _anyone_can_pay_ for lock script and _Nervos DAO_, _Simple UDT_ for type script. To construct transactions with system smart contracts, the _code_hash_ and _out_point_ of system contract in mainnet Lina and testnet Aggron are needed.

## System Smart Contracts

### SECP256K1/blake160

SECP256K1/blake160 is a popular smart contract to signature and validate transaction in CKB.

SECP256K1/blake160 smart contract is for **lock script**:

- Lina

| parameter   | hash / number                                                        |
| ----------- | -------------------------------------------------------------------- |
| `code_hash` | `0x9bd7e06f3ecf4be0f2fcd2188b23f1b9fcc88e5d4b65a8637b17723bbda3cce8` |
| `tx_hash`   | `0x71a7ba8fc96349fea0ed3a5c47992e3b4084b031a42264a018e0072e8172e46c` |
| `index`     | `0`                                                                  |

- Aggron

| parameter   | hash / number                                                        |
| ----------- | -------------------------------------------------------------------- |
| `code_hash` | `0x9bd7e06f3ecf4be0f2fcd2188b23f1b9fcc88e5d4b65a8637b17723bbda3cce8` |
| `tx_hash`   | `0x6495cede8d500e4309218ae50bbcadb8f722f24cc7572dd2274f5876cb603e4e` |
| `index`     | `0`                                                                  |

<br />

### SECP256K1/multisig

SECP256K1/multisig is a smart contract which allows a group of users to sign a single transaction.

SECP256K1/multisig smart contract is for **lock script**:

- Lina

| parameter   | hash / number                                                        |
| ----------- | -------------------------------------------------------------------- |
| `code_hash` | `0x5c5069eb0857efc65e1bca0c07df34c31663b3622fd3876c876320fc9634e2a8` |
| `tx_hash`   | `0x71a7ba8fc96349fea0ed3a5c47992e3b4084b031a42264a018e0072e8172e46c` |
| `index`     | `1`                                                                  |

- Aggron

| parameter   | hash / number                                                        |
| ----------- | -------------------------------------------------------------------- |
| `code_hash` | `0x5c5069eb0857efc65e1bca0c07df34c31663b3622fd3876c876320fc9634e2a8` |
| `tx_hash`   | `0x6495cede8d500e4309218ae50bbcadb8f722f24cc7572dd2274f5876cb603e4e` |
| `index`     | `1`                                                                  |

<br />

### Nervos DAO

Nervos DAO is a smart contract and One function of Nervos DAO is to provide an dilution counter-measure for CKByte holders. By deposit in Nervos DAO, holders get proportional secondary rewards, which guarantee their holding are only affected by hardcapped primary issuance as in Bitcoin.

Nervos DAO smart contract is for **type script**:

- Lina

| parameter   | hash / number                                                        |
| ----------- | -------------------------------------------------------------------- |
| `code_hash` | `0x82d76d1b75fe2fd9a27dfbaa65a039221a380d76c926f378d3f81cf3e7e13f2e` |
| `tx_hash`   | `0xe2fb199810d49a4d8beec56718ba2593b665db9d52299a0f9e6e75416d73ff5c` |
| `index`     | `2`                                                                  |

- Aggron

| parameter   | hash / number                                                        |
| ----------- | -------------------------------------------------------------------- |
| `code_hash` | `0x82d76d1b75fe2fd9a27dfbaa65a039221a380d76c926f378d3f81cf3e7e13f2e` |
| `tx_hash`   | `0x96fea0dfaac1186fbb98fd452cb9b13976f9a00bcce130035fe2e30dac931d1d` |
| `index`     | `2`                                                                  |

<br />

### Simple UDT

Simple UDT provides a way to issue custom tokens on Nervos CKB.

Simple UDT smart contract is for **type script**:

- Aggron

| parameter   | hash / number                                                        |
| ----------- | -------------------------------------------------------------------- |
| `code_hash` | `0x48dbf59b4c7ee1547238021b4869bceedf4eea6b43772e5d66ef8865b6ae7212` |
| `tx_hash`   | `0x0e7153f243ba4c980bfd7cd77a90568bb70fd393cb572b211a2f884de63d103d` |
| `index`     | `0`                                                                  |

<br />

### anyone_can_pay

anyone_can_pay is is a smart contract that can accept any amount of payment.

anyone_can_pay smart contract is for **lock script**:

- Aggron

| parameter   | hash / number                                                        |
| ----------- | -------------------------------------------------------------------- |
| `code_hash` | `0x6a3982f9d018be7e7228f9e0b765f28ceff6d36e634490856d2b186acf78e79b` |
| `tx_hash`   | `0x69c70d65832cdfd97fe78d32eb25f840232f6b8cb6445464f11dad891b11fd83` |
| `index`     | `0`                                                                  |
