# Milestone Delivery :mailbox:

> ⚡ Only the GitHub account that submitted the application is allowed to submit milestones. 
> 
> Don't remove any of the mandatory parts presented in bold letters or as headlines! Lines starting with `>`, such as this one, can be removed.

**The [invoice form :pencil:](https://docs.google.com/forms/d/e/1FAIpQLSfmNYaoCgrxyhzgoKQ0ynQvnNRoTmgApz9NrMp-hd8mhIiO0A/viewform) has been filled out correctly for this milestone and the delivery is according to the official [milestone delivery guidelines](https://github.com/w3f/Grants-Program/blob/master/docs/Support%20Docs/milestone-deliverables-guidelines.md).**  

* **Application Document:** [https://github.com/w3f/Grants-Program/blob/master/applications/solidity-trie-verifier.md](https://github.com/w3f/Grants-Program/blob/master/applications/solidity-trie-verifier.md) 
* 
* **Milestone Number:** 1

**Context**
> This milestone presents the completion of the Solidity Trie library, enabling gas efficient Verification of Substrate style merkle patricia tries.

**Deliverables**

| Number | Deliverable | Link | Notes |
| ------------- | ------------- | ------------- |------------- |
| 0a. | License | [https://github.com/polytope-labs/solidity-merkle-trees/blob/merkle-patricia-trie/LICENSE](https://github.com/polytope-labs/solidity-merkle-trees/blob/merkle-patricia-trie/LICENSE) | Apache 2.0 | 
| 0b.  | Documentation |[https://github.com/polytope-labs/solidity-merkle-trees/tree/merkle-patricia-trie#merkle-patricia-trie](https://github.com/polytope-labs/solidity-merkle-trees/tree/merkle-patricia-trie#merkle-patricia-trie)| |
| 0c | Testing and Testing Guide | Test coverage include; [unit test](https://github.com/polytope-labs/solidity-merkle-trees/blob/merkle-patricia-trie/forge/src/merkle_patricia.rs), [Solidity](https://github.com/polytope-labs/solidity-merkle-trees/blob/merkle-patricia-trie/test/MerklePatricia.t.sol) and [Fuzz Test](https://github.com/polytope-labs/solidity-merkle-trees/blob/merkle-patricia-trie/forge/fuzz/src/lib.rs) | |
| 1 | Solidity Scale Codec | [This](https://github.com/polytope-labs/solidity-merkle-trees/blob/merkle-patricia-trie/src/MerklePatricia.sol) includes functionality to decode the node enums using [`decodeNodeKind`](https://github.com/polytope-labs/solidity-merkle-trees/blob/a03bd6bf609e1a3cc5e79a3d87c1cacdbb5f8b7c/src/trie/substrate/SubstrateTrieDB.sol#L25), the [`ByteSlice`](https://github.com/polytope-labs/solidity-merkle-trees/blob/a03bd6bf609e1a3cc5e79a3d87c1cacdbb5f8b7c/src/trie/Bytes.sol#L7) can be utilized for decoding `Vec<Vec<u8>>` as earlier [discussed](https://github.com/w3f/Grants-Program/pull/1481#issuecomment-1409013021) | |
| 2 | Trie Verifier | [`VerifySubstrateProof`](https://github.com/polytope-labs/solidity-merkle-trees/blob/1c25889773cb817ffaf915c1b300061e9a91304d/src/MerklePatricia.sol#L30) along with it's sub-implementations(i.e [Node](https://github.com/polytope-labs/solidity-merkle-trees/blob/merkle-patricia-trie/src/trie/Node.sol), [NodeCodec](https://github.com/polytope-labs/solidity-merkle-trees/blob/merkle-patricia-trie/src/trie/NodeCodec.sol), [NibbleSlice](https://github.com/polytope-labs/solidity-merkle-trees/blob/merkle-patricia-trie/src/trie/NibbleSlice.sol)...) | |
