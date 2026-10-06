# HODLPay

**Non-Custodial Escrow Infrastructure on Stellar**

HODLPay is a non-custodial escrow payment platform built on the Stellar network using Soroban smart contracts.

It allows users to create escrow agreements, lock Stellar assets in a smart contract, and release or refund funds based on the terms of the agreement.

> **Network:** Stellar Testnet  
> **Status:** MVP  
> **Technology:** Stellar + Soroban

---

## Overview

Traditional escrow services require users to trust a centralized third party to hold and release funds.

HODLPay uses Soroban smart contracts to provide a programmable escrow layer where funds remain locked until the conditions of an agreement are satisfied.

### Core Flow

**Create Escrow → Fund Escrow → Lock Funds → Release or Refund**

---

## Problem

Freelancers, developers, agencies, and clients need a simple and transparent way to exchange payments for services.

Traditional escrow solutions can introduce:

- Centralized custody
- High fees
- Delayed settlement
- Limited transparency
- Counterparty risk

HODLPay provides a blockchain-based escrow alternative where funds are controlled by smart-contract logic rather than a centralized intermediary.

---

## Solution

HODLPay allows users to create an escrow agreement specifying:

- Payer
- Payee
- Asset
- Amount
- Escrow terms
- Release conditions
- Refund conditions

The agreed funds are deposited into the Soroban escrow contract and remain locked until the appropriate action is executed.

---

## Features

### Escrow Creation

Create an escrow agreement with:

- Payer wallet
- Payee wallet
- Asset
- Amount
- Escrow terms

### Non-Custodial Fund Locking

Funds are locked inside the Soroban smart contract rather than being held by a centralized platform.

### Fund Release

Release escrowed funds to the intended recipient when the agreed conditions are satisfied.

### Refund

Return escrowed funds to the payer when the refund condition is triggered.

### Escrow Status

Track the current state of an escrow:

```text
Created
   ↓
Funded
   ↓
Locked
   ↓
Released / Refunded
