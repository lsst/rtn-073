.. image:: https://img.shields.io/badge/rtn--073-lsst.io-brightgreen.svg
   :target: https://rtn-073.lsst.io
.. image:: https://github.com/lsst/rtn-073/workflows/CI/badge.svg
   :target: https://github.com/lsst/rtn-073/actions/

################################################################
Rules of Engagement for Accessing Data During the Embargo Period
################################################################

RTN-073
=======

Data must be embargoed after arriving at the USDF - for 30 days in commissioning and 80 hrs in Survey Operations. Alert Processing will not record vetoed streaks. What rules will we impose on accessing data during that period?

**Links:**

- Publication URL: https://rtn-073.lsst.io
- Alternative editions: https://rtn-073.lsst.io/v
- GitHub repository: https://github.com/lsst/rtn-073
- Build system: https://github.com/lsst/rtn-073/actions/


Build this technical note
=========================

You can clone this repository and build the technote locally if your system has Python 3.11 or later:

.. code-block:: bash

   git clone https://github.com/lsst/rtn-073
   cd rtn-073
   make init
   make html

Repeat the ``make html`` command to rebuild the technote after making changes.
If you need to delete any intermediate files for a clean build, run ``make clean``.

The built technote is located at ``_build/html/index.html``.

Publishing changes to the web
=============================

This technote is published to https://rtn-073.lsst.io whenever you push changes to the ``main`` branch on GitHub.
When you push changes to a another branch, a preview of the technote is published to https://rtn-073.lsst.io/v.

Editing this technical note
===========================

The main content of this technote is in ``index.rst`` (a reStructuredText file).
Metadata and configuration is in the ``technote.toml`` file.
For guidance on creating content and information about specifying metadata and configuration, see the Documenteer documentation: https://documenteer.lsst.io/technotes.
