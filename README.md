# Network-Design-Implementation-and-documentation

This repository contains the Packet Tracer network design project for the Diploma in Cybersecurity and Digital Forensics at Temasek Polytechnic. The network design includes detailed configurations for HQ, Branch, and ISP routers, as well as a comprehensive VLSM IP addressing scheme, DHCP implementation, and security configurations.

## Table of Contents

- [Project Overview](#project-overview)
- [Network Design Components](#network-design-components)
- [VLSM IP Addressing Design](#vlsm-ip-addressing-design)
- [Router Configurations](#router-configurations)
- [DHCP Implementation](#dhcp-implementation)
- [NAT Configuration](#nat-configuration)
- [Security Measures](#security-measures)
- [Testing and Validation](#testing-and-validation)
- [Disadvantages and Suggested Improvements](#disadvantages-and-suggested-improvements)

## Project Overview

This project involves the design and configuration of a network for a hypothetical company with headquarters (HQ) and a branch office, both connected to the Internet via an ISP. The network is designed to meet specific requirements for IP addressing, security, and network performance.

## Network Design Components

- **HQ Router**: Configured to manage both internal and external networks, including NAT, static routes, and DHCP services.
- **Branch Router**: Similar to the HQ router, configured for branch network management, including NAT and DHCP.
- **ISP Router**: Manages the connection between the HQ and Branch routers to the Internet.
- **Firewall and Security Configurations**: Implemented at the HQ to ensure secure communication between internal and external networks.

## VLSM IP Addressing Design

The project uses Variable Length Subnet Masking (VLSM) to efficiently allocate IP addresses to different network segments. The key subnets include:

- **HQ Internal Private LAN**: 192.168.192.0/21
- **HQ DMZ LAN**: 192.168.202.0/25
- **Branch Internal Private LAN**: 192.168.200.0/23
- **WAN Connections**: Specific IP ranges are allocated for public WAN interfaces between routers.

## Router Configurations

Each router is configured with specific IP addresses, NAT settings, and security configurations. The configurations include interface setups, routing protocols, NAT, and access control lists (ACLs).

## DHCP Implementation

DHCP is implemented at both HQ and Branch routers to dynamically assign IP addresses to devices within the internal networks. Specific IP ranges are excluded for static assignments.

## NAT Configuration

Network Address Translation (NAT) is configured to allow internal devices to communicate with external networks using public IP addresses. The configurations include both static NAT for specific services and dynamic NAT for general traffic.

## Security Measures

Security configurations include setting up AAA for user authentication, enabling password encryption, setting up access control lists (ACLs), and configuring firewalls to protect internal networks from unauthorized access.

## Testing and Validation

Testing procedures include verifying connectivity between PCs and servers, ensuring DHCP is functioning correctly, and validating that NAT and security configurations are effectively securing the network.

## Disadvantages and Suggested Improvements

The current network design has some disadvantages, such as the use of public IP addresses within internal networks. Suggested improvements include transitioning to private IP addresses and implementing stricter security controls.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
