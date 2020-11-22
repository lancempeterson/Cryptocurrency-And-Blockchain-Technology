**CRYPTOCURRENCY AND BLOCKCHAIN TECHNOLOGY**

**Lance M. Peterson**

[**lancepeterson50@gmail.com**](mailto:lancepeterson50@gmail.com)

**Abstract**

The concept of currency has changed a lot since the days of barter systems and commodity money. The internet paved way for digital currencies, where transactions can be made instantaneous with people across the globe. Like other fiat currencies, digital currency is of no intrinsic value as it is simply a digital file. Files are easy to copy so it could be possible for someone to purchase two or more items using the same digital token. Is it possible to solve this issue without relying on a third party such as a financial institution? A solution to this problem was made in 2009 with the introduction of Bitcoin, the first ever cryptocurrency. Cryptocurrencies utilize a powerful technology called the blockchain which is essentially a growing list of records. We will examine how the blockchain works, the application of blockchain technology, and the challenges surrounding blockchain-oriented software engineering.

**Currency**

By most definitions, currency is money that can be used as a medium of exchange. Simply put, currency can be used to buy goods or services. Before currencies were widely used, people relied on a barter system to directly exchange goods and services. This barter system had many inconveniences. For example, if someone wanted to trade their soap for a block of cheese, they would have to find someone with cheese willing to trade it for soap. Over time, things like metals, livestock, and certain foods became commonly used and acceptable sources of exchange. This was due to the fact that these items were commonly found and easily quantifiable. There were still problems with this method. It was difficult to store wealth as many foods are not easy to store and some goods deteriorate over time. Also, there was a lack of divisibility of these goods. People wanted to trade things of equal value, which proved to be difficult to do because you cannot trade half of an animal for example. This led to the introduction of physical coins made out of precious metal. Currency with intrinsic value is referred to as commodity money, because the value of the currency comes from the commodity that they are made of, like gold or silver. Today, most countries use fiat money, which is currency with no intrinsic value. There is no value in the currency itself, and the currency is not backed up by anything of value. The reason fiat money works in because enough people have trust that currency holds a value. The US dollar is a fiat currency because the cotton and linen by which it is made holds very little value.

**Digital Currency**

Today money is being exchanged more and more over the internet. This is done with digital currency, a type of currency that is only available in digital form. The benefit of digital currency is that transactions can be made instantaneous, even with people across the globe. Digital currency is not something that exists in a physical form like a US Dollar or British Pound. However, it is no different than physical money when it comes to intrinsic value. It still only holds a value because people widely agree that it does.

**The Double-Spend Problem**

Since digital currencies are essentially digital files there exists a potential weakness in its use. Digital files are much easier to copy than physical currency so it could be possible for someone to buy two or more items using the same digital token. Suppose Alice has 1 digital token and decides to send it to Bob. At the same time Alice sends 1 digital token to Charlie. Alice only has 1 token in her account so how can we get confirmation to either Bob or Charlie the token they receive hasn&#39;t already been used? This is referred to as the double-spend problem. Double spending leads to inflation, and a loss of trust in the currency. There are two main ways to prevent double-spending. The first is a centralized prevention technique. This can be implemented by using a central trusted third party that can verify whether a token has been spent. This is when digital currency follows a centralized system shown in Figure 1.

![](RackMultipart20201122-4-1vqttvw_html_afc14c5eff422ec1.png)

Figure 1: Centralized System

Many systems follow centralized client-server architecture. Common examples of digital currency that follows a centralized system include credit cards, debit cards, Venmo, or Apple Pay. It is common for stored information, such as personal info and transactions to be all kept in a single database. We rely on trusted third parties to process transactions and hold user information. This setup means that everything is controlled by a single entity. This could be problematic as it means that there is a single point of failure. In a centralized system, a hacker could theoretically alter or delete information in the database. How can we solve this single point of failure issue, begin to trust the information we access, and trust the central party responsible for keeping this data?

**Cryptocurrency**

The answer is to use a decentralized or distributed system. Digital currency can also follow a system of decentralized control where there is a public transaction database which functions as a distributed ledger. This distributed ledger is known as a blockchain which will be elaborated on later, but for now understand that a blockchain is essentially a growing list of records. This is where cryptocurrency comes in. Cryptocurrency is a digital currency that acts as a medium of financial exchange on the blockchain platform. Cryptocurrency as the name suggests, uses cryptography to secure its transactions, control creation of additional units, and to verify the transfer of assets. Cryptocurrencies utilize two very important cryptography tools, namely hashing and digital signatures. These will be discussed later. Cryptography used to be a practice that only the military and spy agencies used in secret. That is, until the US government published the Data Encryption Standard and first publicly available work on public-key cryptography by Whitfield Diffie and Martin Hellman. A group of people named &quot;cypherpunks&quot; with ideas as to how use cryptography to transform many industries including digital currency. Some notable members in this group include Julian Assange the founder of WikiLeaks, Bram Cohen creator of BitTorrent, Hal Finney author of PGP 2.0, and more.

**Bitcoin**

Bitcoin was the first ever cryptocurrency. It was introduced in a white paper [1] by an unknown person or group under the pseudonym Satoshi Nakamoto. It is widely thought that one or more members of the cyherpunks are the founders of bitcoin. Its introduction came following the 2008 US stock market crash and big bank bailout so it was a time when there was very little trust in the financial institutions. Bitcoin gave the world a solution to the double-spend problem that did not put the fate of the entire money system on a central authority. When it comes to the double-spend problem it is obvious that there needs to be a way to keep track of all previous transactions. This is necessary so a payee can know that the previous owner of the token did not already make a transaction with it. The earliest transaction will be the valid transaction, while other attempts to spend the same token are checked and denied. Satoshi Nakamoto realized that there needs to be a system for participants to agree on a single history of the order in which transactions occur. This is in the form of a distributed ledger that keeps track of records called the blockchain.

**Blockchain**

Blockchain can be thought of a distributed database. One way to think of this is to imagine an online ledger that is duplicated thousands of times across a distributed network of computers. Since the information is not stored centrally, it is impossible to corrupt or steal vital data from one source. Before a hacker can perpetrate any form of attack on a block, such criminal needs to hack every ledger in the network (millions of information) at the same time and this is simply impossible. [7]

![Traditional vs Blockchain approach](img/BlockchainApproach.png?raw=true "Traditional vs Blockchain approach")

Figure 2: Traditional vs Blockchain approach [7]

**Hashing**

Cryptography plays a vital role in the blockchain. Blockchain uses cryptographic hashing to guarantee that no transactions in the history can be tampered with. Hashing itself is easy enough to understand. [10] It means taking an input string of any length, running it through a hashing algorithm such as SHA-256, and getting output of a fixed length string. Small changes in the input will result in large changes to the output. This is known as the &quot;avalanche effect&quot; and is a necessary trait of a good cryptographic function. If the hash function did not satisfy the avalanche effect to a significant degree, then someone could make predictions about the input if given the output. This increases the chance of someone cracking the algorithm used in the hash function. Figure 3 shows an example of a hash function with a good avalanche effect. It is shown that by changing a single bit in the input results in totally different output.

![Hashing example with avalanche effect](img/HashingAvalancheEffect.png?raw=true "Hashing example with avalanche effect")

Figure 3: Hashing example with avalanche effect

For cryptocurrencies like Bitcoin, the sequence of transactions for the current block and the previous block&#39;s hash are the inputs that are put into the hash function. The result is a new hash for the current block. Each block hash points to the block before it. This system makes it easy to ensure that no previous transactions have been altered because if any part of the transaction changes, so does the hash for the block it belongs to, and any following blocks. SHA-256 makes it so that everyone on the blockchain only needs to agree on a 256 bit string to represent the state of the blockchain. No matter how big the blockchain gets in size, the current state of the blockchain can always be represented in 256 bits!

**Digital Signatures**

Digital signature encryption is also essential for cryptocurrency and the blockchain to work. Users of the cryptocurrency use a key pair, which are a public key and a private key. The keys are related to each other mathematically using some known algorithm. Whatever is encrypted with a public key can only be decrypted by its corresponding private key.

![Public Key and Private Key](img/PublicKeyPrivateKey.png?raw=true "Public Key and Private Key")

Figure 4: Public Key and Private Key [9]

With bitcoin, a user has a Bitcoin address, which is a hash of the public key portion of the user&#39;s key pair. This can be shared with other users to receive cryptocurrency. The private key is used to act as a digital signature to sign off on transactions much like signature would work on a contract. Every transaction on the blockchain is digitally signed by the sender using their private key. In this way, only the owner of the account can send money out of their account. The signature of the previous token owner is used to verify that the current owner has ownership of that token. This is can be shown in Figure 5.

![Transaction digital signatures](img/DigitalSignatures.png?raw=true "Transaction digital signatures")

Figure 5: Transaction digital signatures [1]

A token can be thought of as a chain of digital signatures. Each owner transfers the token to the next owner by digitally signing a hash of the previous transaction and the public key of the next owner.

**Consensus Network and Proof-Of-Work**

To implement a network consensus protocol, the blockchain network for Bitcoin is comprised of a decentralized network of many different validating nodes. Each node uses a client that performs the task of validating and relaying transactions. As such, each node can be seen as an administrator capable of entering new data into the blockchain. For an addition to be made to the blockchain, the majority of nodes must reach consensus. Since all nodes verify new additions to the blockchain, this consensus mechanism guarantees the security of the network, making it almost impossible for a hacker to corrupt. Consensus resolves all discrepancies in the proposed transaction order all guarantees that all blockchain network nodes are operating on an identical ledger. So, how is consensus achieved if anyone can join the network? Cryptocurrencies use proof-of-work to do this. An example of a proof of work that most people are familiar with is a CAPTCHA. This is when you try to submit data on a web page and the form asks you to prove that you are a person. The web page makes you do some form of work, such as typing oddly shaped text from an image or clicking all squares in a picture that contain a street sign. Proof-of-work like this is important so that robots cannot send junk data super-fast to bring down the system. In Bitcoin, consensus is reached by what is called mining. About every 10 minutes mining computers collect hundreds of pending transactions, which is a block. The miners are trying to solve a complex hashing puzzle which involves trying to find a value that when hashed, the hash begins with a number of zero bits. The miner who finds a solution first gets to add their block the blockchain and they get a piece of bitcoin as a reward. This gives miners an incentive to participate in the system, using their power and computational resources to update and verify the blockchain. [6] There are a fixed number of bitcoins, and it is estimated that the bitcoin limit could be reached by 2140. Once this happens, incentives for miners will come from payments of money collected from senders and receivers in the form of transaction fees.

**Application of Blockchain**

While blockchain was originally created for cryptocurrency, the technology community is finding more and more potential applications for this technology. Blockchain technology has the power to completely revolutionize many aspects of today&#39;s world. It is thought that this new technology is set to make huge changes to many different industries much like how the introduction of the internet did. The most powerful applications of blockchain technology may be done with smart contracts.

**Smart Contracts**

The use of cryptocurrency and blockchain technology has expanded the emerging application of smart contracts. [5] Smart contracts are essentially self-executing programs that happen when certain conditions are met. The benefit of this is that it helps eliminate the inherent issues with traditional business transaction. Using smart contracts it becomes easy to exchange anything from money, business shares, properties, and more, conflict-free without having to make transaction payments to middlemen. Smart contracts define the rules and penalties of an agreement in the same way that a traditional business contract would, but it also automatically enforces the contract obligations. The process of creating a smart contract is relatively simple, involving three steps. First the contract between two or more parties is written in code and posted on the blockchain. Next, an event has to happen to trigger the execution of the smart contract such as money being sent or an expiration date. Finally the contract self-executes according to the original terms that were coded and both parties get what was promised out of each other through the contract. With smart contracts you are assured of lowered cost of a transaction since you can bypass fees from a middleman and the potentially lengthy procedures associated with traditional financial transactions. Smart contracts add trust to the transaction because the documents involved are encrypted on a shared ledger, the other party or middleman can&#39;t say they lost them. This also means that the blockchain serves as a reliable backup, as your documents are duplicated multiple times over. Smart contracts can save someone a lot of time. Normally you would have to spend time filling out paper work to manually process documents. Smart contracts use code to automate these tasks, saving you precious time. Smart contracts are also very accurate. Assuming they are coded correctly, they avoid errors that could happen while filling out paper work manually.

Smart contracts are not without faults however. As with other software, there could be bugs in the code. Another problem arises if the contract is set to execute but the external situation changes. For example, suppose you have a contract for renting an apartment and your apartment is unexpectedly condemned making it impossible for you to live there. Normally the contract you made with the landlord could be rescinded in court with the help of a lawyer. However if a smart contract was made, it will perform its code for the transaction with no way to stop it. Challenges like this are roadblocks that are stopping some businesses from adopting smart contract technology. Many experts are working on potential solutions to get over these hurdles.

**Blockchain-oriented software engineering**

As blockchain technology is reshaping many different industries there is a need for companies and software engineers to have an understanding of blockchain-oriented software. Blockchain-oriented software is defined as all software working with an implementation of a blockchain. [2] There are some challenges facing software engineers practicing blockchain-oriented software (BOS) and it would benefit them to be aware of. The first need is the specialized skills and education needed to fill the professional role of working with BOS. Due to the nature of the blockchain, many financial and legal entities have shown great interest in this software. Skills in finance and law will become critical to pair with an expertise in software engineering. An education involving more than just computer science and software engineering will become almost necessary to have the skills needed in developing BOS. The next is being aware of the testing techniques that will work best with BOS. In the software engineering world, a test suite is a group of test cases that are used to test a software program and show that is has some specified set of behaviors and functionality. Specific test suites should be considered when performing testing on BOS. The first is smart contract testing (SCT). SCT is concerned with making tests ensuring that smart contracts satisfy the clients specifications, comply with the laws and legal systems involved, and not do include unfair contract terms. The next test suite is blockchain transaction testing (BTT). BTT is concerned with creating tests that ensure the integrity of transaction status and that the software doesn&#39;t allow double spending.

**Conclusion**

In a new digital age, cryptocurrencies may very well be the financial system of the future. Anyone can benefit greatly from having knowledge of the history of cryptocurrency, the problems it solves, and how it is implemented. Cryptocurrency may have introduced the world to the power of the blockchain, but any industry could find ways to utilize this new technology. Software engineers looking to get into blockchain-oriented software development should understand the specialized skills and testing practices needed to have success implementing a blockchain to their software project.

**References**

[1] Nakamoto, S. (2009). Bitcoin: A peer-to-peer electronic cash system. Retrieved from [https://bitcoin.org/bitcoin.pdf](https://bitcoin.org/bitcoin.pdf)

[2] A. Abran, J. W. Moore, P. Bourque, R. Dupuis, and L. Tripp, &quot;Swebok: Guide to the software engineering body of knowledge 2004 version,&quot; IEEE Computer Society, Los Alamitos, California, 2004.

[3] Hoyt, K. (2004). Blockchain Vocabulary. Retrieved from http://www.kevinhoyt.com/2017/04/11/blockchain-vocabulary/

[4] S, L. (2015) How Bitcoin mining works. Retrieved from https://www.economist.com/blogs/economist-explains/2015/01/economist-explains-11

[5] Kukushkina, N. (2018) Blockchain Solutions: The way to Transform Your Business Processes. Retrieved from https://dashbouquet.com/blog/blockchain/blockchain-solutions-the-way-to-transform-your-business-processes

[6] _Bitcoin total bitcoins in circulation_. (2014, March 14). Retrieved from https://blockchain.info/charts/total-bitcoins?timespan=all&amp;showDataPoints=false&amp;daysAverageString=1&amp;show\_header=true&amp;scale=0&amp;address=

[7] Reyes, A. (2017) the World of Blockchain. Retrieved from https://medium.com/michiganblockchain/the-world-of-blockchain-f3b268e3d748

[8] Marvin, R. (2017) Blockchain: The Invisible Technology that&#39;s Changing the World. Retrieved from https://www.pcmag.com/article/351486/blockchain-the-invisible-technology-thats-changing-the-word

[9] Comodo. Public Key and Private Keys Retrieved from https://www.comodo.com/resources/small-business/digital-certificates2.php

[10] Rosic, A. What is Hashing? Under the Hood of Blockchain. Retrieved from https://blockgeeks.com/guides/what-is-hashing/
