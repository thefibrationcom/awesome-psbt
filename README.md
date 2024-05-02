# awesome-psbt
Here you can find useful content about PSBTs:

- [How PSBTs are used in different projects:](#section1)
  - [Security of PSBT on Magic Eden](#section1.1)
  - [Bitcoin Auctions on Magic Eden](#section1.2)
  - [Contracts State Based on UTXOs in RGB protocol](#section1.3)
  - [OKX implementation of PSBTs withinin their 'Discover' platform](#section1.4)
  - [Ordinals Protocol utilizes PSBTs for trading Bitcoin NFTs](#section1.5)
- [PSBTs challenges](#section2)
- [BIPs](#section3)
- [Libraries](#section4)
- [BTC Runes](#section5)

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
- 
<a id="section2"></a>
## [PSBT challenges](https://d-central.tech/what-is-a-partially-signed-bitcoin-transaction-psbt/)
- txn-mempool-conflict (https://github.com/bitcoinjs/bitcoinjs-lib/issues/2093)
- Taproot script-spend-path with sighash ALL|ANYONECANPAY (https://github.com/bitcoinjs/bitcoinjs-lib/issues/2046)
- PSBT Taproot Key Path Finalizer Assumes Fixed 64-byte Signature Length (https://github.com/bitcoinjs/bitcoinjs-lib/issues/2004)
- error in signing PSBT transaction via electrum (https://bitcoin.stackexchange.com/questions/117149/how-to-resolve-error-when-trying-to-sign-and-broadcast-psbt-transaction-via-elec)

<a id="section3"></a>
## BIPs
- BIP 0174 (https://en.bitcoin.it/wiki/BIP_0174)
- BIP 0370 (https://github.com/bitcoin/bips/blob/master/bip-0370.mediawiki)
- BIP 0371 (https://github.com/bitcoin/bips/blob/master/bip-0371.mediawiki)
- BIP 0372 (https://github.com/bitcoin/bips/blob/master/bip-0372.mediawiki)

<a id="section4"></a>
## Libraries:
- Bitcoinlib (https://github.com/petertodd/python-bitcoinlib)
- bitcoinjs (https://github.com/bitcoinjs/bitcoinjs-lib)
- bitcointx (https://pypi.org/project/python-bitcointx/)
- btclib (https://btclib.org/)
- rust-bitcoin (https://github.com/rust-bitcoin/rust-bitcoin)

<a id="section5"></a>
## BTC Runes
- What is Runes (https://runes.gitbook.io/xrcmarket/learn/what-is-runes)
- RuneLib (https://github.com/sCrypt-Inc/runelib)
- Issue discussion "How PSBTs work? ([Figure out how PSBTs work](https://github.com/casey/runestone/issues/46))
