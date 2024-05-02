# awesome-psbt
Place where you can find useful content about PSBTs:
- How PSBTs are used in different projects:
  - Security of PSBT on Magic Eden
  - Bitcoin Auctions on Magic Eden
  - Contracts State Based on UTXOs in RGB protocol
  - OKX implementation of PSBTs withinin their 'Discover' platform
  - Ordinals Protocol utilizes PSBTs for trading Bitcoin NFTs
- PSBTs challenges
- How to create/sign/broadcast psbt using different approaches

## How different projects are using PSBTs right now

### [Security of PSBT on Magic Eden]([url](https://help.magiceden.io/en/articles/7191642-safeguarding-your-bitcoin-transactions-exploring-the-security-of-psbt-on-magic-eden))
Magic Eden emphasizes safety and accessibility in Bitcoin transactions through Partially Signed Bitcoin Transactions (PSBT). Here's a breakdown of the key points:

- Wallet and Private Key Protection: Magic Eden ensures the privacy and security of users' wallets and private keys by not accessing them directly. Instead, the platform interacts with users' Bitcoin wallets to securely guide them in signing PSBT transactions.
- Confidentiality of Partial Signatures: Sellers' partial signatures for listings remain confidential and are never exposed to the public. Magic Eden has open-sourced and published msigner, a signing tool for PSBT, ensuring utmost security for transactions and personal information.
- Robust Encryption and Security Measures: Magic Eden employs the NaCl encryption system and AWS Key Management Service (KMS) to manage cryptographic keys, guaranteeing the highest standard of encryption management for user signatures.
- Buyer Responsibility: Buyers are responsible for signing the full transaction, ensuring comprehensive knowledge of transaction details and contributing to overall transaction security.
- Access to Open-Source Details: Users can access open-source details and information through Magic Eden's GitHub repository and Twitter thread.
- Invalidation of Old Listings: Magic Eden is developing an ordinal batch-transfer tool for on-chain invalidation of previous listings, ensuring gas-efficient transfer of ordinals to wallets and invalidating previous off-chain listings.
- Advantages of PSBT: PSBT offers secure and efficient transaction execution in Bitcoin Ordinal platforms. By safeguarding sellers' partial signatures and employing high-quality encryption, PSBT enables confident buying and selling of Digital Artifacts. The transparent and open-source nature of PSBT facilitates ongoing improvements and user-friendly experiences for users of all experience levels.

### [Bitcoin Auctions on Magic Eden]([url](https://help.magiceden.io/en/articles/8437081-dive-into-the-world-of-bitcoin-auctions-on-magic-eden))
Magic Eden facilitates Bitcoin auctions through a user-friendly process that integrates cutting-edge blockchain technology. Here are the key points:

- Connecting Wallet: Users connect their wallets like Unisat, Xverse, or Hiro to Magic Eden Bitcoin.
- Navigating to Auctions: Users navigate to their desired Bitcoin auction page.
- Auction Wallet: Magic Eden provides a unique auction wallet for depositing bid funds, featuring a multisig contract for security.
- Transferring Funds: Users initiate deposits from their wallets to the auction wallet to participate in auctions.
- Deposit Confirmation: Funds show as "Pending" until confirmed, typically taking two confirmations.
- Direct Deposit Limitation: Direct deposits from BTC wallets to the bidding wallet aren't supported yet, but a workaround is available.
- Bidding Process: Users bid from their available balance, with the current top bid and remaining time displayed.
- Unbroadcasted PSBT: Magic Eden uses an unbroadcasted PSBT system, eliminating gas fees until the auction concludes.
- Winning and Receiving Artifacts: The top bidder's PSBT is broadcasted after the auction, and they receive the digital artifact automatically.
- Withdrawal: Users can withdraw funds from the bidding wallet back to their connected wallet.
- Recommendations: Magic Eden recommends larger bid deposits, anticipating network delays, and managing auction balances effectively for a seamless experience.

Overall, Magic Eden aims to streamline the Bitcoin auction process, making it efficient and accessible for both seasoned bidders and newcomers in the digital art space.

### [Contracts State Based on UTXOs in RGB protocol]([url](https://lbanklabs.medium.com/renaissance-of-bitcoin-scaling-iv-rgb-0ce0a3c8a656))
Partially Signed Bitcoin Transactions (PSBT) within the RGB protocol for managing contract states. Here are the key points:

- Contract State Evolution in RGB: Contract states in RGB are linked to unspent transaction outputs (UTXOs) on the Bitcoin blockchain. Each state is associated with an issuer and defined by a schema outlining validation rules for client-side validation.
- State Change Actions: Ownership of a contract state can change through various actions, such as spending the UTXO, transferring ownership, or making it a global state. When a new state is created, a PSBT containing the underlying witness transaction is generated by the wallet and sent to RGB nodes.
- State Chain as a DAG: The state chain in RGB forms a directed acyclic graph (DAG) of state transitions. This DAG is maintained as client-validated data, enabling participants to trace UTXO records and verify the history of state changes independently.
- Inheritance of Security from Single-Use Seals: RGB employs the concept of single-use seals, with UTXOs serving as seals. When a new state is created, the previous state is revealed and closed, generating a new UTXO. This approach prevents double spending and ensures the integrity and reliability of state transitions, inheriting the security of the Bitcoin network.
- Integrity and Security: RGB's management of contract states ensures the integrity and security of transitions while leveraging the scalability and privacy advantages of client-side validation.

In summary, the RGB protocol utilizes PSBT to manage contract states on the Bitcoin blockchain efficiently. This integration ensures robust security, integrity, and scalability for state transitions within the protocol.

### [OKX implementation of PSBTs withinin their 'Discover' platform]([url](https://finance.yahoo.com/news/flash-news-okx-wallet-enhances-030800985.html))
OKX Wallet's integration of Partially Signed Bitcoin Transactions (PSBT) to enhance accessibility for Bitcoin decentralized applications (DApps) through its 'Discover' platform. Here are the key points:

- Introduction of PSBT Functionality: OKX Wallet has upgraded its 'Discover' platform to incorporate the PSBT signature function, a standard in Bitcoin transactions. PSBT facilitates the portability of unsigned transactions, allowing multiple parties to easily sign the same transaction.
- Overcoming Previous Limitations: Prior to this upgrade, users of OKX Wallet's Discover platform faced limitations in utilizing BTC-related DApps due to the absence of PSBT functionality. This upgrade aims to address these limitations.
- Seamless Interaction with Bitcoin DApps: With the implementation of PSBT, users can now seamlessly connect to and interact with Bitcoin DApps such as UniSat, Magic Eden, and idclub directly through OKX Wallet's Discover platform.
- Transaction History Display: Additionally, OKX Wallet users can now view their transaction histories for Bitcoin-related DApps, further enhancing transparency and usability.
- Diverse Offering on Discover Platform: OKX Wallet's Discover platform boasts over 5,500+ DApps, decentralized exchanges (DEXs), blockchain games, non-fungible tokens (NFTs), and supplementary tools, providing users with a comprehensive ecosystem to explore and engage with.

In summary, OKX Wallet's integration of PSBT functionality within its Discover platform expands accessibility and usability for Bitcoin DApps, offering users a seamless experience to connect with various applications and explore the broader blockchain ecosystem.

### [PSBT challenges]([url](https://d-central.tech/what-is-a-partially-signed-bitcoin-transaction-psbt/))
The challenges and limitations associated with Partially Signed Bitcoin Transactions (PSBT) and discusses ongoing developments to address these issues. Here are the key points:

- Learning Curve and Operational Complexity: PSBTs introduce a learning curve and operational complexity, especially for new Bitcoin users or those not technically inclined. The multi-step process of creating, signing, and broadcasting PSBTs can be daunting compared to traditional Bitcoin transactions, potentially hindering widespread adoption among casual users.
- Size and Complexity of PSBT Files: PSBT files can become large and complex, particularly in transactions with multiple inputs, outputs, or signatures. Each component adds to the file's size, making it cumbersome to handle, especially when bandwidth and storage are limited. Managing and verifying the information within PSBT files can also be challenging, requiring careful attention to detail to avoid errors.
- Ongoing Developments and Future Prospects: Developers in the Bitcoin community are actively working on enhancements and new versions of the PSBT standard to address its limitations. PSBT version 2 (BIP 370) is one such development aiming to improve transaction construction efficiency, support new transaction types, and reduce the size and complexity of PSBT files. These enhancements aim to simplify the PSBT process while retaining its security and flexibility benefits.
- Community Commitment to Improvement: The ongoing development of PSBT underscores the Bitcoin community's commitment to evolving and improving the network's capabilities. Future iterations promise to enhance the security, privacy, and interoperability of Bitcoin transactions, offering new possibilities for users and developers alike.

In summary, while PSBTs offer significant advantages for Bitcoin transactions, they also present challenges such as operational complexity and large file sizes. Ongoing developments, including PSBT version 2, aim to address these limitations, ensuring that PSBT remains a valuable tool for the Bitcoin ecosystem.

### [Ordinals Protocol utilizes PSBTs for trading Bitcoin NFTs]([url](https://research.aimultiple.com/how-do-ordinals-marketplaces-work/))
Ordinals marketplaces utilize Partially Signed Bitcoin Transactions (PSBT) for trading Bitcoin NFTs. Here's a summary of how Ordinals incorporate PSBTs into their marketplace operations:

- PSBT Solution Overview: Ordinals marketplaces adopt a PSBT solution, as proposed by Bitcoin Improvement Proposal (BIP) 174, to streamline multi-party transactions involved in trading Bitcoin NFTs. PSBT simplifies transactions requiring authorization by multiple signees before broadcasting to the Bitcoin network.
- PSBT Process Steps:
  - Transaction Creation: A group member generates a PSBT file containing transaction details, such as inputs (UTXOs being spent) and outputs (UTXO destinations), without signatures.
  - Transaction Signing: The PSBT creator sends it to other group members for approval and signing.
  - Transaction Finalization: Once the PSBT gathers all required signatures, it becomes 'final' and ready for broadcast. The final signer transforms the PSBT into a fully signed transaction.
  - Broadcast: The fully signed transaction is then broadcast to the Bitcoin network, where it undergoes confirmation, completing the transaction on the Bitcoin blockchain.
- Differences from Traditional NFT Marketplaces:
  - Transaction Handling: Ordinals marketplaces differ from traditional NFT marketplaces in transaction handling, signing, and confirmation processes.
  - Complexity: PSBT-enabled transactions on Ordinals typically involve multiple parties, additional security layers, and situations requiring approval from more than one party before confirmation, such as multi-signature wallets.
  - Transaction Process: PSBT-based transactions involve creating an unsigned transaction, obtaining signatures from necessary parties, finalizing it, and broadcasting it to the network.

In summary, Ordinals marketplaces leverage PSBTs to facilitate secure and multi-party transactions for trading Bitcoin NFTs. Unlike traditional NFT marketplaces, Ordinals employ PSBTs to handle more complex scenarios and ensure additional layers of security, providing a robust framework for trading on the Bitcoin network.

## How to create/sign/broadcast psbt

### PSBT on python:
- How to make a Bitcoin transaction with Python (https://medium.com/coinmonks/how-to-make-a-bitcoin-transaction-with-python-450d7d3db864)
- Bitcoinlib (https://github.com/petertodd/python-bitcoinlib)
- btclib (https://medium.com/coinmonks/how-to-make-a-bitcoin-transaction-with-python-450d7d3db864)

### PSBT on JS:
- psbt (https://github.com/alexbosworth/psbt)
- Creating Partially Signed Bitcoin Transactions (PSBTs) with Bitcoin Core and Node Js (https://medium.com/@teebams49/creating-partially-signed-bitcoin-transactions-psbts-with-bitcoin-core-and-node-js-bbb066c041b7)
- bitcoinjs (https://github.com/bitcoinjs/bitcoinjs-lib/blob/master/ts_src/psbt.ts)
- unchained bitcoin psbt (https://unchained-capital.github.io/unchained-bitcoin/module-psbt.html)
- send psbt with bitcoinjs (https://nhancv.medium.com/send-a-btc-bitcoin-transaction-with-bitcoinjs-psbt-24fd0d5b42d0)

### PSBT on RUST:
- rust psbt (https://github.com/tcharding/rust-psbt/)
- psbt (https://docs.rs/psbt/latest/psbt/)
- how ot sign psbt in RUST (https://medium.com/@clovrlabs/nodeguard-signer-extension-how-to-sign-a-psbt-in-rust-92414bb1fb70)
- build, sign and broadcast psbt in RUST (https://medium.com/@aifeanyi019/build-sign-and-broadcast-psbts-in-rust-part-1-0fca98c6af40)
