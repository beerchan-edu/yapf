# Yet another pump.fun

(solely for the educational purposes)

# Local development
In a separate terminal start `solana-test-validator` and run tests via `anchor test --skip-local-validator`
+ locally update config via `solana config set -ul`

# Solana bootcamp
[videos](https://www.youtube.com/watch?v=amAq-WHAFs8)

First checkbox is for Nikita, second checkbox is for Yana.
+ [ ] [ ] Project 1 - Building a Favorites Program
+ [ ] [ ] Project 2 - Creating a Voting Application
+ [ ] [ ] Project 3 - Integrating Blinks and Actions
+ [ ] [ ] Project 4 - Building a CRUD Application
+ [X] [ ] Project 5 - Creating a Token
+ [ ] [ ] Project 6 - Creating a NFT
+ [X] [ ] Project 7 - Building a Swap Program
+ [ ] [ ] Project 8 - Creating a Token Vesting App
+ [ ] [ ] Project 9 - Building a Token Lottery
+ [ ] [ ] Project 10 - Lending Application
+ [ ] [ ] Project 11 - Programmable Money
+ [ ] [ ] Project 12 - Attacking the Bank
+ [ ] [ ] Project 13 - Getting to Production
+ [ ] Go Build Your Application!

# Tokens
As starting point, we use two tokens `Pupa` & `Lupa`. Their keys are saved in `keys/` folder (for security reason excluded from .git). We can update :
1. `solana config set --keypair ~/Workspace/yapf/keys/PupfM2bSZmfZyVtMJ5979hkkT1JVhiNcCNsgZdSD8V2.json`.
2. `solana config set --keypair ~/Workspace/yapf/keys/LupbwHA7axsmcf5trsr84f1jtnwnnzFsm4hFEBKkUKe.json`

Mint addresses of those tokens are `mPu9y8vEpAgfENx9AzDkS6A6SsGExCptdVJkUWx3u8V` & `mLuhk9zLeeECSwY2in1B75gxXZG4PfWDQzSMgY5Njnv`.
[devnet link Pupa](https://explorer.solana.com/address/mPu9y8vEpAgfENx9AzDkS6A6SsGExCptdVJkUWx3u8V?cluster=devnet) & [devnet link Lupa](https://explorer.solana.com/address/mLuhk9zLeeECSwY2in1B75gxXZG4PfWDQzSMgY5Njnv?cluster=devnet)

How to mint as authority?
1. create associated PDA `spl-token create-account mPu9y8vEpAgfENx9AzDkS6A6SsGExCptdVJkUWx3u8V`
2. mint tokens to this new associated account `spl-token mint mPu9y8vEpAgfENx9AzDkS6A6SsGExCptdVJkUWx3u8V 100`