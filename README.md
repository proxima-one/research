# Research

*This is a repository of research that is guiding the development of Proxima. We have authored some of these papers for the networking and data layer of our Protocol. Several other papers have been included because they have promising applications in the blockchain data layer. The goal of the Proxima Protocol is to create a decentralized blockchain agnostic data layer that provides rich and performant queries on indexed data. In order to accomplish this goal, our research has focused on several areas of interest:*

- **Authenticated data structures** are used to increase the performance, and improve the feature-set of ProximaDB. 
- **Networking** will mediate routing, synchronization, bootstrapping, and load-balancing of the protocol network. 
- **Decentralized payments and authentication** will be the incentive mechanism for our protocol.
- **Optimized rollups** are the method upon which we build and verify fraud proofs for data queries.  


## B+ Merkle Tree
The primary area of focus was authenticated data structures. There exists a large body of research on authenticated data structures, but this research has pushed towards unordered, batched, zero-knowledge solutions like RSA accumulators. The B+ Merkle tree, the data structure that we developed, optimizes efficient proofs and fast range queries so that it can play the role of an ordered authenticated index for a  performant authenticated database. 


> ### **Dynamic B+ Merkle Tree with Efficient Proofs**
> 
> *A recursive data structure that mimics a B+ tree, with polynomial commitments to provide constant-sized intranode proofs with arbitrary branching factors. This 
> structure is designed to act as a database index to enable range proofs for authenticated relational databases.*
> 
> *(https://arxiv.org/pdf/2006.01994.pdf)*


## Efficient Peer-to-Peer Networking
While researching a method for synchronization and routing within the network, we decided to use a hybrid of guassian mixture models and location-based addressing to construct the distributed hash tables of peers within the network. This approach was designed to lower the latency of individual message paths,  as well as the overall load on the network. This methodology for network addressing will be utilized for the distribution of data across geographies. 

> ### **Proximity-based Networking: Small world overlays optimized with particle swarm optimization**
> 
> *A distributed peer-to-peer network that uses dynamic Gaussian Mixture Models to build a small-world distributed hash table that ensures efficient and low latency message routing.*
> 
> *(https://arxiv.org/abs/2006.02006)*



## Other Areas of Interest
Along with the papers we have authored. There are several papers and ideas that we draw inspiration from.

### Optimistic and Zk-Rollups
Optimistic and zk-rollups  utilize a chain of state transitions. They can be used to construct fraud proofs, that can be verified by stateless clients. Our system

**Important links and papers**
- **Rollups**

https://dyor-crypto.fandom.com/wiki/Rollups


### Decentralized payments and authentication
Decentralized payments are used as the incentive and authorization mechanism for the Proxima Protocol. Our initial focus is on integrating a hybrid solution for payments and authentication. It would include authentication based on a staked addresses signatures along with the potential authentication relying on the distribution of micro-transactions, or packetized rewards.


#### **Important links and papers**
- **Packet-payments**

https://dl.acm.org/doi/abs/10.1145/3286062.3286067?casa_token=USUZsV2Tsi0AAAAA:lKE8tIyHjw4kzn1RyP4iIFC5qVLvMA7eAk4KaPdQejnxgE-Hl2IeNUdsIHyiwzrE1zGLru3gtnS04ws
- **Micro-transactions and Streaming payments**

https://anrg.usc.edu/www/papers/streamingDataPaymentProtocol_2018.pdf
- **API tokens**

https://www.researchgate.net/profile/Khalid_Aloufi/publication/338209250_Secure_IoT_Resources_with_Access_Control_over_RESTful_Web_Services/links/5e6669a04585153fb3cea156/Secure-IoT-Resources-with-Access-Control-over-RESTful-Web-Services.pdf






