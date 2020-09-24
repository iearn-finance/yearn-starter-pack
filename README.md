# yearn-starter-pack

### What you'll find here

Solidity Smart Contracts for DAI Curve Strategy plus it's Controller and yVault.

Interfaces for some of the most used DeFi protocols on ethereum mainnet.

Sample test suite that runs on mainnet fork.


### How does it work for the User

Let's say Alice holds 100 DAI and wants to start earning yield % on them.

For this Alice needs to `DAI.approve(yVault.address, 100)`.

Then Alice will call `yVault.deposit(100)`.

yVault will then transfer 100 DAI from Alice to itself, and mint Alice the corresponding shares.

Alice can then redeem those shares using `yVault.withdrawAll()` for the corresponding DAI balance.


### How does it work for the Vault

TODO

### Requirements

- [Install Brownie](https://eth-brownie.readthedocs.io/en/stable/install.html)

- Install Dev dependencies: `pip3 install -r requirements-dev.txt`
    - Use whatever pip version avaiable

- Install ganache-cli: `npm install -g ganache-cli@6.10.1`

- Copy `.envrc.example` to `.envrc`

- Setup `ETHERSCAN_TOKEN` & `WEB3_INFURA_PROJECT_ID`

### Tests

- Run tests with: `npm test`

