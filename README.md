# Palo Alto Networks MSSP templates

The templates are provided for MSSP repeatable services such as simple
Internet gateway or GPCS remote network access.

Configurations can be loaded into the Panorama management platform or direct
to the firewall.

### Documentation

More details about the templates can be found at:

[MSSP template docs](https://mssp-templates.readthedocs.io)


### Dependency on the Iron-Skillet Day One Configuration

The templates are not stand-alone and instead work as a complement to the
Iron-Skillet day one configurations. Included are security objects, security policies,
logging and reporting samples, dynamic updates, and general device hardening.

For more information and the loadable Iron-Skillet templates go to:

[Iron-Skillet template repo on Github](https://github.com/PaloAltoNetworks/iron-skillet)



### Quick Start for Internet Gateway

For users wanting to explore the internet gateway templates using a firewall GUI can
load the configuration with CLI `set` commands. These are found in internet_gateway/panos/set_commands.

**NOTE:** before loading the configuration, first load the iron-skillet PAN-OS configuration.




