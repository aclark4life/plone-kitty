
.. image:: https://github.com/aclark4life/plone_1_fun/raw/master/screenshot.png

Introduction
============

Feeling nostalgic for the early 2000s? Take some time out of your day to have
some fun with Plone 1.

Installation
============

Follow these steps::

    $ git clone git@github.com:aclark4life/plone_1_fun.git
    $ python2.4 bootstrap.py -d
    $ bin/supervisord

Now for some work-arounds::

    $ cd parts/zope2
    $ ../../bin/zopepy zpasswd.py -u euser -p euser access

Login as euser and reset admin's password. Logout and login as admin and
create a Plone site. It will produce a traceback, at which point go to the ZMI
and manually add a CMF ActionsIcon tool.

Enjoy!
