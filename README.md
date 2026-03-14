EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

AIM:

To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.

SCENARIO:

You are part of a content curation team for an educational platform that delivers quick summaries of research papers to undergraduate students. Your task is to summarize a 500-word technical article on "The Basics of Blockchain Technology" using multiple AI platforms and prompting strategies.

Your goal is to determine which combination of prompting technique + platform provides the best summary in terms of:

1.Accuracy

2.Coherence

3.Simplicity

4.Speed

5.User experience

# OUTPUT:

**THE BASICS OF BLOCK CHAIN TECHNOLOGY**

Blockchain technology is a modern digital system used to record and store information in a secure, transparent, and decentralized way. It was first introduced as the underlying technology behind the cryptocurrency Bitcoin, but today it is used in many industries such as finance, healthcare, supply chain management, and digital identity systems. For undergraduate students studying computer science or information technology, understanding the basics of blockchain helps in learning how modern secure digital systems work.

At its core, a blockchain is a distributed digital ledger. A ledger is simply a record of transactions or data entries. In traditional systems, a ledger is usually maintained by a central authority such as a bank or an organization. However, blockchain works differently because it is decentralized. Instead of being controlled by a single organization, copies of the ledger are stored across multiple computers in a network called nodes. Each node has the same version of the blockchain, which ensures transparency and reduces the risk of data manipulation.

The term “blockchain” comes from the way data is stored. Information is grouped into blocks, and each block contains a list of transactions. Once a block is filled with data, it is linked to the previous block using cryptographic techniques, forming a chain of blocks. Each block contains a hash, which is a unique digital fingerprint generated from the data in that block. The hash of the previous block is also stored in the current block, creating a secure link between them. If someone tries to change the data in one block, its hash will change, which immediately breaks the connection with the next block. This mechanism makes blockchain highly resistant to tampering.

Another important feature of blockchain technology is consensus mechanisms. Since there is no central authority controlling the system, the network must agree on which transactions are valid. Consensus mechanisms are algorithms used to achieve this agreement among the nodes. One common method is Proof of Work (PoW), where computers solve complex mathematical problems to validate transactions. Another method is Proof of Stake (PoS), where validators are chosen based on the number of tokens they hold and are willing to stake as collateral.

Blockchain also offers several advantages compared to traditional data systems. First, it provides security through cryptography and distributed storage. Second, it ensures transparency, because every transaction recorded on the blockchain can be verified by participants in the network. Third, it improves trust, as users do not need to rely on a central authority to confirm transactions.

Today, blockchain technology is used in many real-world applications. Cryptocurrencies like Bitcoin and Ethereum use blockchain to record financial transactions securely. In supply chain management, blockchain helps track products from manufacturers to consumers, ensuring authenticity and reducing fraud. In healthcare, it can be used to securely store patient records while allowing authorized access to medical professionals.

In conclusion, blockchain technology is an innovative system that provides secure, transparent, and decentralized data management. As industries increasingly adopt digital systems, blockchain is becoming an important technology for ensuring data integrity and trust in modern applications. Understanding its basic concepts helps students appreciate how distributed systems and cryptography work together to create reliable digital infrastructures.

**1. Zero-Shot Prompt**

~~~
Summarize the following article about "The Basics of Blockchain Technology" in about 80–100 words suitable for undergraduate students.
~~~
RESULT:
