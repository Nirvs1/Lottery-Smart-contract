# Lottery-Smart-contract
A smart contract the selects a winner from a list of players who send a minimum amount of Ethereum partake in the lottery.
The lottery.sol was written is solidity version 0.4.17 and the updated version will be uploaded to my profile in due time.
The contract accepts a minimum of 0.01 ether from any address and automatically adds the address to a list of players.
The function pickWinner() is restricted only to the creator of the contract.
I also added a getPlayers() function to output the list of players who have joined the lottery.
The getPlayers() function is not private and accessible to all.
Javascript was used to interact with the web3 instance and a couple of tests were run in the lottery.test.js file.

Variables used:
manager
Players[] (please note that this is a dynamic array)

Also when the manager tells the smart contract to pick a winner, you have to understand that in solidity it is impossible to generate random numbers.
So we have to create a pseudo-random number with the use of the block difficulty, time of transaction and all the players listed in the array.
With all these we then perform a keccak256 or sha3 algorithm to get a large hexadecimal which is then used as an argument into a uint function.

Most of this code was written in Javascript and less in solidity.
