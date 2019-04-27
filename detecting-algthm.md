# de-faker-algthm
Purpose: Planning for the algorithm of detecting self-trading


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

## Scenario #2
An abuser owning a specific group of wallets utilizes those wallets to generate fake transactions. If the number of wallet is limited due to the wallet creating cost or technical reason, then this scenario might work.

### Detection 1. Closed token flow
If we succeed in finding the token flow in a closed group of wallets, then it can be verified as a group fake transaction.
* Requirement:
  - list of transactions of active wallets and interacting wallets
  - Closed group detecting algorithm
* Output:
  - list of fake wallets in the closed group

## Scenario #3
An abuser might use a same method repeatedly to generate fake transactions.

### Detection 1. Repeated transaction pattern
If we can find any correlations between transactions, then those transactions could be regarded a fake.
* Requirement:
  - list of transactions from the contract
  - Pattern recognition algorithm (hopefully machine learning based?)
* Output:
  - Repeated pattern and the fake tx generating scheme
  - list of fake transactions

## Scenario #4

### Detection 1. Liquid token cap
