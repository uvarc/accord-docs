User Guide
======================

.. contents::

.. toctree::
   :maxdepth: 2


Access
--------

Request Access
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
User onboarding is a multi-step process:

1. A PI self-registers using an online form.

.. raw:: html

    <button class="btn-accord">Request Access</button>

2. If the PI is from an institution that is new to ACCORD, an MOU/contract with your institution and UVA will need to be established.
3. Once that is in place, or for subsequent PIs, the project application will be reviewed and approved/declined.
4. Once approved a user will confirm their email and complete additional profile registration steps.
5. When registration is complete the user will be notified by email. They can then create a project.


Create a Project
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Principal Investigators (PIs) can create a new, empty project using the ACCORD Console. This action
triggers three processes behind the scenes:

1. Creates a new system group with the PI as both a member and owner.
2. Creates a new 1TB project storage share within ACCORD cluster storage.
3. Creates a new home directory for the PI within that project storage.

PIs may suspend a project at any time using the console. Project data is stored for ~6 months and then
automatically removed. Suspended projects can be reinstated by request before this time.

.. raw:: html

    <button class="btn-accord">Create/Manage a Project</button>


Add Team Members
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Once additional researchers have requested access to ACCORD and have been approved (following the onboarding
steps above), the owner of a project can add those individuals to their project. The PI can add additional 
users at any time, and may also remove users as needed.

Because user authentication is handled through single sign-on from each user's home institution, PIs should
be aware of the ``eppn`` for their colleagues. An ``eppn`` looks similar to most institutional email
addresses, in the form of ``userid`` + ``domain``, such as ``mst3k@mit.edu`` or ``abc5y@virginia.edu``.


Transfer Data
-------------------
asldkfjsldkfjsdlfkjsdflksdj lksdj flksdj f


Manage Environments
-------------------------

Create an Environment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
From the ACCORD console, select the project you want to work with. Next select an environment template
from the list of environments. Your container should be running within a few seconds and will appear
under "Running Environments" on the same page.

To learn more about your choices of environment, see `Environments <environments.html>`_

View the status of an environment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Check the "Running Environments" section of the ACCORD console. This will tell you the type of environment,
when you created it, how long it has been running, and how to connect to or terminate it.


Connect to an Environment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Once you have created an environment, the console will display all of your running environments. Click on 
the "CONNECT" button for the appropriate environment and a new browser tab will open directly to your 
endpoint.


Terminate an environment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Using the "Running Environments" section of the ACCORD console, find the environment you wish to terminate.
On the far right will be a red "Terminate" button. Clicking this will stop and destroy your environment.
Note that your files and storage are never terminated or destroyed in this process. Any special session information
or data read into memory will be lost, however.

Terminated environments cannot be recovered. However, they can be replicated (see below).

Replicate an environment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
To replicate or repeat an environment you used before, scroll down on the ACCORD console to see a list of
environments you have run before. Click the orange "Run" button next to an environment you want to reuse.


Software Requirements
-------------------------

- A modern web browser such as Chrome, Firefox, Safari, or Edge.
- Install and register OPSWAT, a posture-checking client.

.. raw:: html

    <button class="btn-accord">Learn more about OPSWAT</button>

- Create and install an authentication certificate.

.. raw:: html

    <button class="btn-accord">Create a Certificate</button>
