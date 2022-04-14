# Blockchain_concepts
<details><summary>Prerequisite to Execute the code</summary>
<p>

## MetaMask (Creation of Ethereum Account)
1. Installation and creation of account, wallet named "x21145059-student-wallet" under Ropsten Test Network
2. Get enough Test Ethers from Ropsten test faucets
3. Update the wallet address in .env file "Owner_Address"

## Remix IDE
1. Create the Smart contract file named "ProjectERC20.sol". Modify name and symbol in ProjectERC20.sol file (Line 166)

  ```js
    constructor() {
        _name = "x21145059-Student";
        _symbol = "ETH";
        
        _mint(msg.sender, 1000000000000000000000000);
    }
  ```
2. Compile and Deploy the smart contract in Injected Web3 environment.
3. Update the contract address in .env file "Contract_Address"
  
## INFURA
1. Create an account, and new project in INFURA. Select product as Ethereum.
2. Update the Infura_Token in .env file taking Ropsten Endpoint address
</p>
</details>

<details><summary>Code Execution</summary>
<p>
  
 ## Steps followed in Visual Studio
 1. Open Node.js files in Visual Studio (Contract.js, Distribute.js, accounts.txt, .env, DeployedContract.sol).
  
 2. Install the Dependencies using Node package manager (nmp)

  `$npm i web3 fs big-number ethereumjs-tx dotenv`
  
 3. Create the package.json file using below command
  `$npm init`
 
 4. To execute the Javascript file using node.js execute the below command
 `node distribute.js`
 
 5. Distribute.js file will call the contract.js, .env files where we have all the details of token address, contract address, MetaMask private key value
 
 6. Tokens will be equally distributed among 10 accounts meintioned in account.txt
  
 7. We can verify the same flow of token in Etherscan 
 </p>
</details>

<details><summary>Code Execution using Docker</summary>
<p>
 ## Steps followed to deploy Docker
 1. Create Docker account and then download Docker app on the system.
  
 2. Run the below commands in Visual Studio inside the main folder 
 
 3. To create new Docker file which will be used to create an image and then the container run `touch Dockerfile`
  
 4. `docker build . -t shilpimadan27`
  
 5. From the Docker hub webpage create new public docker repository "x21145059-blockchain"
  
 6. Create Tag "shilpiproject", by using this tag we can add multiple images to the specific repository 
  
 7. To create a Docker image run command 
  `docker build . -t shilpimadan27/x21145059-blockchain:shilpiproject`
 
 8. To push the above created Docker container image in the Docker Hub using the tag run command
  `docker push shilpimadan27/x21145059-blockchain:shilpiproject`
  
 9. Go to the Docker hub page under the mentioned repository and tag we will get the pull command
  `docker pull shilpimadan27/x21145059-blockchain:shilpiproject`
  
 </p>
</details> 
  
