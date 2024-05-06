# awesome-psbt
Here you can find useful content about PSBTs:

- [How PSBTs are used in different projects:](#section1)
  - [Security of PSBT on Magic Eden](#section1.1)
  - [Bitcoin Auctions on Magic Eden](#section1.2)
  - [Contracts State Based on UTXOs in RGB protocol](#section1.3)
  - [OKX implementation of PSBTs withinin their 'Discover' platform](#section1.4)
  - [Ordinals Protocol utilizes PSBTs for trading Bitcoin NFTs](#section1.5)
  - [Lightning CoinJoins](#section1.6)
  - [CoinSwap Wallet](#section1.7)
  - [Wasabi Wallet CoinJoin](#section1.8)
  - [Portal's Ordinal Atomic Swaps](#section1.9)
- [Possible use cases of psbt](#section_possible_use_cases) 
- [PSBTs challenges](#section2)
- [BIPs](#section3)
- [Libraries](#section4)
- [BTC Runes](#section5)
- [Inscriptions](#section6)
- [Learn](#section7)

<a id="section1"></a>
## How different projects are using PSBTs right now
<a id="section1.1"></a>
- [Security of PSBT on Magic Eden](https://help.magiceden.io/en/articles/7191642-safeguarding-your-bitcoin-transactions-exploring-the-security-of-psbt-on-magic-eden)
<a id="section1.2"></a>
- [Bitcoin Auctions on Magic Eden](https://help.magiceden.io/en/articles/8437081-dive-into-the-world-of-bitcoin-auctions-on-magic-eden)
<a id="section1.3"></a>
- [Contracts State Based on UTXOs in RGB protocol](https://lbanklabs.medium.com/renaissance-of-bitcoin-scaling-iv-rgb-0ce0a3c8a656)
<a id="section1.4"></a>
- [OKX implementation of PSBTs withinin their 'Discover' platform](https://finance.yahoo.com/news/flash-news-okx-wallet-enhances-030800985.html)
<a id="section1.5"></a>
- [Ordinals Protocol utilizes PSBTs for trading Bitcoin NFTs](https://research.aimultiple.com/how-do-ordinals-marketplaces-work/)
<a id="section1.6"></a>
- [Lightning CoinJoins](https://thebitcoinmanual.com/articles/lightning-coinjoins/)
<a id="section1.7"></a>
- [CoinSwap Wallet](https://www.coinswap.space/)
<a id="section1.8"></a>
- [Wasabi Wallet CoinJoin](https://blog.wasabiwallet.io/sending-psbt-transactions/)
<a id="section1.9"></a>
- [Portal's Ordinal Atomic Swaps](https://bitcoin-takeover.com/portal-presents-ordinal-atomic-swap-tech-demo/)

<a id="section_possible_use_cases"></a>
## Possible use cases of PSBTs
- Light Pools (https://rodarmor.com/blog/tag/markets/)
- Bitcoin lottery contract (https://github.com/supertestnet/bitcoin-lottery-contract/)
- Transaction Data, Inputs & Outputs in Ordinals (https://github.com/ordinals/ord/discussions/3709)
- Bring CRDT to ordinals (https://github.com/ordinals/ord/discussions/3657)

<a id="section2"></a>
## PSBT challenges
- txn-mempool-conflict (https://github.com/bitcoinjs/bitcoinjs-lib/issues/2093)
- Taproot script-spend-path with sighash ALL|ANYONECANPAY (https://github.com/bitcoinjs/bitcoinjs-lib/issues/2046)
- PSBT Taproot Key Path Finalizer Assumes Fixed 64-byte Signature Length (https://github.com/bitcoinjs/bitcoinjs-lib/issues/2004)
- error in signing PSBT transaction via electrum (https://bitcoin.stackexchange.com/questions/117149/how-to-resolve-error-when-trying-to-sign-and-broadcast-psbt-transaction-via-elec)
- Multi Signature with PSBT (https://github.com/zkSNACKs/zIPs/issues/60)
- bitcoins blocked on wasabi wallet (https://github.com/zkSNACKs/WalletWasabi/discussions/12652)

<a id="section3"></a>
## BIPs
- BIP 0174 (https://en.bitcoin.it/wiki/BIP_0174)
- BIP 0370 (https://en.bitcoin.it/wiki/BIP_0370)
- BIP 0371 (https://en.bitcoin.it/wiki/BIP_0371)
- BIP 0372 (https://en.bitcoin.it/wiki/BIP_0372)

<a id="section4"></a>
## Libraries / tools:
- Bitcoinlib (https://github.com/petertodd/python-bitcoinlib)
- bitcoinjs (https://github.com/bitcoinjs/bitcoinjs-lib)
- bitcointx (https://pypi.org/project/python-bitcointx/)
- btclib (https://btclib.org/)
- rust-bitcoin (https://github.com/rust-bitcoin/rust-bitcoin)
- munstr: MuSig + Nostr (https://github.com/0xBEEFCAF3/munstr)

<a id="section5"></a>
## BTC Runes
- Tokens on BTC: Casey Rodarmor Creator of Runes (https://www.youtube.com/watch?v=q9RDE8U6CkI)
- What is Runes (https://runes.gitbook.io/xrcmarket/learn/what-is-runes)
- RuneLib (https://github.com/sCrypt-Inc/runelib)
- Issue discussion "How PSBTs work? ([Figure out how PSBTs work](https://github.com/casey/runestone/issues/46))

<a id="section6"></a>
## Inscriptions
- BRC20 standard (https://ordiswap.gitbook.io/ordiswap/protocol-concepts/brc-20-standard)
- Things you Need To Know About Inscriptions (https://www.forbes.com/sites/digital-assets/2023/12/31/things-you-need-to-know-about-bitcoin-inscription/?sh=5787b8562859)
- Ordiscan (https://ordiscan.com/)
- Dune Ordinals Dashboard (https://dune.com/dataalways/ordinals)
- Casey Rodarmor: Creator of Ordinals Protocol (https://www.youtube.com/watch?v=IS406ToIRo4)

<a id="section7"></a>
## Learn

### Podcasts:
- Rodarmor podcast (https://hellpodcast.money/)
- Ledger's New Bitcoin App: PSBT, Taproot (https://podcasts.apple.com/mu/podcast/slp337-salvatore-ingala-ledgers-new-bitcoin-app-psbt/id1415720320?i=1000547513341)
- Episode 78: Partially Signed Bitcoin Transactions (https://www.youtube.com/watch?v=vyJhvGCfo88)
- How to Buy, Sell and Mint Runes (https://www.youtube.com/watch?v=hGtZBlAkTKw)

### Books, Docs:
- Mastering Bitcoin (https://books.google.kz/books?id=4TfhEAAAQBAJ&dq=btc+psbt+whitepaper&hl=ru&source=gbs_navlinks_s)
- How to Bitcoin (https://www.google.kz/books/edition/How_to_Bitcoin/31UnEAAAQBAJ?hl=ru&gbpv=0)
- Bitcoin for Dummies (https://www.google.kz/books/edition/Bitcoin_For_Dummies/Nl9iEAAAQBAJ?hl=ru&gbpv=0)
- Runes - Ordinal Theory Handbook (https://docs.ordinals.com/runes.html)
- A Bitcoin Smart Contract Glossary: Tools and Best Practices (https://github.com/supertestnet/btcsmartcontracts)
- Chain Signatures (https://docs.near.org/build/chain-abstraction/chain-signatures)
- Submarine Swap - On-chain to Off-chain (https://bitcoinjs-guide.bitcoin-studio.com/bitcoinjs-guide/v5/part-three-pay-to-script-hash/submarine_swaps/swap_on2off_p2wsh)
- PSBTs: Bitcoin Ordinals Wiki (https://bitcoinordinals.fandom.com/wiki/PSBTs)

### Articles:
- The Basic Concept of PSBTs (https://medium.com/@emmanuelchidera/the-basic-concept-of-psbts-b21c18b5a40f)
- In-depth Concept of Partially Signed Bitcoin Transactions: Part 2 (https://medium.com/@emmanuelchidera/in-depth-concept-of-partially-signed-bitcoin-transactions-part-2-548d1eafad46)
- CoinJoin (https://en.bitcoin.it/wiki/CoinJoin)
- CoinSwap (https://en.bitcoin.it/wiki/CoinSwap)
- Atomic Swap (https://en.bitcoin.it/wiki/Atomic_swap)
- How Do PSBT Dutch Auctions Work for Bitcoin Ordinal NFTs? (https://trustmachines.co/blog/how-do-psbt-dutch-auctions-work-for-bitcoin-ordinal-nfts/)
- What Are Bitcoin Runes? Bringing Memecoins to Bitcoin (https://www.coingecko.com/learn/what-are-bitcoin-runes#:~:text=Runes%20in%20the%20Bitcoin%20Ecosystem&text=As%20each%20Runestone%20corresponds%20to,simple%2C%20efficient%2C%20and%20secure.)
- Runes Protocol: Explained (https://trustwallet.com/ru/blog/runes-protocol-explained)
- NFT 101: The Comprehensive Guide to Runestone & Runes Protocol (https://medium.com/nftscan/nft-101-the-comprehensive-guide-to-runestone-runes-protocol-4193d1f8dce2)
- Renaissance of Bitcoin Scaling V — Runes Protocol (https://lbanklabs.medium.com/renaissance-of-bitcoin-scaling-v-rune-protocol-9e518297d1dc)
- Ordinals & PSBT — A Fresh Start for the Bitcoin Ecosystem (https://scalinglabs.medium.com/ordinals-psbt-a-fresh-start-for-the-bitcoin-ecosystem-50e0e543ad59)
- PSBT vs Smart Contracts: An In-Depth Comparison for 2024 (https://www.marketingscoop.com/ai/psbt-vs-smart-contracts/)
- The PSBT Standard (https://dev.to/eunovo/the-psbt-standard-i0d)
- Bitcoin news: all the developments on the Lightning Network and the introduction of the PSBT standard (https://en.cryptonomist.ch/2023/06/15/bitcoin-news-arrive-psbt-lightning-network/)
- Basic Analysis of Bitcoin BRC20 Ecosystem (https://dao.stafi.io/t/basic-analysis-of-bitcoin-brc20-ecosystem/89)
- Taproot: You Betcha (https://blog.bitmex.com/taproot-you-betcha/)
- WASABI VERSUS SAMOURAI: TX0 HAS NOTHING TO DO WITH IT (https://bitcoinmagazine.com/technical/wasabi-vs-samourai-for-bitcoin-mixing#:~:text=Wasabi%20elects%20to%20create%20very,anonymity%20across%20many%20successive%20transactions)
- JoinStr: Decentralized CoinJoin Implementation Using Nostr (https://www.nobsbitcoin.com/joinstr-decentralized-coinjoin-implementation-using-nostr/)
- zkSNACKs blocks U.S. users from Wasabi Wallet and other services (https://www.theblock.co/post/291293/zksnacks-blocks-u-s-users-from-wasabi-wallet-and-other-services)
- ZKSNACKS Coinjoin Coordination Service Will Stop Functioning From June 1 (https://coinedition.com/zksnacks-coinjoin-coordination-service-will-stop-functioning-from-june-1/)
- SLP364 MAX HILLEBRAND ZKSNACKS BLACKLISTING COINS (https://stephanlivera.com/episode/364/)
- WASABI WALLET’S ADVISORY FOR TREZOR USERS (https://blog.wasabiwallet.io/wasabi-wallets-advisory-for-trezor-users/)
- THE NOSTR PRIVACY PARADOX (https://bitcoinmagazine.com/technical/how-nostr-can-improve-bitcoin-privacy)

### Discussions
- Offer PBST design (https://github.com/ordinals/ord/issues/2706)
- Figure out how PSBTs work (https://github.com/casey/runestone/issues/46)
- Dynamic variable offer (https://github.com/casey/runestone/issues/105)
- AMM infrastructure design (https://github.com/casey/runestone/issues/21)
- The Wacky Zone (https://github.com/casey/runestone/issues/26)
- Buy and Sell Inscriptions/Rare Sats (Buy and Sell Inscriptions/Rare Sats)
- Takers & Makers (https://twitter.com/rodarmor/status/1778962658265628769)
- Multisig Address (https://twitter.com/zhouzhuojie/status/1709313943012044893)
- PSBTs are fantastic atomis swaps on Bitcoin, except the are centralizing force on Ordinals trading (https://twitter.com/BobBodily/status/1746257358312067531)

