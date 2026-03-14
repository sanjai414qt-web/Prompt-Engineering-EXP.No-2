# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

 # AIM:

To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.

# SCENARIO:

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

# 1.CHATGPT

**1. Zero-Shot Prompt**

**prompt input**

Summarize the following article about "The Basics of Blockchain Technology" in about 80–100 words suitable for undergraduate students.


**output**

Blockchain technology is a decentralized digital ledger used to record transactions securely across a network of computers. Instead of relying on a central authority, data is stored in blocks that are linked together using cryptographic hashes, forming a secure chain. Each participant in the network maintains a copy of the ledger, which improves transparency and prevents data tampering. Consensus mechanisms such as Proof of Work and Proof of Stake help verify transactions. Blockchain is widely used in cryptocurrencies like Bitcoin and Ethereum and has applications in supply chain management, healthcare, and digital identity systems.

**2.Fewshot prompt**

**prompt input**

Example:

Article: Artificial Intelligence is the simulation of human intelligence in machines that are programmed to think and learn.

Summary: Artificial Intelligence allows machines to mimic human thinking and learning abilities.

Example 2:

Article: Cloud computing provides on-demand computing services such as storage, servers, and software through the internet.

Summary: Cloud computing allows users to access computing resources like storage and software online without owning physical hardware.

Now summarize the following article on "The Basics of Blockchain Technology" in a similar short format (80–100 words).

**output**

Blockchain is a decentralized digital ledger that securely records transactions across many computers in a network. Data is stored in blocks that are connected using cryptographic hashes, creating a chain that is difficult to alter. Each computer in the network maintains a copy of the ledger, which increases transparency and reliability. Blockchain systems use consensus mechanisms such as Proof of Work or Proof of Stake to validate transactions. Although it was first used for cryptocurrencies like Bitcoin, blockchain is now applied in areas such as healthcare, supply chain tracking, and digital identity management.

**3.Chain of thought prompt**

**prompt input**

Read the following article about "The Basics of Blockchain Technology".

Step 1: Identify what blockchain technology is.
Step 2: Explain how blockchain stores and secures data.
Step 3: Mention the role of consensus mechanisms.
Step 4: List important applications of blockchain.

After reasoning through these steps, create a clear 100-word summary suitable for undergraduate students.

**output**


Blockchain technology is a decentralized system used to securely record digital transactions across multiple computers. Data is organized into blocks that are connected using cryptographic hashes, forming a secure chain that prevents tampering. Since the ledger is distributed across many nodes, it improves transparency and eliminates the need for a central authority. Consensus mechanisms such as Proof of Work and Proof of Stake help verify and validate transactions within the network. Originally developed for cryptocurrencies like Bitcoin, blockchain is now used in areas such as supply chain tracking, healthcare data management, and digital identity systems.

# 2.GEMINI

**1.Zeroshot**

**prompt input**

Based on the text provided about blockchain, summarize the three main reasons why blockchain is considered more secure than traditional centralized ledgers in two sentences.


**output**

Blockchain is more secure because it uses a decentralized network of nodes to prevent a single point of failure and employs cryptographic hashing to link blocks, making data tampering easily detectable. Additionally, consensus mechanisms ensure that all participants agree on the validity of transactions without needing a central authority

**2.Fewshot prompt**

**prompt input**

Extract key definitions from the text in the following format:

Term: Ledger
Definition: A record of transactions or data entries.

Term: Node
Definition: Individual computers in a network that store copies of the blockchain.

Term: Hash
Definition:"


**output**

Term: Hash
Definition: A unique digital fingerprint generated from data in a block used to secure and link it to the previous block

**3.Chain of thought prompt**

**prompt input**

Explain what happens to a blockchain if a hacker tries to change a transaction in an old block. Break your answer down step-by-step:

Describe the change to the data.

Describe the effect on the Hash.

Describe the effect on the subsequent blocks.

Conclude with why the network would reject this.

**output**

1. Data Change: The hacker modifies a transaction amount in Block 2 of the chain.
2. Hash Impact: Because the hash is a unique fingerprint of the data, changing even one character causes the Hash of Block 2 to change entirely.
3. Chain Reaction: Since Block 3 contains the 'Previous Hash' of Block 2, the link is now broken because the stored hash no longer matches the new hash of Block 2. This invalidates all following blocks.
4. Conclusion: The rest of the nodes in the network will see that the hashes don't align and will reject the hacker’s version of the ledger in favor of the original, consistent

# 3.PERPLEXITY

**1.Zero shot prompt**

**prompt input**

Rewrite the following text about blockchain for undergraduate CS/IT students. Make it concise, engaging, and structured with headers/lists while keeping key concepts intact:


**output**

Consensus like Proof of Work (PoW) or Stake (PoS) validates transactions. Benefits: security, trust without middlemen. Used in crypto (Bitcoin), supply chains, healthcare. Key for modern distributed systems..

**2.Few shot prompt**

**prompt input**

Rewrite texts for undergrad CS/IT students: concise, structured, engaging.

Example 1:
Input: [Short text on databases]
Output: **Databases 101** ... [structured rewrite]

Example 2:
Input: [Short text on networks]
Output:**Networking Basics** ... [structured rewrite]


**output**

A distributed ledger of transaction blocks chained via hashes—change one, break the chain. Decentralized nodes agree via PoW/PoS. Advantages: secure, transparent, trustless. Apps: Bitcoin, supply tracking, patient records.

**3.Chain of thought**

**prompt input**

Rewrite the blockchain text below for CS/IT undergrads. Think step-by-step:

1. Identify core concepts: ledger, decentralization, blocks/hashes, consensus, advantages, uses.
2. Structure: Intro hook, explanation with analogy, sections for features/advantages/uses, conclusion.
3. Tone: Friendly, concise (under 400 words), use lists/headers.
4. Enhance: Add one analogy (e.g., for hashing).


**output**

Blockchain: Distributed ledger where nodes store identical blockchains of transactions. Hashes link blocks tamper-proof style. Consensus (PoW/PoS) validates sans central authority. Wins: Security, transparency, trust. Real uses: Crypto, supply chains, health records—vital for secure digital systems.

# comparison for three different platform

<img width="1721" height="1168" alt="ai_model_comparison_table" src="https://github.com/user-attachments/assets/326eac4d-bf41-4d3c-873e-152fecf62bd5" />

# RESULT:
Thus for comparing all three platform,chatgpt give more appropriate and precise answer.
