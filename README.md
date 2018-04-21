Jdecoin integration/staging tree
================================

http://www.jdecoin.net

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2014 Ltecoin Developers
Copyright (c) 2018 JDECoin Developers

What is Jdecoin?
----------------

Jdecoin is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.
 - premined coins
 - 20 sec block targets
 - subsidy halves in 4,665,600  blocks (~3 years)
 - +77 billion total coins

The rest is the same as Bitcoin and Litecoin, combined.
 - 200 coins per block
 - 2021 blocks to retarget difficulty

For more information, as well as an immediately useable, binary version of
the Jdecoin client sofware, see http://www.jdecoin.net.

License
-------

Jdecoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Jdecoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/jdecoin-project/jdecoin/tags) are created
regularly to indicate new official, stable release versions of Jdecoin.



# Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake JDECOIN_QT_TEST=1 -o Makefile.test jdecoin-qt.pro
    make -f Makefile.test
    ./jdecoin-qt_test

