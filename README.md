# Solana NFT Staking

## Overview

This project is a Solana-based staking management system for NFTs, pNFTs (programmable NFTs), and cNFTs (compressed NFTs). Users can stake their NFTs to earn rewards, track staking progress, and manage their assets within the ecosystem.

## Features

- **Stake & Unstake NFTs**: Users can stake and unstake their NFTs seamlessly.
- **Support for pNFTs & cNFTs**: The staking protocol supports Solana's compressed and programmable NFTs.
- **Reward Distribution**: Users earn staking rewards based on predefined logic.
- **Claim Rewards**: Stakeholders can claim rewards in SPL tokens.
- **Admin Controls**: A dedicated admin interface to configure staking parameters.
- **Solana Smart Contract (Anchor Framework)**: The program is developed using the Anchor framework for security and reliability.

## Technologies Used

- **Solana Blockchain**
- **Rust (Anchor Framework)** for smart contract development
- **TypeScript & React** for frontend interface
- **Metaplex** for NFT handling
- **SPL Tokens** for rewards distribution

## Installation & Setup

### Prerequisites

Ensure you have the following installed:

- [Solana CLI](https://docs.solana.com/cli/install-solana)
- [Anchor CLI](https://book.anchor-lang.com/chapter_2/installation.html)
- [Node.js](https://nodejs.org/en/download/)
- Yarn or npm

### Clone the Repository

```sh
git clone https://github.com/muffin819/solana-NFT-staking.git
cd solana-NFT-staking
```

### Install Dependencies

```sh
yarn install  # or npm install
```

### Build & Deploy Smart Contract

```sh
anchor build
anchor deploy
```

### Configure Environment Variables

Create a `.env` file in the root directory and add the necessary configurations:

```
RPC_URL=https://api.mainnet-beta.solana.com
WALLET_KEYPAIR=./keypair.json
PROGRAM_ID=YOUR_DEPLOYED_PROGRAM_ID
```

### Run the Frontend

```sh
yarn dev  # or npm run dev
```

## Smart Contract Overview

The smart contract consists of the following core functions:

- `initialize_pool`: Initializes the staking pool.
- `stake_nft`: Allows users to stake their NFTs.
- `unstake_nft`: Enables users to unstake their NFTs.
- `claim_rewards`: Lets users claim staking rewards.
- `update_pool`: Admin function to update staking parameters.

## API Endpoints

If using a backend service, here are some example API endpoints:

- `POST /stake` - Stake an NFT.
- `POST /unstake` - Unstake an NFT.
- `GET /rewards` - Fetch reward details.
- `POST /claim` - Claim staking rewards.

## Future Enhancements

- Integration with Solana Pay for reward redemptions.
- Multi-chain NFT staking support.
- UI improvements with additional analytics.

## Contributing

Pull requests are welcome! Feel free to fork the repo and create a PR with your changes.

## License

This project is licensed under the MIT License.

