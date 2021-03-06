datavetenskap.nu_
################

Welcome to the repository containing the webpage of Computer Scientists at Uppsala University.

Installation
============

.. code-block:: bash

    $ git clone git@github.com:uppsaladatavetare/datavetenskap.nu.git
    $ cd datavetenskap.nu
    $ virtualenv env
    $ . env/bin/activate
    $ pip install -r requirements.txt

Recompile upon modification and serve locally (the site should 
be available at http://localhost:8000):

.. code-block:: bash

    $ make devserver

When you are done, stop the server:

.. code-block:: bash

    $ make stopserver


How do I contribute?
====================

1. Fork this repositry.
2. Clone your fork: ``git clone git@github.com:YOUR_USERNAME/datavetenskap.nu.git``
3. Create a new branch: ``git checkout -b some-improvement``
4. Create a reStructuredText_ file with your own content:

   - Blog posts at ``content/blog/YEAR/MONTH-DAY-SLUG.rst``
   - Articles at ``content/article/SLUG.rst``

5. Commit the changes. 
6. Push the changes to your fork.
7. Create a pull request and set the target branch to ``origin/master``.
8. Await approval from one of the members of `@uppsaladatavetare/website-managers`_.

As soon the managers have reviewed and merged your contribution, it will
appear on the website.

Why not just use WordPress?
===========================

WordPress is a cool piece of software, but is a bit of an overkill for our
simple site that is basically static. What we do here instead is to store all
the content in form of text files (in reStructuredText_) and transform them
into a static webpage using Pelican_. The main advantage of this approach is
that we now get a site that anyone can easily contribute to using Git.


.. _Pelican: http://docs.getpelican.com/en/stable/
.. _Python: http://www.python.org/
.. _datavetenskap.nu: http://www.datavetenskap.nu/
.. _reStructuredText: http://docutils.sourceforge.net/rst.html
.. _`@uppsaladatavetare/website-managers`: https://github.com/orgs/uppsaladatavetare/teams/website-managers
