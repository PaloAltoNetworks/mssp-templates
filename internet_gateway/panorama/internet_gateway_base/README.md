# Internet Gateway template base configuration

This set of snippets are loaded prior to the security tier selection.

The snippets included are:

* interface (template): interface elements loaded into the base template

* interface (stack): zone and additional elements at the stack level

* virtual router: sets of basic routing with a default-gateway to the internet

* zone: 2-zone model with internet and trust zones

* NAT: source-based port NAT mapping all users to a single public IP

* network profiles: management interface profile

The MSSP can edit/append as required for their specific deployments.

**NOTE**: The `vsys_imports` snippet is used to create a mapping
of interfaces, zones, and the virtual router. This element is managed by
the system when doing standard GUI/CLI edits yet required for a working
xml configuration.

