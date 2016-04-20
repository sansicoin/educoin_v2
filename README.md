EducoinV integration/staging tree
================================



Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2016 EducoinV Developers

What is EducoinV?
----------------

EducoinV --> Educoin Vietnam (EDC)
Developed and designed for students in Vietnam to support them and to grow up the quality of the education in this country.
On this way we want to support especially those, who live in rural areas and often do not have the chances to get the proper education.
Students can "earn" coins with their work, solving tasks homeworks etc.
The earned coins can be redeemed for school stuff, books, free lessons or even free courses.
We are teachers from all over the world, UK, USA, Germany, France, Australia, Canada, Vietnam living for long time in Vietnam and working with young people, teaching different subjects.
This should be seen as our volunteer job.
20% premined ( around 20M coins) are kept by our group of teachers to give away to the students and for marketting. We are still looking for a developer of the android wallet.


P.S.
We are not programmer and we try to keep coin costs low.
Any suggestions and help are welcome.






EducoinV is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 2.5 minute block targets
 - subsidy halves in 840k blocks (~4 years)
 - ~99 million total coins

The rest is the same as Bitcoin.
 - 50 coins per block
 - 576 blocks to retarget difficulty - 1 day

For more information, as well as an immediately useable, binary version of
the EducoinV client software.

Blockexplorer: http://blockexplorer.viet-systems.com
Miningpool   : http://miningpool.viet-systems.com
Node         : node.viet-system.com





License
-------

EducoinV is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the EducoinV
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/vietmarek/educoinv_v2/tags) are created
regularly to indicate new official, stable release versions of EducoinV.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./educoinv-qt_test

