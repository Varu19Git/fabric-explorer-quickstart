# Development Guide

This document explains how to work with this repository.

## Repository Structure

This is a simple Git repository with:
- One working branch: `master`
- One remote: `origin` pointing to https://github.com/Varu19Git/fabric-explorer-quickstart.git

## Development Workflow

1. **Make changes to files** in the `/home/tuf/explorer-repo` directory

2. **Stage your changes**:
   ```bash
   git add .
   ```

3. **Commit your changes**:
   ```bash
   git commit -m "Description of your changes"
   ```

4. **Push to GitHub**:
   ```bash
   git push
   ```

## Directory Structure

```
fabric-explorer-quickstart/
├── config/                       # Explorer configuration files
│   ├── config.json               # Main Explorer config
│   └── connection-profile/       # Network connection profiles
│       └── test-network.json     # Connection profile for test network
├── docker-compose.yaml           # Docker services configuration
├── scripts/                      # Management scripts
│   ├── install.sh                # For installation
│   ├── start.sh                  # For starting the network
│   ├── stop.sh                   # For stopping the network
│   └── cleanup.sh                # For cleaning up resources
└── README.md                     # User documentation
```

## Important Files

- `docker-compose.yaml`: Defines the services (orderer, peers, Explorer)
- `scripts/install.sh`: Sets up the environment
- `scripts/start.sh`: Starts the network and Explorer
- `config/connection-profile/test-network.json`: Connects Explorer to the network

## GitHub Repository

Your GitHub repository is at: https://github.com/Varu19Git/fabric-explorer-quickstart

When someone wants to use your project, they just need to:
1. Clone the repository
2. Follow the instructions in README.md 