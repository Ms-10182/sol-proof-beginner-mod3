# Candy Machine + UI
This is a fullstack code for minting fo SPL tokens and used them to buy NFT using candy machinge.
## Working
First the SPL tokens were minted by entering the private key string into ```getTokens.js``` file and then from solana explorer ```spltoken``` address and ```spltokenAccount``` address was copied and pasted into the ```config.json```. Then the candy machine was deployed. After deployment its machine id was used in ```.env``` file and in ```package.json```, dependency was updated. After this using ```yarn start``` front end was started and its live!!.
## Steps for project
1)  Follow these commands:
  ```javascript
solana-keygen new --outfile ./wallet.json
 solana config set --keypair ./wallet.json
solana config set --url https://api.devnet.solana.com
solana airdrop 1
```
2) paste your private key in ```getTokens.js``` and mint 20 SPL. and then send some SPL to other account purpose.
3) From solana explorer copy and paste the ```splToken``` and ```splTokenAccount``` into ```config.js```
4) Follow there commands:
        ```sugar validate```
        ```sugar upload```
        ```sugar deploy```
        ```sugar verify```
5) Now ```git clone https://github.com/metaplex-foundation/candy-machine-ui ./candy-machine-ui/
cd candy-machine-ui```
6) copy paste these into .env.example
```javascript
REACT_APP_CANDY_MACHINE_ID=<your machine id>
REACT_APP_SOLANA_NETWORK=devnet
REACT_APP_SOLANA_RPC_HOST=https://api.devnet.solana.com
SKIP_PREFLIGHT_CHECK=true
```
run these commands : 
```javascript
yarn install
yarn start
```
7)  now open the url and connect the wallet which have the spl tokens.
8)  click mint and sign the transaction , SPL will be deducted and NFT will be minted to the wallet.

   
   
