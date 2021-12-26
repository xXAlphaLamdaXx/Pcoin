PCoin Core
=============

Setup
---------------------
PCoin Core is the original PCoin client and it builds the backbone of the network. It downloads and, by default, stores the entire history of PCoin transactions, which requires approximately 1 gigabyte of disk space. Depending on the speed of your computer and network connection, the synchronization process can take anywhere from a few seconds to a minute or more.

Running
---------------------
The following are some helpful notes on how to run Litecoin Core on your native platform.

### Unix

Unpack the files into a directory and run:

- `bin/litecoin-qt` (GUI) or
- `bin/litecoind` (headless)

### Windows

Unpack the files into a directory, and then run litecoin-qt.exe.

### macOS

Drag Litecoin Core to your applications folder, and then run PCoin Core.

### Need Help?

* See the documentation at the [Litecoin Wiki](https://litecoin.info/)
for help and more information.
* Ask for help on [#litecoin](http://webchat.freenode.net?channels=litecoin) on Freenode. If you don't have an IRC client use [webchat here](http://webchat.freenode.net?channels=litecoin).
* Ask for help on the [LitecoinTalk](https://litecointalk.io/) forums, in the [Technical Support section](https://litecointalk.io/c/technical-support).

Building
---------------------
The following are developer notes on how to build PCoin Core on your native platform. They are not complete guides, but include notes on the necessary libraries, compile flags, etc.

- [Dependencies](dependencies.md)
- [macOS Build Notes](build-osx.md)
- [Unix Build Notes](build-unix.md)
- [Windows Build Notes](build-windows.md)
- [FreeBSD Build Notes](build-freebsd.md)
- [OpenBSD Build Notes](build-openbsd.md)
- [NetBSD Build Notes](build-netbsd.md)
- [Gitian Building Guide (External Link)](https://github.com/bitcoin-core/docs/blob/master/gitian-building.md)

---------------------
Distributed under the [MIT software license](/COPYING).
This product includes software developed by the OpenSSL Project for use in the [OpenSSL Toolkit](https://www.openssl.org/). This product includes
cryptographic software written by Eric Young ([eay@cryptsoft.com](mailto:eay@cryptsoft.com)), and UPnP software written by Thomas Bernard.
