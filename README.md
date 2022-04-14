# Blockchain_concepts
<details><summary>Prerequisite to Execute the code</summary>
<p>

## MetaMask (Creation of Ethereum Account)
1. Installation and creation of account, wallet named "x21145059-student-wallet" under Ropsten Test Network
2. Get enough Test Ethers from Ropsten test faucets
3. Update the wallet address in .env file "Owner_Address"

## Remix IDE
1. Create the Smart contract file named "ProjectERC20.sol". Modify name and symbol in ProjectERC20.sol file (Line 166)
  js
    constructor() {
        _name = "x21145059-Student";
        _symbol = "ETH";
        
        _mint(msg.sender, 1000000000000000000000000);
    }
2. Compile and Deploy the smart contract in Injected Web3 environment.
3. Update the contract address in .env file "Contract_Address"
  
## INFURA
1. Create an account, and new project in INFURA. Select product as Ethereum.
2. Update the Infura_Token in .env file taking Ropsten Endpoint address
</p>
</details>

<details><summary>Code Execution</summary>
<p>
 1. Open Node.js files in Visual Studio (Contract.js, Distribute.js, accounts.txt, .env, DeployedContract.sol).
 2. 
 </p>
</details>
