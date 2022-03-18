# Udacity Capstone

## Install

Compatible with:

* Truffle v5.3.7 (core: 5.3.7)
* Solidity v0.8.5 (solc-js)
* OpenZeppelin v4.1.0 (solidity: 0.8.0)
* Node v16.2.0
* Web3.js v1.3.6
* Ganache CLI v6.12.2 (ganache-core: 2.13.2)
* Zokrates v0.7.3

Run:

`npm install`

`truffle compile`

## Develop Back-End

### Testing

Start local ethereum blockchain:

`ganache-cli`

To run all tests:

`npm test` or `truffle test`

To run a single test:

- `truffle test ./test/TestSolnSquareVerifier.js`
- `truffle test ./test/TestERC721Mintable.js`
- `truffle test ./test/TestSquareVerifier.js`

### Deployment on Rinkeby

Create in root folder `.rinkeby-infurakey` and `.secret` and run:

`truffle migrate --network rinkeby`

### Deployment info (required for project submission)

- My Rinkeby accounts:
    - contract owner & token seller:
      [0x637E7075fc1B2D30d23D9Da79581eBE8Df531c89](https://rinkeby.etherscan.io/address/0x637E7075fc1B2D30d23D9Da79581eBE8Df531c89)
    - token buyer:
      [0xeEFC23Bd910bb99bEBa0dAe9dA67CB5ED6eDe54d](https://rinkeby.etherscan.io/address/0xeEFC23Bd910bb99bEBa0dAe9dA67CB5ED6eDe54d)
- Contract SquareVerifier v4:
    - address:
      [0x7c3f2fEe85378bE7bA697505440B43b9BC6fA2c1](https://rinkeby.etherscan.io/address/0x7c3f2fEe85378bE7bA697505440B43b9BC6fA2c1)
- Contract SolnSquareVerifier v4:
    - address:
      [0xFf21fb7154c2286Fe6F9156A768EB7d6d9ABb5dF](https://rinkeby.etherscan.io/address/0xFf21fb7154c2286Fe6F9156A768EB7d6d9ABb5dF)
    - [event's history](https://rinkeby.etherscan.io/address/0xFf21fb7154c2286Fe6F9156A768EB7d6d9ABb5dF#events)
    - [abi](pareot-contract-abi.json)
    - [deployment log](res/rinkeby-deployment-log.md)

## Develop Front-End

### Token Minting

- Start Brave browser
- Log-in to your [my ether wallet - MEW CX](https://www.myetherwallet.com)
- Change network to Rinkeby Testnet
- Select the contract owner account
- Navigate to [interace with contract](https://www.myetherwallet.com/interface/interact-with-contract)
- Connect to SolnSquareVerifier address and use [this contract abi](pareot-contract-abi.json)
- Mint some tokens

### Front store & minted NFT listed on Open Sea (required for project submission)

Visit the [Front Store](https://testnets.opensea.io/assets/unidentified-contract-2m8wyj1rug) ...

... or select directly one of the tokens:

- [token-0](https://testnets.opensea.io/assets/0xFf21fb7154c2286Fe6F9156A768EB7d6d9ABb5dF/0)
- [token-1](https://testnets.opensea.io/assets/0xFf21fb7154c2286Fe6F9156A768EB7d6d9ABb5dF/1)
- [token-2](https://testnets.opensea.io/assets/0xFf21fb7154c2286Fe6F9156A768EB7d6d9ABb5dF/2)
- [token-3](https://testnets.opensea.io/assets/0xFf21fb7154c2286Fe6F9156A768EB7d6d9ABb5dF/3)
- [token-4](https://testnets.opensea.io/assets/0xFf21fb7154c2286Fe6F9156A768EB7d6d9ABb5dF/4)
- [token-5](https://testnets.opensea.io/assets/0xFf21fb7154c2286Fe6F9156A768EB7d6d9ABb5dF/5)
- [token-6](https://testnets.opensea.io/assets/0xFf21fb7154c2286Fe6F9156A768EB7d6d9ABb5dF/6)
- [token-7](https://testnets.opensea.io/assets/0xFf21fb7154c2286Fe6F9156A768EB7d6d9ABb5dF/7)
- [token-8](https://testnets.opensea.io/assets/0xFf21fb7154c2286Fe6F9156A768EB7d6d9ABb5dF/8)
- [token-9](https://testnets.opensea.io/assets/0xFf21fb7154c2286Fe6F9156A768EB7d6d9ABb5dF/9)



- Copy 'zokrates/verifier.sol' to 'contracts/SquareVerifier.sol' and upgrade its version to 0.8.5
- Import ISquareVerifier.sol and make sure SquareVerifier implements it
- Copy 'proof/proof-token0.json' as 'proof/proof-token0-fake1.json' and change the inputs to generate fake proof which
  is not causing exception
- Copy 'proof/proof-token0.json' as 'proof/proof-token0-fake2.json' and change the proof parameters to generate fake
  proof which is causing exception

# Project Resources

* [Remix - Solidity IDE](https://remix.ethereum.org/)
* [Truffle Framework](https://truffleframework.com/)
* [Ganache - One Click Blockchain](https://truffleframework.com/ganache)
* [Open Zeppelin ](https://openzeppelin.org/)
* [Interactive zero knowledge 3-colorability demonstration](http://web.mit.edu/~ezyang/Public/graph/svg.html)
* [Docker](https://docs.docker.com/install/)
* [ZoKrates](https://zokrates.github.io/gettingstarted.html)
* [OpenSea](https://opensea.io/)
* [OpenSea DevDoc](https://docs.opensea.io/docs/3-viewing-your-items-on-opensea)
