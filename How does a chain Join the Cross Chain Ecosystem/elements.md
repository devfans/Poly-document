<h1 align="center">Essential Chain Elements Need to be Clarified</h1>


## Introduction

Before starting implementation, some features and attributes are required for joining the cross-chain ecosystem. These features are the critical elements for implementing the core interface method for handling block headers or cross-chain transactions.

## Requirement List

1. **Consensus Algorithm**

The Consensus Algorithm determines how blockchains select consensus validators,  voters, and block producers for minting new blocks and bookkeeping block transactions. The developers need to clearly understand the consensus protocol of the blockchain to get sufficient information for validating block headers.
For instance, for blockchains that use POS, one of the essential elements for verifying blocks are signatures from validator nodes, which requires the developers Know the consensus nodes' election process, and who are the consensus nodes in the next epoch.

2. **Genesis Block of the Chain**

The genesis block's block header needs to be submitted to the consortium chain of the cross-chain ecosystem to verify the consequent transactions and block headers on this chain.

3. **Block Header Structure and Verification Method **

The block header verification and processing method and the block structure need to be submitted so that the relay chain can verify the block headers that will be transferred from this chain.

The side chain needs to provide its block header format, the serialization, and the deserialization methods. The mode of signature verification allows the relay chain to process and verify block headers.

4. **Merkle Tree Structure and Verification Method**

The Merkle tree structure, the Merkle tree generation, and the verification method for the ledger records or transactions need to be submitted to the relay chain to verify cross-chain transactions from this chain. 

The source chain stores cross-chain information and construct a Merkle tree, and then sends the Merkle tree root and the Merkle proof of the information to the side chain. The side chain verifies the proof using the Merkle root and confirms the validity of the cross-chain information.

Merkle proofs are a solution. When events and transactions are recorded on the blockchain, a corresponding Merkle proof, by having a Merkle proof and the correct block header, we can prove that a particular transaction or event did occur on the chain with certainty.




