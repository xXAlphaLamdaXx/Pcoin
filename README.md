PCoin Core integration/staging tree
=====================================

What is PCoin?
----------------

PCoin is an experimental digital currency that enables instant payments to
anyone, anywhere in the world. PCoin uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. PCoin Core is the name of open source
software which enables the use of this currency.

Specifications
----------------------

Halving of block reward every 69120 blocks (4 months)
A new block every 2.5 minutes
Normal block reward of 50 Pcoins
When you mine a block you have to wait 16 blocks to spend the reward of 50 Pcoins
Difficulty retarget every day
Block size up to 2KB for massive save in storage
Total supply 6.912.000 coins

On testnet, which is a network to test the capabilities of the network, retargets are every 14 days, blocks every 30 seconds for quick confirmation with halvings every month. Because 50% of the testnet coins come in the first month and in the next few months the supply will be exhausted, please donate your coins to other testnet users. Total testnet supply 8.640.000 coins

In regtest, which is a private blockchain for more centralised experiments, halvings occur every 16 blocks (40 minutes) with block target every 2.5 minutes. Because of the non-permanence of this network, difficulty adjustments happen every 14 days. Total regtest supply 1.600 coins.

License
-------

PCoin Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/test), written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and macOS, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

We only accept translation fixes that are submitted through [Bitcoin Core's Transifex page](https://www.transifex.com/projects/p/bitcoin/).
Translations are converted to PCoin periodically.

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.
