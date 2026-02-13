# StellarSave

## USDC Micro-Savings & Dollar Protection App Built on Stellar

---

# Overview

StellarSave is a micro-savings and dollar-protection application built on the Stellar Network. It enables users in high-inflation economies to save securely in USDC, protect their earnings from currency devaluation, and build financial stability through automated savings tools.

The platform leverages Stellar’s fast, low-cost blockchain infrastructure to provide instant, transparent, and borderless access to digital dollar savings.

StellarSave is designed for financial inclusion, empowering individuals without access to traditional dollar banking systems.

---

# Problem Statement

In many emerging markets (e.g., Nigeria and other high-inflation economies):

a. Local currencies rapidly lose value.  
b. Access to USD bank accounts is restricted or expensive.  
c. Savings options are limited and unreliable.  
d. Many individuals lack structured saving mechanisms.  
e. Small daily earnings are difficult to accumulate efficiently.

As a result, millions are unable to protect their income or build long-term financial security.

---

# Solution

StellarSave provides:

## 1. USDC-Based Savings

Users can:
a. Deposit funds and convert to USDC on Stellar.  
b. Hold savings in a stable, dollar-backed digital asset.  
c. Protect value from inflation and currency volatility.

## 2. Automated Micro-Savings (Round-Up System)

- Automatically round up transactions.
- Convert spare change into USDC savings.
- Encourage disciplined saving habits.

Example:  
If a user spends $4.60 → $0.40 is automatically saved in USDC.

## 3. Time-Locked Vaults

Users can:
a. Lock savings for predefined periods (e.g., 30, 90, 180 days).  
b. Prevent impulsive withdrawals.  
c. Earn reward incentives for completing lock periods.

## 4. Yield Strategies (Future Phase)

a. Integrate low-risk DeFi yield mechanisms.  
b. Provide transparent, on-chain yield distribution.  
c. Display real-time vault performance.

---

# Why Stellar?

1. 2–5 second transaction finality
2. Extremely low transaction fees
3. Built for cross-border payments
4. Native support for USDC
5. Secure and decentralized infrastructure

StellarSave utilizes:
a. USDC on Stellar for stable savings  
b. XLM for transaction fees  
c. Soroban smart contracts for vault automation (Phase 2)

---

# Backend Architecture

The backend powers automation, vault metadata management, and integration with Stellar smart contracts.

It does NOT custody user funds.

All funds remain in user-controlled wallets or smart contracts.

---

## Tech Stack

- Node.js
- Express
- TypeScript
- PostgreSQL
- Stellar SDK
- Soroban RPC
- Redis (optional)

---

## Core Responsibilities

### 1. Vault Metadata

Stores:

- Vault ID
- User public key
- Lock duration
- Deposit amount
- Maturity date
- Vault status

Funds are locked via Soroban smart contracts.

---

### 2. Round-Up Engine

- Tracks transaction activity
- Calculates round-up savings
- Initiates USDC micro-deposits
- Logs savings behavior

---

### 3. Smart Contract Interaction

- Submits contract calls
- Monitors vault maturity
- Triggers reward distribution
- Listens for blockchain events

---

### 4. Fiat On/Off Ramp Integration

- Payment provider integration
- USDC conversion logic
- Webhook handling

---

# Security

- No private key custody
- JWT authentication
- Rate limiting
- Input validation
- Secure webhook verification

---

# Setup

```bash
npm install
npm run dev
```
