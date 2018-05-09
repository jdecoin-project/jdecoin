Jdecoin integration/staging tree
================================

http://www.jdecoin.net

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2014 Ltecoin Developers
Copyright (c) 2018 JDECoin Developers

What is Jdecoin?
----------------
JDEcoin, an internet currency runs on scrypt algorithm. Functions and security features are the same as other known decentralized cryptocurrencies. You can find the waller installer for Windows here.

It was developed by a group of developers and analyst as well as crypto lovers to contribute to the improvement of the structure of the crypto community. JDecoin technology draws inspiration from the well-known Bitcoin and Litecoin and with enhanced security measures for better safekeeping.

Predominantly, 80% of the JDEcoin is already premined in keeping with the emerging trend as the smart contracts or ICOs.

Further, the premined coins are intended for development and marketing purposes --airdrops and bounties.And speaking of incentives, this will prove superior over ICOs in terms of incentivizing development teams.

The main core is the decentralization which enables to share and fosters freedom currently dominated by few.

 - premined coins
 - 20 sec block targets
 - subsidy halves in 50,000 blocks (~3 years)
 - 200 coins per block
 - 2021 blocks to retarget difficulty

For more information, as well as an immediately useable, binary version of
the Jdecoin client software, see http://www.jdecoin.net.


# Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src/
    make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake JDECOIN_QT_TEST=1 -o Makefile.test jdecoin-qt.pro
    make -f Makefile.test
    ./jdecoin-qt_test

