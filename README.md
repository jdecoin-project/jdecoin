Jdecoin integration/staging tree
================================

http://www.jdecoin.net

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2014 Ltecoin Developers
Copyright (c) 2018 JDECoin Developers

What is Jdecoin?
----------------

Jdecoin is a tweak combined of Bitcoin and Litecoin using scrypt as a proof-of-work algorithm.
 - premined coins
 - 20 sec block targets
 - subsidy halves in 4,665,600  blocks (~3 years)
 - +77 billion total coins
 - 200 coins per block
 - 2021 blocks to retarget difficulty

For more information, as well as an immediately useable, binary version of
the Jdecoin client sofware, see http://www.jdecoin.net.


# Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src/
    cd leveldb/
    chmod +x build_detect_platform
    cd ..
    make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake JDECOIN_QT_TEST=1 -o Makefile.test jdecoin-qt.pro
    make -f Makefile.test
    ./jdecoin-qt_test

