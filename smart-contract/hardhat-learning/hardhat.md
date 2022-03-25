# Hardhat start-guide
## Installation
[hardhat installation tutorial](https://hardhat.org/getting-started/#installation)

Steps:
1. make a new folder, into it and run  `npm init -y`
2. intall the hardhat package `npm install --save-dev hardhat`
3. Create hardhat project `npx hardhat `, I choose the one with keywords "typescript"

## Use Truffle dashboard to interaction 
- Open another terminal inside the project run `truffle dashboard` 
- Then in another terminal, 
    - either diretly run in terminal `npx hardhat run ./scripts/deploy.ts --network truffle`'
    - or in the `package.json`, in the `scripts` section, add ` "deploy": "hardhat run ./scripts/deploy.ts --network truffle"`. Then run `yarn deploy`
    - [NOTE how `dotenv` works with `process.env.{ENVRAIBLES}`](https://dev.to/francis04j/how-to-add-env-and-use-process-env-to-your-typescript-project-3d6b),this author also proposed it's better to use `endpoints.config.ts` as more fexible and easy-to-test method
    - [`hardhat.config.ts` example](https://github.com/paulrberg/solidity-template/blob/main/hardhat.config.ts) 
    