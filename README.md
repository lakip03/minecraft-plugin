# SolCraft Plugin

**A Minecraft plugin that bridges the blockchain world with Minecraft gameplay**

![Version](https://img.shields.io/badge/version-1.0--SNAPSHOT-blue)
![API](https://img.shields.io/badge/Minecraft%20API-1.21-green)
![License](https://img.shields.io/badge/license-MIT-yellow)

## Project Overview

SolCraft Plugin integrates Solana blockchain functionality directly into Minecraft, allowing players to link wallets, trade in-game diamonds for blockchain tokens, and check token balances — all without leaving the game.

This project demonstrates practical blockchain integration in gaming environments and showcases modern Kotlin development techniques including asynchronous processing, clean architecture, and GraphQL API communication.

## Features

- **Wallet Management**: Players can link and unlink Solana wallets to their Minecraft accounts
- **Token System**: Trade in-game diamonds for blockchain tokens
- **Balance Checking**: View token balances from within Minecraft
- **Secure Communication**: Asynchronous GraphQL API communication
- **User-Friendly Commands**: Simple commands for all blockchain interactions

## Technologies & Skills

- **Kotlin**: Modern, concise JVM language with robust null safety
- **Bukkit/Spigot API**: Minecraft server plugin development
- **GraphQL**: Data query and manipulation language for APIs
- **Asynchronous Programming**: Non-blocking I/O operations
- **JSON Processing**: Handling API responses and data extraction
- **Clean Architecture**: Separation of concerns and modular design

## Command Usage

| Command | Description | Usage |
|---------|-------------|-------|
| `/setwallet <address>` | Link a Solana wallet to your Minecraft account | `/setwallet Ht7CKBdkbsFk2hrnvhyqaRZx3Bb6N41XKE9NWT7yDfm7` |
| `/mywallet` | View your currently linked wallet address | `/mywallet` |
| `/unlinkwallet` | Remove the link between your wallet and Minecraft account | `/unlinkwallet` |
| `/balance` | Check your token balance | `/balance` |
| `/soltrade <amount>` | Exchange diamonds for tokens | `/soltrade 5` |
| `/howmany` | Count diamonds in your inventory | `/howmany` |

## Technical Implementation

### Architecture Highlights

- **Service-Oriented Design**: Modular components with clear responsibilities
- **Async Request Handling**: Non-blocking HTTP requests keep the server responsive
- **Error Handling**: Robust exception management and user feedback
- **Regex Processing**: Efficient extraction of data from API responses
- **Transaction Security**: Safe handling of in-game transactions with rollback capability

### Key Components

- **GraphQLService**: Core communication layer for API interactions
- **Command Handlers**: Individual executors for each blockchain-related command
- **Transaction Processing**: Safe exchange of in-game items for blockchain tokens
- **Response Parsing**: Efficient extraction of critical data from API responses

## Development Focus

- **User Experience**: Clear feedback messages and intuitive commands
- **Performance**: Async operations to prevent server lag during blockchain operations
- **Error Resilience**: Comprehensive error handling and fallback mechanisms
- **Security**: Safe transaction processing with verification steps

## Future Possibilities

- Enhanced token usage within gameplay
- NFT integration for unique in-game items
- Marketplace functionality for player-to-player trading
- Economic gameplay mechanics leveraging blockchain

## Installation & Setup

1. Place the plugin JAR in your server's `plugins` folder
2. Configure backend GraphQL endpoint in the config file
3. Restart your server
4. Players can now use commands to interact with the blockchain

## Requirements

- Minecraft server running version 1.21 or later
- Access to a compatible GraphQL backend service
- Java 17 or higher

---

This project demonstrates practical blockchain integration, modern Kotlin development, and scalable plugin architecture for Minecraft—showcasing both technical excellence and innovative gameplay possibilities.
