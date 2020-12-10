Security
==========
ACCORD can meet HIPAA, FERPA, and other less-restrictive data sensitivity requirements. 
More restrictive levels, such as CUI, FISMA, PCI cannot be satisfied. A list of compliance
will be released as the platform nears production launch.

.. image:: ../_static/images/security.png
   :alt: Security
   :align: right

Authentication
--------------

ACCORD makes use of InCommon authentication, a federated SAML-based standard used by most institutions of 
higher education in the U.S. This means that ACCORD does not have its own user identity store but instead 
relies upon authentication via your home institution's single sign-on tool.


Encryption
----------

All connectivity to ACCORD environments is encrypted using SSL certificates over HTTPS. 
Plain-text (unencrypted) access is prohibited. 

Data at rest is also encrypted within ACCORD storage systems.

Isolation
---------

ACCORD environments cannot, by design, have any access to other environments -- including storage, 
network connectivity, or data. Environments run within isolated Kubernetes pods and their (overlyay)
network connectivity is isolated and encrypted. The cluster control plane is also encrypted for management
and requests.


Private Environment URLs
------------------------

**[TO-DO]** When you request an ACCORD environment, a unique HTTPS endpoint is created for you and 
*can only be used by you*. That URL will look something like:

.. code-block:: html
   
   https://jupyter-notebook-1a2b3c4d5e-mst3k.uvarc.io/


These environments cannot be shared.

Using certificate authentication from your browser (something you will set up the first time you use 
ACCORD and will renew annually), the platform verifies that you, and only you, access that environment. 
If you want to collaborate with a co-investigator, they can simply create an identical environment 
within the same project!

