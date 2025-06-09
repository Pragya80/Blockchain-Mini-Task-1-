# Blockchain-Mini-Task-1

1.) BLOCKCHAIN BASICS

Blockchain: Blockchain is like a unique kind of notebook. It is shared with group of people, Once you wite something in it, it cannot be removed or changed. Every member of the group has a copy, and they all agree on what's written through the system.Through this all records are saved honestly and there is no need of any central authority or boss. In blockchain the chain is created by connecting block to the previos one. Everyone know that a page change is fraudulent. Due to this Blockchain very helpful and secure for safely storing crucial information without relying on a middleman, such as money transfer, agreements, or records, without needing to trust a middleman.

Example:
I. Art Provenance and ownership-> The artwork is registered as NFT, That is the proof you own that artwork even copies exist of that artwork. This helps artist to earn.

II. Charity Donation-> In many fundraisers, we never really know where the money goes. But with the help of Blockchain we can able to see the entire path of the donation.

2.)BLOCK ANATOMY

┌────────────────────────────────────────────────────────────┐
│                         BLOCK                              │
├────────────────────────────────────────────────────────────┤
│ Timestamp    : 2025-06-09 02:35:00                          │
│ Nonce        : 45219                                       │
│ Previous Hash: 0000abc1...45fe                             │
│ Merkle Root  : 8e9c4f...d7a1                               │
├────────────────────────────────────────────────────────────┤
│                       DONATION DATA                        │
│ TX1: Riya donated ₹100 to “FoodForAll”                     │
│ TX2: Aman donated ₹250 to “CleanWaterNow”                 │
│ TX3: Zoya donated ₹500 to “TreeMission”                   │
│ TX4: Ravi donated ₹150 to “EduFund India”                 │
└────────────────────────────────────────────────────────────┘

The Merkle root uses hash functions to compile a block's transactions, acting as a last seal or fingerprint. It assists in confirming that the information within hasn't been altered or tampered with.

Example:
I. Riya donated ₹100 to FoodForAll
II. Aman donated ₹250 to CleanWaterNow
III. Zoya donated ₹500 to TreeMission
IV. Ravi donated ₹150 to EduFund India

The Merkle root is the single hash that remains at the top after each transaction is transformed into a hash, combined, and hashed once more.

Imagine someone tries to change one record like changing Aman donated 250 to 50. This change completely change the hash of that transaction.
Result- Changed hash will affect the combined hash above it.
        This change travel up.
        At last the merrkle root will be different from the original.
So the current one not matching the original merkle root, Then we instantly know something has been changed in data.

3.) CONSENSUS CONCEPTUALIATION

Q-What is Proof of Work and why does it require energy?
To add a block to the blockchain, computers must solve Proof of Work, which is similar to a challenging puzzle. After much trial and error, the computer continues to guess answers (nonces) until it finds one that satisfies the rules. PoW is an energy-intensive guessing game because it requires powerful machines that consume a lot of electricity and time. Because solving the puzzle demonstrates that one did the "work," it is made so that cheating is difficult.

Q-What is Proof of Stake and how does it differ?
Based on how much cryptocurrency a user "stakes" or locks up, such as making a security deposit, Proof of Stake determines who adds the next block. Similar to having more raffle tickets, your chances of being selected increase with the amount you stake. There isn't much computer work involved, consequently, it consumes a lot less energy than Proof of Work. Because PoS depends on financial commitment rather than brute-force computing, it is more environmentally friendly.

Q-What is Delegated Proof of Stake and how are validators selected?
The way Delegated Proof of Stake operates is similar to a democracy: coin holders elect a select group of reliable individuals, known as validators or delegates, to oversee the blockchain. People can vote these validators out if they behave badly. They alternately add blocks. Compared to PoW or PoS, this system is quicker and more scalable, but it relies on voting process trust. It's similar to designating class representatives to turn in your work rather than having everyone complete it themselves.
