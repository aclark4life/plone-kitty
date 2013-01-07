Introduction
============

Feeling nostalgic for the early 2000s? Take some time to run Plone 1!

.. image:: https://github.com/aclark4life/plone_1_fun/raw/master/screenshot.png

Installation
------------

Follow these steps::

    $ virtualenv-2.4 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Edit ``buildout.cfg`` to look like this::

    [buildout]
    extends = https://raw.github.com/pythonpackages/buildout-plone/master/1.1.x-dev

Then::

    $ bin/buildout
    $ bin/supervisord

Open http://localhost:8080/manage in your web browser and login with the credentials specified during installation (i.e. buildout). Create a Plone Site in the Zope Management Interface.

Heroku
~~~~~~

Now works on Heroku thanks to `Python Runtime Support <https://devcenter.heroku.com/articles/python-runtimes>`_.

Known issues
------------

- Creating a Plone Site in the ZMI will produce a traceback. To fix this, go to the ZMI and add a CMF ActionsIcon tool.
- It is in no way a good idea to use this in a production environment, it's just for fun.
