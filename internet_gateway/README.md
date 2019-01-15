# The Internet Gateway template

 This template snippet set is based on a simple two-zone model consisting
 of three service tiers aligned with device licensing:

 1. Gold: all subscriptions enabled (Threat, URL Filtering, Wildfire)

 2. Silver: Threat enabled without URL Filtering or Wildfire

 3. Bronze: No subscriptions enabled; basic firewall platform


 ### Network configuration

 * 2 Ethernet interfaces with associated trust/internet L3 zones

 * Internet Ethernet interface acts as DHCP client

 * Dynamic IP/port NAT using the public IP address


