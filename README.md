# LiveCodeBlockchainDemo
This is a very basic visual introduction to the concepts behind a blockchain using LiveCode

This LiveCode stack contains a series of cards that contain code and objects to demonstrate the core principles of how a Blockchain work.

Card 1 demonstrates how a SHA256 Hash value is created for a data field where the user can enter data.  As the users types, every character recalculates the Hash.

Card 2 demonstrates how a Block is created and signed by Mining the Block.  A block's hash is calculated using the Block Number, Nonce and the Data.  If the Hash doesn't have 4 leading zeros, then it is considered to be "Unsigned" by this demo's rules for a signed block.  For example, if you type hi into the Data field, a Nonce of 59396 will be needed to generate a Hash with 4 leading zeros.

Card 3 demonstrates how a series of Blocks become a Blockchain and how the chain preserves the integrity of the chain using signed hashes.  There is a dependency Hash that comes from the proceeding Block that ensures that the current block can only be valid if the previous black values have not changed once it was Mined and Signed. Any change in a preceding Block will invalidate the following Block.
