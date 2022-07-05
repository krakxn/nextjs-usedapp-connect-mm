# nextjs-useDapp-metamask-connect

This is a minimalistic project to show us how we can connect to metamask using [useDapp](https://usedapp.io/) in nextjs / react.

This could just as easily be done in typescript.

This project started with nexjs boilerplate by running `yarn create next-app nextjs-useDapp-metamask-connect`

Video Coming soon...

- [nextjs-useDapp-metamask-connect](#nextjs-usedapp-metamask-connect)
- [Getting Started](#getting-started)
  - [Requirements](#requirements)
  - [Quickstart](#quickstart)
    - [Important localhost note](#important-localhost-note)
- [Full Examples](#full-examples)
- [Thank you!](#thank-you)

Video coming soon...

# Getting Started

## Requirements

- [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
  - You'll know you did it right if you can run `git --version` and you see a response like `git version x.x.x`
- [Nodejs & npm](https://nodejs.org/en/)
  - You'll know you've installed nodejs right if you can run:
    - `node --version` And get an ouput like: `vx.x.x`
  - You'll know you've installed npx right if you can run:
    - `npm --version` And get an ouput like: `x.x.x`
- [Yarn](https://classic.yarnpkg.com/lang/en/docs/install/) instead of `npm`
  - You'll know you've installed yarn right if you can run:
    - `yarn --version` And get an output like: `x.x.x`
    - You might need to install it with npm
- [Metamask](https://metamask.io/)
  - This is a browser extension that lets you interact with the blockchain.
- A Testnet Kovan project [Alchemy URL](https://alchemy.com/?a=673c802981)

## Quickstart

1. Clone and install dependencies

```
git clone https://github.com/PatrickAlphaC/nextjs-ethers-metamask-connect
cd nextjs-ethers-metamask-connect
yarn
```

2. Then, you'll need to open up a second terminal and run:

```
git clone https://github.com/PatrickAlphaC/hardhat-simple-storage
cd hardhat-simple-storage
yarn hardhat node
```

This will deploy a sample contract and start a local hardhat blockchain.

3. Connect your [metamask](https://metamask.io/) to your local hardhat blockchain.

> **PLEASE USE A METAMASK ACCOUNT THAT ISNT ASSOCIATED WITH ANY REAL MONEY.**
> I usually use a few different browser profiles to separate my metamasks easily.

In the output of the above command, take one of the private key accounts and [import it into your metamask.](https://metamask.zendesk.com/hc/en-us/articles/360015489331-How-to-import-an-Account)

Additionally, add your localhost with chainid 31337 to your metamask.

4. Open the UI

Then, back in your first terminal, run:

```
yarn dev
```

5. Hit buttons

You'll be brought to the UI after running `yarn dev` which has exactly 2 buttons. Hit `connect`, metamask, then hit `execute`.

First, you deploy a multicall contract, and then and you'll send a transaction to your local hardhat.

### Important localhost note

If you use metamask with a local network, everytime you shut down your node, you'll need to reset your account. Settings -> Advanced -> Reset account. Don't do this with a metamask you have real funds in.

# Full Examples

- [defi-stake-yield-brownie](https://github.com/PatrickAlphaC/defi-stake-yield-brownie)

# Thank you!