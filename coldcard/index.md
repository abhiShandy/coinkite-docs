menu-title: Table of Contents
title: Coldcard User Documentation
ordering: 1000

# Quick Start

- [Official getting started with your new Coldcard guide](quick)
- [Coldcard Video Tutorials <mark>NEW</mark> (near 20 videos! Make sure to subscribe)](https://www.youtube.com/playlist?list=PLZKkuPrgFw0axLoDDzxAIYzpZeC_T1i7W)
- [How to upgrade the firmware](upgrade)

### Guides by Others

- Full guides
	- [Coldcard 101 by Bitcoin Q+A (Basic intro, Main features, How to set one up, Receive and send a transaction using Electrum, Create a backup, Adding a passphrase)](https://www.bitcoinqna.com/post/coldcard-101)

- Electrum
	- [Video: How to use ColdCard with **Electrum**](https://www.youtube.com/watch?v=9A0cS2wwMI0)
	- [How to make offline transactions in **Electrum** with Coldcard wallet.](https://medium.com/@Multicripto/how-to-make-offline-transactions-in-electrum-with-coldcard-wallet-838f84df379a) | [Spanish](https://medium.com/@Multicripto/c%C3%B3mo-hacer-transacciones-offline-con-coldcard-wallet-a-trav%C3%A9s-de-electrum-b2eeb847e4b2)
	- [Video: How To Use Coldcard Wallet | Setup + Electrum Wallet](https://www.youtube.com/watch?v=_6mgLnTxPUs)


- Wasabi
	- [End to End Coldcard setup by Bitcoin Citadel](https://mattodell.keybase.pub/BitcoinCitadel_%20Coldcard_Wasabi%20Reference%20Guide.pdf)
    - [Video: Using Coldcard with **Wasabi Wallet**](https://www.youtube.com/watch?v=kocEpndQcsg)
	- [Video: TFTC Guides: Coldcard + **Wasabi** Wallet Basic Setup and Usage](https://www.youtube.com/watch?v=sM2uhyROpAQ)


- CLI & ckcc-protocol
	- [Video: Coldcard wallet](https://www.youtube.com/watch?v=f8dBNrlwJ0k)
	- [Video: **Passphrase over ckcc-protocol**](https://www.youtube.com/watch?v=zP1VV0AB5Os)

- BTCPay Server
	- [Video: Connecting Coldcard wallet to BTCPay Server](https://www.youtube.com/watch?v=N0eVwdP_7EQ)
	- [Video: Coldcard wallet and BTCPay Server - PSBT Sending from a wallet airgapped](https://www.youtube.com/watch?v=oK0h-76Giaw)
	
- Bluewallet
	- [Video: How to use Coldcard with Bluewallet](https://www.youtube.com/watch?v=hF2MyDB0nno)

- Misc
	- [How to use an SD card of more than 32GB with Coldcard](https://hive.blog/coldcard/@transisto/how-to-use-an-sd-card-of-more-than-32gb-with-coldcard)
	- [Video: Setting up ColdCard Mark2 **Wallet Backup**](https://www.youtube.com/watch?v=w6MvnUu2GBo)
	- [Video: Coldcard **PIN Design and Operation**](https://www.youtube.com/watch?v=iuiOqqZ8eeU) 
	- [Video: How to set up the **different PINs** of Cold Card Wallet](https://www.youtube.com/watch?v=hk1Lq2Rp2KM) 
	- [Video: Secure **Upgrade Firmware** of ColdCard Mark 2](https://www.youtube.com/watch?v=JCZzugnfQPs) 
	- [Video: **Unbagging** the ColdCard Mark2](https://www.youtube.com/watch?v=5FwOOTYH7Uw) 
	- [Video: How To Use Coldcard Wallet | Import-Backup Wallets + Settings](https://www.youtube.com/watch?v=M3miU_xp-IY)
	- [Videos em Portugues: Coldcard | Tutorial Completo](https://www.youtube.com/watch?v=jutQyA0X_Sc&list=PLgcVYwONyxmgyS3fAPkLCyejKEDQJWRLd)
	- [Video: How to show your Coldcard balance on iPhone](https://www.youtube.com/watch?v=xWeQwOyEDhI&t=356s)
	- [Protect your Bitcoin with an Electrum Multisig wallet, with Coldcard, Ledger, and Trezor](https://medium.com/@1700constantino/protect-your-bitcoin-with-an-electrum-multi-sig-wallet-with-coldcard-ledger-and-trezor-96397e4ce287)


- Reviews
	- [Video: Ministry of Nodes Review - Coinkite Coldcard Mk2](https://www.youtube.com/watch?v=eXInjdY9AM8)

# Learn About Your New Coldcard

- [**Upgrade**](upgrade) to the latest firmware.

- [Hardware features](hardware) including keypad and connectors.

- [BIP39 Encrypted seeds](passphrase) allows unlimited wallets.

- [Use a D6 Dice](import#dice-rolls) to pick a random private key.

- [Understanding the settings](settings) on your Coldcard.

- [Advanced Menu](advanced) commands.

- [Multisig](multisig) features.

- How [Encrypted Backups](backups) work on the Coldcard.

- How to install and use the [command line (CLI) tools.](cli)

- Read the [Frequently Asked Questions (FAQ)](faq) and [Trouble-shooting](trouble) tips and tricks.

- Wallet [software download (ie. Electrum)](downloads)


# User Guide Chapters

{% for p in PAGES if not p.hidden %}
1. [{{p.menu_title}}]({{p.url}})
{%- for sd in  p.childern(PAGES) %}
    - [{{sd.menu_title}}]({{sd.url}})
{%- endfor %}
{% endfor %}

# Advanced Topics

- [HSM Mode and the CKBunker](ckbunker-hsm) to permit automated signing and remote access.
- Your can view and download the [source code on Github](https://github.com/coldcard/firmware).
- Long and detailed discussion of 
  [PIN codes and the security element]({{DOCS}}/pin-entry.md) that holds the real secrets.
- Details of our [encrypted backup files]({{DOCS}}/backup-files.md).
- Documented [limitations]({{DOCS}}/limitations.md), policy choices, and TODO items.
- [Importing seed words ]({{DOCS}}/electrum-usage.md) into Electrum for funds recovery and other tips.
- How to use with [Bitcoin Core.]({{DOCS}}/bitcoin-core-usage.md) 
- How [developers can modify Coldcard]({{DOCS}}/dev-access.md) to extend it.
- [Memory map]({{DOCS}}/memory-map.md)  highlights.

# **Mk3** Specifications

- Size: 88 x 51 x 9 mm
- Weight: approximate 30 grams
- Power: 20 to 40mA
- [Unofficial Volumetric 3D model [STP]](https://github.com/TiKawamoto/3d-printing/tree/master/Coldcard) by [@TiKawamoto](https://twitter.com/TiKawamoto/status/1257489848388239362)
