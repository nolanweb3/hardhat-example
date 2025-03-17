# Example React Typescript Ethers.js Hardhat Project

This repo contains a Hardhat and React Dapp starter project. The React Dapp in the `frontend` dir of this repo interacts with Hardhat's example `Greeter.sol` smart contract running on a local blockchain. The Hardhat `Greeter.sol` example contract is the boilerplate contract that Hardhat creates when creating a new Hardhat project via `yarn hardhat init`.

The React Dapp in this repo looks like this:

![React Dapp](https://res.cloudinary.com/divzjiip8/image/upload/c_scale,w_1280/v1641785505/Screen_Shot_2022-01-03_at_3.52.58_PM_n7ror7.png)

The Dapp uses the [@web3-react npm package's](https://www.npmjs.com/package/web3-react) injected web3 provider to connect to MetaMask and demonstrates the following functionality:
* Connecting a Dapp to the blockchain
* Reading account data from the blockchain
* Cryptographically signing digital messages
* Deploying new instances of a smart contract
* Reading and writing data to and from the deployed smart contract

This repo can be useful to anyone looking to get a local Ethereum blockchain running and to get a Dapp up and communicating with the local node quickly.

Additionally, this repo is a companion project to [ChainShot](https://www.chainshot.com)'s [How to Build a React Dapp with Hardhat and MetaMask](https://medium.com/p/9cec8f6410d3) Medium article. The article and this GitHub repo are recommended for anyone wanting to build up their web3 skills and are helpful resources for anyone interested in joining any of [ChainShot's bootcamps](https://www.chainshot.com/bootcamp).

The smart contract and Hardhat node part of this project were created by installing the [Hardhat npm package](https://www.npmjs.com/package/hardhat) and bootstrapping a Hardhat project by running: `yarn hardhat init`.

Pull this project down from GitHub, cd into the project directory and run the following commands to get setup and running.

```shell
yarn
yarn compile
yarn hardhat node
```

The commands above will install the project dependencies, compile the sample contract and run a local Hardhat node on port `8545`, using chain id `31337`.

After running the above tasks, Use:

    cd to the frontend directory of this project
    Run yarn to install the necessary dependencies
    yarn start to startup the webserver
    Visit localhost:3000 in your browser to interact with the browser Dapp and the Greeter contract running on your local Hardhat blockchain.

to run a React Dapp using ethers.js that will interact with the sample contract on the local Hardhat node.

Some other hardhat tasks to try out are:

```shell
yarn hardhat accounts
yarn hardhat clean
yarn hardhat compile
yarn hardhat deploy
yarn hardhat help
yarn hardhat node
yarn hardhat test
```


