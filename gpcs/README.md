# The GlobalProtect Cloud Service (GPCS) template

 This template provides three configuration elements for Remote Network
 internet access:

 1. Baseline: initial service infrastructure, Device-group, and Template Stack configuration

 2. Remote Network: reference IKE and IPSEC configuration with site onboarding

 3. Reference CPE configuration snippets for IPSEC connectivity to GPCS

Included in the template configuration is the
[IronSkillet](https://github.com/PaloAltoNetworks/iron-skillet) day one configuration.


**NOTE:** This assumes the Panorama platform is operational with the GPCS
plugin installed and licensed.


### Optional: Gold MSSP Internet Gateway Rules

The .meta-cnc.yaml file includes the MSSP Internet gateway security rules
that can be loaded as part of the baseline configuration.

Based on template requirements, these rules can be commented out or deleted
from the .meta-cnc.yaml file. Additional, other security policies can be added
as required.