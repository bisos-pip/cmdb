======================================================================================================================================
bisos.cmdb: Python Command-Services for BISOS's CMDB (Configuration Management DataBase) /DCIM (Data Center Infrastructure Management)
======================================================================================================================================

.. contents::
   :depth: 3
..

Overview
========

bisos.cmdb is a python package that uses the PyCS-Framework for NOTYET.
It is a BISOS-Capability and a Standalone-BISOS-Package.

*bisos.cmdb* is based on PyCS-Foundation and can be used both as a
Command and as a Service (invoke/perform model of remote operations)
using RPYC for central management of multiple systems.

.. _table-of-contents:

Table of Contents TOC
=====================

-  `Overview <#overview>`__
-  `Part of BISOS — ByStar Internet Services Operating
   System <#part-of-bisos-----bystar-internet-services-operating-system>`__
-  `bisos.cmdb is a Command Services (PyCS)
   Facility <#bisoscmdb-is-a-command-services-pycs-facility>`__
-  `Uses of bisos.cmdb <#uses-of-bisoscmdb>`__
-  `bisos.cmdb as a Standalone Piece of
   BISOS <#bisoscmdb-as-a-standalone-piece-of-bisos>`__
-  `Installation <#installation>`__

   -  `Installation With pip <#installation-with-pip>`__
   -  `Installation With pipx <#installation-with-pipx>`__

-  `Usage <#usage>`__

   -  `Locally (system command-line) <#locally-system-command-line>`__
   -  `Remotely (as a service –
      Performer+Invoker) <#remotely-as-a-service----performerinvoker>`__

      -  `Performer <#performer>`__
      -  `Invoker <#invoker>`__

   -  `Use by Python script <#use-by-python-script>`__

      -  `bisos.cmdb Source Code is in writen in COMEEGA (Collaborative
         Org-Mode Enhanced Emacs Generalized Authorship)
         – <#bisoscmdb-source-code-is-in-writen-in-comeega-collaborative-org-mode-enhanced-emacs-generalized-authorship----httpsgithubcombx-bleecomeega>`__\ https://github.com/bx-blee/comeega\ `. <#bisoscmdb-source-code-is-in-writen-in-comeega-collaborative-org-mode-enhanced-emacs-generalized-authorship----httpsgithubcombx-bleecomeega>`__
      -  `The primary API for bisos.cmdb is ./bisos/cmdb/cmdb-csu.py. It
         is self documented in
         COMEEGA. <#the-primary-api-for-bisoscmdb-is-bisoscmdbcmdb-csupy-it-is-self-documented-in-comeega>`__

-  `Documentation and Blee-Panels <#documentation-and-blee-panels>`__

   -  `bisos.cmdb Blee-Panels <#bisoscmdb-blee-panels>`__

-  `Support <#support>`__

Part of BISOS — ByStar Internet Services Operating System
=========================================================

| Layered on top of Debian, **BISOS**: (By\* Internet Services Operating
  System) is a unified and universal framework for developing both
  internet services and software-service continuums that use internet
  services. See `Bootstrapping ByStar, BISOS and
  Blee <https://github.com/bxGenesis/start>`__ for information about
  getting started with BISOS.
| **BISOS** is a foundation for **The Libre-Halaal ByStar Digital
  Ecosystem** which is described as a cure for losses of autonomy and
  privacy in a book titled: `Nature of
  Polyexistentials <https://github.com/bxplpc/120033>`__

*bisos.cmdb* is part of BISOS.

bisos.cmdb is a Command Services (PyCS) Facility
================================================

bisos.cmdb can be used locally on command-line or remotely as a service.
bisos.cmdb is a PyCS multi-unit command-service. PyCS is a framework
that converges developement of CLI and Services. PyCS is an alternative
to FastAPI, Typer and Click.

bisos.cmdb uses the PyCS Framework to:

#. Provide access to cmdb facilities through native python.
#. Provide local access to cmdb facilities on CLI.
#. Provide remote access to cmdb facilities through remote invocation of
   python Expection Complete Operations using
   `rpyc <https://github.com/tomerfiliba-org/rpyc>`__.
#. Provide remote access to cmdb facilities on CLI.

What is unique in the PyCS-Framework is that these four models are all a
single abstraction.

The core of PyCS-Framework is the *bisos.b* package (the
PyCS-Foundation). See https://github.com/bisos-pip/b for an overview.

Uses of bisos.cmdb
==================

Within BISOS, bisos.cmdb is used as a common facility.

bisos.cmdb as a Standalone Piece of BISOS
=========================================

bisos.cmdb is a standalone piece of BISOS. It can be used as a
self-contained Python package separate from BISOS. Follow the
installtion and usage instructions below for your own use.

Installation
============

The sources for the bisos.cmdb pip package is maintained at:
https://github.com/bisos-pip/cmdb.

The bisos.cmdb pip package is available at PYPI as
https://pypi.org/project/bisos.cmdb

You can install bisos.cmdb with pip or pipx.

Installation With pip
---------------------

If you need access to bisos.cmdb as a python module, you can install it
with pip:

.. code:: bash

   pip install bisos.cmdb

Installation With pipx
----------------------

If you only need access to bisos.cmdb as a command on command-line, you
can install it with pipx:

.. code:: bash

   pipx install bisos.cmdb

The following commands are made available:

-  cmdb.cs
-  roInv-cmdb.cs
-  roPerf-cmdb.cs

These are all one file with 3 names. *roInv-cmdb.cs* and
*roPerf-cmdb.cs* are sym-links to *cmdb.cs*

Usage
=====

Locally (system command-line)
-----------------------------

``cmdb.cs`` can be invoked directly as

.. code:: bash

   bin/cmdb.cs

Remotely (as a service – Performer+Invoker)
-------------------------------------------

You can also run

Performer
~~~~~~~~~

Run performer as:

.. code:: bash

   bin/roPerf-cmdb.cs

Invoker
~~~~~~~

Run invoker as:

.. code:: bash

   bin/roInv-cmdb.cs

Use by Python script
--------------------

bisos.cmdb Source Code is in writen in COMEEGA (Collaborative Org-Mode Enhanced Emacs Generalized Authorship) – https://github.com/bx-blee/comeega.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The primary API for bisos.cmdb is ./bisos/cmdb/cmdb-csu.py. It is self documented in COMEEGA.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Documentation and Blee-Panels
=============================

bisos.cmdb is part of ByStar Digital Ecosystem http://www.by-star.net.

This module's primary documentation is in the form of Blee-Panels.
Additional information is also available in:
http://www.by-star.net/PLPC/180047

bisos.cmdb Blee-Panels
----------------------

bisos.cmdb Blee-Panles are in ./panels directory. From within Blee and
BISOS these panles are accessible under the Blee "Panels" menu.

Support
=======

| For support, criticism, comments and questions; please contact the
  author/maintainer
| `Mohsen Banan <http://mohsen.1.banan.byname.net>`__ at:
  http://mohsen.1.banan.byname.net/contact
