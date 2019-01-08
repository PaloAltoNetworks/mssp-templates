
Global Protect Cloud Service (GPCS) Templates
=============================================

The configuration snippet descriptions and the associated GitHub repository link for each xml snippet.

The GPCS templates are provided for 3 deployment needs:

    + Initial infrastructure setup configuration

    + Addition of remote branch sites

    + sample IPSEC tunnel configurations for select CPE vendors


The templates are incremental to and reference the iron-skillet day one configurations. The details of the iron-skillet
templates can be found at:

|skilletpanoramatemplates|.

The metadata.yaml files in each configuration directory contain:

    + list of variables and default values

    + load order including the xpaths and snippet file names


.. Note::
    GPCS can only be configured using Panorama. Therefore no PAN-OS only templates are provided.


Core Service Setup
------------------

----------------------------------------------------------------------

This section shows the configuration elements to automate the addition of a new GPCS cloud service instance.

 (coming soon)

Core Setup
~~~~~~~~~~

:panoramarepo:`gpcs/something.xml`


Remote Network using IPSEC
--------------------------

----------------------------------------------------------------------

This configuration uses the Panorama API interface to configure the 3 elements requires for a new remote site:

    + IKE gateway

    + IPSEC tunnel

    + GPCS plug-in elements


IKE Gateway
~~~~~~~~~~~

:panoramarepo:`gpcs_remote/ike_gateway.xml`


A simple reference IKE gateway configuration reference by the IPSEC tunnel.

    + include NAT traversal

    + simple passphrase connectivity

(have team help with a starter config)


IPSEC Tunnel
~~~~~~~~~~~~

:panoramarepo:`gpcs_remote/ipsec_tunnel.xml`


A simple reference IPSEC tunnel configuration using the IKE gateway and reference in the GPCS plug-in.


(have team help with a starter config)


GPCS Plug-In Onboarding Configuration
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

:panoramarepo:`gpcs_remote/onboarding.xml`


Onboarding elements for a new remote site including:

    + IPSEC tunnel

    + remote subnet

    + tunnel connect site selection

    + bandwidth for remote site connectivity


(have team help with a starter config)


GPCS CPE Tunnel Configuration
-----------------------------

:panoramarepo:`gpcs/cpe_configs`


Provides reference configurations for CPE vendor products that will connect back to GPCS

.. Note::
    These are sample reference configurations only and not supported by Palo Alto Networks


(work in progress to include)


