# Practice2
This repository contains a TON smart contract implemented in FunC. The contract provides several methods for interaction and management.

To ensure the contract's functionality and reliability, a suite of tests has been written and is included in "tests/Main.spec.ts".

*.ts files in scripts folder for interacting with the contract on the TON testnet are also included.
## Contract Methods
The smart contract implements five primary methods that interact with `recv_internal()`:

1. Update Smart Contract Code: This method allows for the updating of the smart contract's code.

2. Transfer Messages to Owner: This method enables the transfer of messages to the owner of the smart contract.

3. Deposit (Simple Send): This method allows for the deposit of funds into the smart contract.

4. Owner Withdraw: This method enables the owner of the smart contract to withdraw funds.

5. Change Owner: This method allows for the transfer of ownership of the smart contract.

## Self-Destruction of the Contract
The `recv_external()` method is used to self-destruct the contract:

1. Selfdestruct (Burn Smart Contract): This method destroys the smart contract and burns the associated funds.
Please note that this smart contract should be used responsibly. Always ensure that you have a backup of the necessary data before initiating the self-destruction of the contract.

## Testing
The **Main.spec.ts** file contains a suite of tests that verify the functionality of the smart contract. These tests cover all the main methods and check for correct behavior in a variety of scenarios. To run the tests, use the following command

```
npx blueprint test
```
## Interacting with the Contract on TON Testnet
Scripts for interacting with the contract on the TON testnet are included in the scripts/ directory. These scripts demonstrate how to perform the following operations:

1. Deposit: This script shows how to deposit funds into the smart contract.

2. Withdraw: This script shows how to withdraw funds from the smart contract.

3. Send Message to Owner: This script shows how to send a message to the owner of the smart contract.

To run the scripts, use the following command
```
yarn blueprint run
```
## Project structure

-   `contracts` - source code of all the smart contracts of the project and their dependencies.
-   `wrappers` - wrapper classes (implementing `Contract` from ton-core) for the contracts, including any [de]serialization primitives and compilation functions.
-   `tests` - tests for the contracts.
-   `scripts` - scripts used by the project, mainly the deployment scripts.

## How to use

### Requirements
- Node.js with a recent version like v18, verify version with node -v
- IDE with TypeScript and FunC support like Visual Studio Code with the FunC plugin
- Ton Keeper (Ton Wallet)

### Install
```
npm create ton@latest 
npm install
npx blueprint test
```
### Build

`npx blueprint build` or `yarn blueprint build`

### Test

`npx blueprint test` or `yarn blueprint test`

### Deploy or run another script

`npx blueprint run` or `yarn blueprint run`

### Add a new contract

`npx blueprint create ContractName` or `yarn blueprint create ContractName`

# License
MIT
# FunC_Practice2
