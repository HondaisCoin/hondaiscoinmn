HondaisCoinMN Core staging tree 1.0.0
===============================

https://www.hondaiscoin.com


What is HondaisCoinMN?
----------------

HondaisCoinMN is an experimental new digital currency that enables anonymous, instant
payments to anyone, anywhere in the world. HondaisCoinMN uses peer-to-peer technology
to operate with no central authority: managing transactions and issuing money
are carried out collectively by the network. HondaisCoinMN Core is the name of the open
source software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the HondaisCoinMN Core software, see https://www.hondaiscoin.com


    Algorithm: x11
    Block type:   POW/MN
    Coin name: HondaisCoinMN
    Coin Ticker: HDCMN
    RPC port: 7819
    P2P port: 7820
    Block reward: 20 coins
    Masternode reward: 50%
    Masternode Collateral: 1000 HDCMN
    Premine: First block is 500,000,000 HDCMN / it will be use for swap ,airdrop, bounty program and system managment. 


License
-------

HondaisCoinMN Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is meant to be stable. Development is normally done in separate branches.
[Tags](https://github.com/HondaisCoin/hondaiscoinmn/) are created to indicate new official,
stable release versions of HondaisCoinMN Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](/doc/unit-tests.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`

There are also [regression and integration tests](/qa) of the RPC interface, written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/qa) are installed) with: `qa/pull-tester/rpc-tests.py`

The Travis CI system makes sure that every pull request is built for Windows
and Linux, OS X, and that unit and sanity tests are automatically run.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.


