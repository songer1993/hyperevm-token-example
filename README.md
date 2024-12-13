# Hyperliquid EVM Token Example

A simple example demonstrating how to deploy and interact with ERC20 token contracts on the Hyperliquid EVM testnet.

## Prerequisites

- Python 3.8+
- Web3.py
- Access to Hyperliquid testnet
- Test ETH in your wallet

## Installation
1. Clone the repository:
```shell
git clone https://github.com/songer1993/hyperevm-token-example.git
cd hyperevm-token-example
```

2. Install dependencies:
```shell
pip install web3 python-dotenv eth-account
```

3. Create a `.env` file in the root directory:
```plaintext
DEPLOYER_PRIVATE_KEY='your_private_key_here'
```

## Contract Details

The project includes an ERC20 token contract (MyToken) with the following features:
- Initial supply of 1,000,000 MTK tokens
- Standard ERC20 functions:
  - `totalSupply()`: Returns the total token supply
  - `balanceOf(address)`: Returns the token balance of an address
  - `transfer(address, uint256)`: Transfers tokens to a specified address
  - Other standard ERC20 functions (approve, transferFrom, etc.)

## Usage

See `token-example.ipynb` for deployment and testing. The notebook includes:
- Contract deployment
- Checking total supply
- Checking account balances
- Transferring tokens between addresses

## Project Structure

```plaintext
├── bin/
│   ├── MyToken.abi        # Contract ABI
│   └── MyToken.bin        # Contract bytecode
├── MyToken.sol            # Solidity source code
├── token-example.ipynb    # Jupyter notebook for deployment and testing
├── README.md             # Project documentation
├── .env                  # Environment variables (not in git)
└── .gitignore           # Git ignore rules
```

## Security

- Never commit your private keys or `.env` file
- Use testnet for development
- Always review transactions before signing

## Network Details

- Network: Hyperliquid Testnet
- RPC URL: https://api.hyperliquid-testnet.xyz/evm

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Hyperliquid team for the testnet
- Web3.py documentation
- OpenZeppelin for ERC20 implementation
