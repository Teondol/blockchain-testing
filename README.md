# blockchain-testing
This is a simple blockchain implementation in Node.js.

## Installation
npm install blockchain-testing


## Usage

```javascript
const { Blockchain, Block } = require('blockchain-testing');

// Create a new blockchain
let myBlockchain = new Blockchain();

// Add a new block to the blockchain
let newDataBlock = new Block(Date.now(), { amount: 5 });
myBlockchain.addBlock(newDataBlock);

// Check if the blockchain is valid
console.log('Blockchain valid?', myBlockchain.isChainValid());