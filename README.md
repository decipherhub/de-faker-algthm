# de-faker-algthm
Purpose: Planning for the algorithm of detecting self-trading

***

## Scenario #1
An abuser generates fake transactions through numerous wallets to avoid fake detection. Especially, creating new wallet does not take any cost in Ethereum, so cost-free abusing is available.

### Detection 1. Number of interacting contracts from a wallet
For every wallet, count the number of contract which interact with the wallet. If the number approaches 1, acknowledge as a fake tx.
* Requirement:
  - list of active wallets
  - list of interacted contract for active wallets
* Output:
  - Average number of interacting contract
  - list of fake wallets

***

## Scenario #2
An abuser owning a specific group of wallets utilizes those wallets to generate fake transactions. If the number of wallet is limited due to the wallet creating cost or technical reason, then this scenario might work.

### Detection 1. Closed token flow

***

## 2. Repeated transaction pattern

***

## 3. 





## 4. Liquid token cap
