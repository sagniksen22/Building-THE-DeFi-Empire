# Building-THE-DeFi-Empire

# README: Deploying an EVM Subnet on Avalanche, Integrating with MetaMask, and Testing with Remix

## Overview

This README provides a step-by-step guide to deploy an EVM subnet on Avalanche using the Avalanche CLI, add the subnet to MetaMask, deploy smart contracts using Remix, and test your application.

### Prerequisites

Ensure you have the following installed:

- Avalanche CLI
- MetaMask browser extension
- Remix IDE (online or locally)
- Node.js and npm (optional for additional tooling)

### Steps

#### 1. Deploy Your EVM Subnet Using the Avalanche CLI

1. **Install Avalanche CLI**: Follow the instructions from the [Avalanche documentation](https://docs.avax.network/build/tools/avalanche-cli) to install the Avalanche CLI.
   
2. **Create a New EVM Subnet**: Run the following command to create a new EVM subnet:

   ```bash
   avalanche subnet create myEvmSubnet
   ```

3. **Deploy the Subnet**: Deploy your subnet to the Avalanche network:

   ```bash
   avalanche subnet deploy myEvmSubnet
   ```

4. **Note the RPC URL**: After deployment, note the RPC URL provided by the CLI.

#### 2. Add Your Subnet to MetaMask

1. **Open MetaMask**: Click on the network dropdown and select "Add Network".

2. **Fill in Network Details**: Use the RPC URL noted earlier and fill in the other required details:

   - Network Name: `My EVM Subnet`
   - New RPC URL: `<Your RPC URL>`
   - Chain ID: `<Your Subnet Chain ID>`
   - Currency Symbol: `AVAX`
   - Block Explorer URL: `<Optional>`

3. **Save the Network**: Click "Save" to add the network to MetaMask.

#### 3. Select Your Subnet Network in MetaMask

Ensure that your newly added subnet network is selected in MetaMask by clicking on the network dropdown and selecting `My EVM Subnet`.

#### 4. Connect Remix to Your MetaMask

1. **Open Remix IDE**: Go to the [Remix IDE](https://remix.ethereum.org/).

2. **Connect MetaMask**: Click on the "Deploy & Run Transactions" tab on the left sidebar.

3. **Select Injected Provider**: In the "Environment" dropdown, select `Injected Web3`. MetaMask will prompt you to connect. Confirm the connection.

4. **Ensure Correct Network**: Make sure that Remix is connected to the `My EVM Subnet` network.

#### 5. Deploy Smart Contracts

1. **Write Your Smart Contract**: In the Remix IDE, create a new file (e.g., `MyContract.sol`) and write your smart contract code.

2. **Compile the Contract**: Go to the "Solidity Compiler" tab and compile your contract.

3. **Deploy the Contract**: Go to the "Deploy & Run Transactions" tab, select your compiled contract, and click "Deploy". Confirm the transaction in MetaMask.

#### 6. Test Your Application

1. **Interact with Deployed Contracts**: Use Remix to interact with your deployed smart contracts by calling functions and sending transactions.

2. **Deploy Tokens, Pools, and More**: Utilize Remix to deploy additional contracts such as tokens or liquidity pools.

### Additional Information

For more details on using the Avalanche CLI, MetaMask, and Remix, refer to their official documentation:

- [Avalanche CLI Documentation](https://docs.avax.network/build/tools/avalanche-cli)
- [MetaMask Documentation](https://metamask.io/faqs.html)
- [Remix Documentation](https://remix-ide.readthedocs.io/en/latest/)

---

By following these steps, you can deploy an EVM subnet on Avalanche, add it to MetaMask, deploy smart contracts using Remix, and thoroughly test your application.
