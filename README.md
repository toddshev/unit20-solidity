# Deploying a Smart Contract with Solidity

### Technologies Used

In order to deploy a Smart Contract on the Ethereum Blockchain, you will need to install and configure Ganache, install the Metamask extension in your browser, and utilize the Remix IDE located at www.remix.ethereum.org.

### Code for a Smart Contract

For this example, we will be depositing an amount into the contract, then dispersing it evenly among three employees.
If there is a remainder, the balance will be sent back to the message sender.
  * The constructor will accept the names (blockchain addresses) of the recipients.
  * There is a function to return the balance of the contract.
  * There is a deposit function, the heart of the application.
  * There is an external payable function to ensure funds do not get locked in the contract.

The code will be written in the Remix IDE.  Create a new contract called _AssociateProfitSplitter.sol_.  The code below will create the smart contract that will perform the aforementioned tasks.

![CodeWindow](/Screenshots/CodeWindow.png)


### Deployment

Once completed, compile the code, then prepare to deploy.  The deployment window should look similar to this:

![Deploy](/Screenshots/DeployConfig.png)

There is no Wei required to deploy a contract, though there will be a gas fee, so ensure the address has been pre-funded.  On a test network, there are various faucets you may go to in order to fund it.

Before deploying, enter the 3 employees (addresses) which will be recipients of the funds. When you click _Deploy_ the Metamask window will pop up asking you to confirm.  Upon successful deployment, you should scroll to the bottom of the left pane, and click the down arrow to show the contract's available functionality:

![Functionality](/Screenshots/Functionality.png)

Scroll back to the top to select the deposit amount, then click on "Deposit" near the bottom.  Ensure you do not try to deposit more than is available in the message sender account.

