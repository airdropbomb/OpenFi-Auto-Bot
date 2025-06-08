# OpenFi Auto Bot

A sophisticated automation bot for interacting with the OpenFi testnet protocol, designed to perform various DeFi operations including supplying assets, borrowing tokens, and claiming faucet tokens.

## Features

- � **Multi-Wallet Support**: Process multiple wallets simultaneously
- 🛡 **Proxy Integration**: Supports HTTP/HTTPS/SOCKS proxies for anonymity
- 💰 **PHRS Operations**: Deposit and manage PHRS tokens
- 🚰 **Faucet Minting**: Mint testnet tokens from the faucet
- 🔄 **Token Management**: Supply, borrow, and withdraw various ERC20 tokens
- ⚙️ **Configurable**: Customize transaction counts and amounts

## Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- Private keys for wallets you want to use
- (Optional) Proxy list for anonymity

## Installation

1. Clone the repository:
```bash
git clone https://github.com/vikitoshi/OpenFi-Auto-Bot.git
cd OpenFi-Auto-Bot
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the project root and add your private keys:
```env
PRIVATE_KEY_1=your_private_key_here
PRIVATE_KEY_2=your_second_private_key_here
# Add as many keys as needed
```

4. (Optional) Add proxies to `proxies.txt` (one per line):
```text
http://user:pass@proxyip:port
socks5://user:pass@proxyip:port
```

## Usage

Run the bot:
```bash
node index.js
```

The bot will present a menu with the following options:

1. **Supply PHRS** - Deposit PHRS tokens to the lending pool
2. **Mint Faucet Tokens** - Claim testnet tokens from the faucet
3. **Supply ERC20 Tokens** - Deposit supported ERC20 tokens
4. **Borrow Tokens** - Borrow assets from the lending pool
5. **Withdraw Tokens** - Withdraw supplied tokens
6. **Exit** - Quit the bot

Follow the on-screen prompts to configure each operation.

## Supported Tokens

The bot supports the following testnet tokens:

1. NVIDIA
2. USDT
3. USDC
4. GOLD
5. TSLA
6. BTC

## Configuration

You can modify the following constants in the code:

- `NETWORK_CONFIG`: RPC URL, chain ID, and explorer
- `CONTRACTS`: Contract addresses for the protocol
- Transaction delays and gas limits

## Security Notes

⚠️ **Important Security Considerations**:
- Never share your private keys
- This is for testnet use only
- The bot comes with no warranties
- Use at your own risk

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)
