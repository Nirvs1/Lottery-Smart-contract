# Lottery-Smart-contract
A smart contract the selects a winner from a list of players who send a minimum amount of Ethereum partake in the lottery.
The lottery.sol was written is solidity version 0.4.17 and the updated version will be uploaded to my profile in due time.
The contract accepts a minimum of 0.01 ether from any address and automatically adds the address to a list of players.
The function pickWinner() is restricted only to the creator of the contract.
I also added a getPlayers() function to output the list of players who have joined the lottery.
The getPlayers() function is not private and accessible to all.
Javascript was used to interact with the web3 instance and a couple of tests were run in the lottery.test.js file.
