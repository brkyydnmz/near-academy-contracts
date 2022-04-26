# The Meme Museum

This repo is deprecated. Please use: https://github.com/NEAR-Edu/near-academy-contracts

1. Prepare your account. You need to make sure your NEAR CLI has access to the account supposed to interact with the contract. Simply use the NEAR CLI and type near login and follow the instructions.

2. Register yourself as a contributor to the museum contract. Make sure to use the accountId that you used when you called near login:

## Terminal steps
1. near call museum.testnet add_myself_as_contributor --accountId YOUR_ACCOUNT_NAME.testnet
2. near call museum.testnet add_meme '{"meme" : "doges", "title" : "again", "data" : "https://9gag.com/gag/ajgKdqg", "category" : 4}' --accountId YOUR_ACCOUNT_NAME.testnet --amount 3 --gas=75000000000000

 Once the meme contract is deployed, you can verify that it was created by returning the list of all available memes: near view museum.testnet get_meme_list. You may now also find it on the blockchain explorer, it is in the public domain now.

 On BlockChain: https://explorer.testnet.near.org/transactions/BaLLyjdoosHzjeZ3mj63ABEd7PSE15ynaqGe6w5vCygg
