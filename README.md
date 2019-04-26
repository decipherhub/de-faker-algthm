# de-faker-algthm
Purpose: Planning for the algorithm of detecting self-trading

1. closed token flow

2. repeated transaction pattern

3. wallets for single contract
For every wallets, count the number of contract which interact with the wallet
If the number approaches 1, acknowledge as a fake tx
* Requirement:
 * list of active wallets
 * list of interacted contract for active wallets
* Output:
 - list of fake wallets

4. liquid token cap
