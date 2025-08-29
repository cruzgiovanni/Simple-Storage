# My Solidity Smart Contracts 🎉

**Solidity Version**: ^0.8.30  
**IDE**: [Remix IDE](https://remix.ethereum.org/)  

---

## 📜 Description

This repository contains **my first smart contracts** written in Solidity! 🥳  
They were created to learn the **fundamentals of blockchain programming** and tested on the **Sepolia testnet**.

**Contracts deployed (Sepolia):**  
- **SimpleStorage:** [0x1e0463625780139cB5e97C243cBd79Ce30482cE2](https://sepolia.etherscan.io/address/0x1e0463625780139cB5e97C243cBd79Ce30482cE2)  
- **StorageFactory:** [0x9c193b21c36f52c91f3afaee8344c4ef0b9e3557](https://sepolia.etherscan.io/address/0x9c193b21c36f52c91f3afaee8344c4ef0b9e3557)  
- *(ExtraStorage was tested locally in Remix IDE for learning purposes.)*

---

## Contracts Overview

### 1. **SimpleStorage.sol**
- **Stores a favorite number** (`favoriteNumber`)  
- **Retrieves the stored number** using `retrieve()`  
- **Adds people with name and favorite number** via a dynamic `People` array  
- **Maps names to favorite numbers** using `nameToFavoriteNumber`  

---

### 2. **StorageFactory.sol**

## Key concepts learned

- How to **deploy contracts from another contract**  
- How to **use arrays of contracts** to handle multiple instances  
- How to **implicitly use addresses and ABI** when calling other contracts  

---

### 3. **ExtraStorage.sol**

## Key concepts learned

- **Inheritance in Solidity**  
- **Overriding functions** to modify existing behavior  

---

## What I Learned

### 1. Basic Solidity contract structure
- State variables (`uint256 favoriteNumber;`)  
- **Structs**, **dynamic arrays**, and **mappings**  

### 2. Read vs write functions
- Functions that **modify the blockchain** (like `store` or `addPerson`) consume **gas**  
- Functions marked as **view** or **pure** (like `retrieve`) do **not** consume gas  

### 3. Memory vs calldata vs storage
- **memory**: temporary and mutable data  
- **calldata**: temporary but immutable (more gas-efficient for parameters)  
- **storage**: permanent data on the blockchain  

### 4. Mappings
- Fast lookup using `nameToFavoriteNumber` without looping through an array  

### 5. Inheritance and Factory Pattern
- **Factory pattern** to manage multiple contracts  
- **Override** to change the behavior of inherited functions  

### 6. Ethereum in practice
- Every deployed contract is **public and immutable** on the Ethereum network  
- State-changing functions require **transactions (gas)**  
- Read-only functions are **free to call**  