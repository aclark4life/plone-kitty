Introduction
============

Feeling nostalgic for the early 2000s? Take some time out of your day to have some fun with Plone 1.

Installation
------------

Follow these steps::

    $ virtualenv-2.4 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Edit `buildout.cfg` to look like this:

    [buildout]
    extends = http://pythonpackages.com/buildout/plone/1.1.x-dev

Then::

    $ bin/buildout
    $ bin/supervisord

Usage
-----

Login as euser and reset admin's password. Logout and login as admin and create a Plone site. It will produce a traceback, at which point go to the ZMI and manually add a CMF ActionsIcon tool.

.. image:: https://github.com/aclark4life/plone_1_fun/raw/master/screenshot.png
