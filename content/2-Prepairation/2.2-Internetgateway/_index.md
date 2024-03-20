---
title : "Internet gateway"
date :  "`r Sys.Date()`" 
weight : 2
chapter : false
pre : " <b> 2.2 </b> "
---

## Internet Gateway

- **Default Network ACL:** After VPC initialization, a default network ACL is available and can be modified. By default, it grants access to all IPv4 or IPv6 traffic entering or leaving the VPC.

![VPC](/images/2-Prepairation/2.2-internetgateway/igw.png?featherlight=false&width=90pc)

## Network ACL Rules

You can manage rules for the default network ACL or create a new one for the VPC. Changes to the network ACL's rules automatically apply to its associated subnets.

Components of a network ACL rule:
- **Rule Number:** Rules are evaluated in sequence order, starting with the lowest number. Once a rule matches traffic, it's immediately applied even if it conflicts with higher-numbered rules.
- **Type:** Defines the traffic type (e.g., SSH). Specify traffic types or custom ranges.
- **Protocol:** Specify the protocol using standard protocol numbers.
- **Port Range:** Define the port or port range for traffic (e.g., HTTP is 80).
- **Source:** [Inbound Rule] Defines the traffic origin (CIDR range).
- **Destination:** [Outbound Rule] Specifies the traffic destination (CIDR range).
- **Allow/Deny:** Choose to Allow or Deny the specified traffic.

![VPC](../images/2-Prepairation/vps.png?featherlight=false&width=60pc)