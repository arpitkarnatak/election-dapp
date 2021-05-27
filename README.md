## Poll Booth
This is a decentralized applcation built using Solidity and React. 

### Features of this application
1. Voters can only be registered by one specific account.
2. Voters won't be registered by name. Only their addresses. Hence, 1 account can only have one voter.
3. Candidates can register themselves. They can enter their name and click Register and a candidate by the name written would be registered at that address.
4. One address can only have one candidate to it.
5. Vote can only be casted from the accounts registered as voters.
6. Once the vote is casted from an address, another vote cannot be casted to maintain integrity of the application.

### Setting up Ganache
1. Open ganache. Click on Create New Workspace.
2. On the truffle project menu, add the truffle-config.js file of this project.
3. Go to server and set port number to 7545.
4. Click save workspace and it'll start a new blockchain instance. Every time you open ganache, you can select this workspace and view your transactions.

### Setting up Metamask
1. Download metamask extenstion from https://metamask.io/
2. After installation, it'll take you to a window to set a password. Select the option to import wallet from seed phrase and set a password.
3. Use the mnemonic from the ganache instance.
4. A localhost blockchain would be added in the list of networks. Change the port number to 7545.

#### Setting up the local development environment
Run the ganache Blockchain and type the following commands in terminal:

git clone https://github.com/arpitkarnatak/election-dapp.git \
npm install \
truffle compile \
truffle migrate (or truffle migrate --reset) \
cd client \
npm install \
npm start 

(truffle migrate if using for the first time. truffle migrate --reset for everytime you want to create a new contract instance and wipe out the old data)
