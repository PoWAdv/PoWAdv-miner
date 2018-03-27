
# PoWAdv ERC20 Token Miner

Solves proof of work to mine supported ERC20 tokens.  


### Update 1.5.23 - 1000X CPU Pool Mining

This new build uses the C++ addon to accelerate the CPU mining one-thousand fold.  

### Building from Source

#### Setup (Windows/Linux)
1. Install NodeJS 8.9
2. Run 'npm install yarn -g' to install yarn package manager
3. Clone/download the project
4. Open a terminal, cd into the project folder and run 'yarn' to install dependencies
5. Run the command 'npm run build' to build C files with node-gyp
6. Start the miner with 'node index.js'

#### Setup (Mac)
1. Install Homebrew & NodeJS 8.9
2. Run 'brew install yarn' to install yarn package manager
3. Clone/download this project
4. Open a terminal, cd into the project folder and run 'yarn'
5. Run the command 'npm run build' to build C files with node-gyp
6. Start the miner with 'node index.js'



### Commands

      {commands}
      "help" - Show the help menu

      "account new" - Create a new mining account
      "account list" - List all mining accounts
      "account select 0x####" - Select a primary mining account by address
      "account balance" - List the ether and token balance of your selected account

      "contract list" - List the selected token contract to mine
      "contract select 0x####" - Select a PoW token contract to mine

      "config gasprice #" - Set the gasprice used to submit PoW to the token smartcontract
      "config cpu_threads #" - Set the number of CPU cores to use for mining
      "config web3provider http://----:####" - Set the web3 provider url for submitting ethereum transactions

      "pool mine" - Begin mining into a pool
      "pool list" - List the selected mining pool
      "pool select http://####.com:####" - Select a pool to mine into

      "mine" - Begin mining solo, directly into the smartcontract




---------------

### Getting Started
1. Build a new mining account with 'account new'
2. View the private key with 'account list'
3. Write down these credentials
4. Mine POWA tokens with the command 'mine'


### Vault Datafiles

(requires 'show hidden files and folders')

Stored at:

- Windows
    '/Users/{user}/Appdata/Roaming/.PoWAdv'

- Mac
    '/home/{user}/Library/Preferences/.PoWAdv'

- Linux
    '/home/{user}/.PoWAdv'




### Testing

npm run test


## Credits (Original developer)

1. Zegordo (Developed the accelerated CPU Miner)

        ETH address [0x8AE981d92875C88f713600EB7dC4D23FA7E0E621]



## Tokens that can be mined using Proof of Work:

1. POWA token - http://powadv.org - https://etherscan.io/address/0x1a136ae98b49b92841562b6574d1f3f5b0044e4c
