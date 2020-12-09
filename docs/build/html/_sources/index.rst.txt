=====================
ACCORD
=====================

A Collaborative Computing Environment for Highly Sensitive Data

.. toctree::
   :maxdepth: 2
   :caption: Contents:
.. contents::


What is ACCORD?
===============

ACCORD is a collaboration between the public universities of Virginia to build and share cyberinfrastructure for research on highly sensitive data. Made possible by a grant from the National Science Foundation, ACCORD attempts to provide a service for institutions that may lack the financial, staffing, or technical resources to support such a platform. This project strives to be a repeatable model for other institutions across the United States.

ACCORD is project-based, which means that investigators request access to the platform, create a project and populate it with co-investigators, import data, and finally create and use disposable computing resources to perform their computational research.

Who can use ACCORD?
-------------------

lksjd flkjsd flksdj flksdj flksdjf lksdfj lskdfj sldkfj sdlkfj sdlfkj sdfl


How do I use ACCORD?
--------------------

ACCORD is entirely web-based, which means that the primary software you need is a good, modern browser such as Chrome, Firefox, or Safari. Once you have created a project, you will use the ACCORD Console to create an environment in which to do your work.

-----

Projects
========

.. image:: _static/images/projects.png
   :alt: Projects
   :align: right

The fundamental organizing unit for your work in ACCORD is a project. Within this platform, a project consists of:

(A) *Researchers* - a group of approved collaborators.
(B) *Data* - source and results data that you bring to the project. Data import/export is managed by Globus transfers.
(C) *Storage* - storage within the infrastructure dedicated to your project.
(D) *Computing Environments* - your choice from an approved library of web-based computing environments.

Researchers
-----------
Must enroll in the ACCORD platform and be approved for entrance into your project. Once co-investigators are onboarded into the platform, PIs can add them
to their project(s).

    <button>Invite a Co-Investigator</button>
    <button>Manage your Teams</button>

Data
------
Can be managed using the Globus federated GridFTP platform. The ACCORD DTN (data transfer node) address can be found once you sign into the ACCORD Console.

    <button>Open Globus</button>

Storage
----------
1TGB of storage will be allocated for each project by default. Additional storage can be purchased for a fee.

Computing Environemts
---------------------
Environments are containerized web interfaces created on-demand for you to use with your project data and code. Environments cannot span two projects at the same time.

    <button>Open the ACCORD Console</button>


-----

Environments
============

.. image:: _static/images/stacks-100.png
   :alt: Environments
   :align: right

Environments consist of web-based, containerized interfaces launched on-demand by researchers. Approved environemnts and details about them are below. 

- **Theia Python** - A rich IDE that allows researchers to manage their files and data, write code with an intelligent editor, and execute code within a terminal session.
- **Jupyter Notebok** - Allows for interactive, notebook-based analysis of data. A good choice for pulling quick results or refining your code.
- **RStudio** - The standard IDE for research using the R programming language. This environment is useful for generating plots and other R-based analysis.

These computing environments can be used for short-lived, interactive, computing and analysis OR you can kick off a longer, more intensive job to run for hours. For longer
runs, you may close your browser tab and return later, if so desired.

While ACCORD is not a BYOC (Bring Your Own Container) environment, we welcome your suggestions for additional containers to be considered in the future.

-----

Security
========

.. image:: _static/images/security.png
   :alt: Security
   :align: right

Authentication
--------------

ACCORD makes use of InCommon authentication, a federated SAML-based standard used by most institutions of higher education in the U.S. This means that ACCORD does not have its
own user identity store but instead relies upon authentication via your home institution's single sign-on tool.


Encryption
----------

All connectivity to ACCORD environments is encrypted using SSL certificates over HTTPS. Plain-text (unencrypted) access is prohibited. 


Isolation
---------

ACCORD environments cannot, by design, have any access to other environments -- including storage, network connectivity, or data. Environments run within isolated Kubernetes pods
and their network connectivity is isolated and encrypted.


Private Environment URLs
------------------------

**[TO-DO]** When you request an ACCORD environment, a unique HTTPS endpoint is created for you and *can only be used by you*. That URL will look something like:

.. code-block:: html
   
   https://jupyter-notebook-1a2b3c4d5e-mst3k.uvarc.io/


Using certificate authentication from your browser (something you will set up the first time you use ACCORD and will renew annually), the platform
verifies that you, and only you, access that environment. If you want to collaborate with a co-investigator, they can simply create an identical
environment within the same project!

-----

The ACCORD Team
===============

The ACCORD project was designed and built by the `Research Computing Group <https://www.rc.virginia.edu>`_ at the `University of Virginia <https://www.virginia.edu/>`_, under the coordination of the ACCORD Grant Project Manager
`Tho Nguyen <https://vpit.virginia.edu/tho>`_ (faculty, Computer Science) and `Ron Hutchins <https://vpit.virginia.edu/>`_, Vice Provost for Information Technology.
