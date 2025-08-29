# My First Smart Contract with Solidity 🎉

**Solidity Version**: ^0.8.3
**IDE**: [Remix IDE](https://remix.ethereum.org/)

---
## 📜 Description
This is **my first smart contract** written in Solidity! 🥳  
It's simple, but it taught me the **basic fundamentals** of blockchain programming.
I have already **deployed it on the Sepolia testnet** using Remix.

**Contract address (Sepolia):**  
[0x1e0463625780139cB5e97C243cBd79Ce30482cE2](https://sepolia.etherscan.io/address/0x1e0463625780139cB5e97C243cBd79Ce30482cE2)

## What the contract does

- **Stores a favorite number** (`favoriteNumber`)  
- **Retrieves the stored number** using `retrieve()`  
- **Adds people with name and favorite number** via a dynamic `People` array  
- **Maps names to favorite numbers** using `nameToFavoriteNumber`  

## What I learned

### 1. Basic Solidity contract structure
- How to declare state variables (`uint256 favoriteNumber;`)  
- How to use **structs**, **dynamic arrays**, and **mappings**  

### 2. Read vs write functions
- Functions that **modify the blockchain** (like `store` and `addPerson`) consume **gas**  
- Functions marked as **view** or **pure** (like `retrieve`) do **not** consume gas  

### 3. Memory vs calldata vs storage
- **memory**: temporary data that can be modified inside functions  
- **calldata**: temporary but immutable data (more gas-efficient for parameters)  
- **storage**: permanent data stored on the blockchain  

### 4. How mappings work
- Creating `nameToFavoriteNumber` to quickly look up someone's favorite number without looping through an array  

### 5. Understanding Ethereum in practice
- Every **deployed contract** is public and immutable on the Ethereum network  
- Functions that change state must be sent as **transactions** (which require gas)  
- Functions that only read data are **free to call** (no gas cost)  
