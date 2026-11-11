# Cisco-Packet-Tracer-LAN-Creation-and-IPv4-Configuration

## Project Overview

This project involved designing and configuring a Local Area Network (LAN) for a fictional branch office using Cisco Packet Tracer. The objective was to establish connectivity between multiple end devices, configure IPv4 addressing, verify local and external network connectivity, and use command-line networking tools to inspect host configurations and network paths.

The activity provided practical experience with basic LAN setup, DHCP, static IP addressing, network troubleshooting, and connectivity verification.

## Objectives

- Connect network devices and end hosts to establish a functional LAN.
- Configure end devices with IPv4 addressing.
- Verify IP configurations and network connectivity.
- Use networking commands to retrieve host information and trace network routes.

## Network Setup

The simulated branch office network consisted of:

- 1 Office Router
- 1 Network Switch
- 2 End-user PCs (Admin and Manager)
- 1 Network Printer
- 1 Internet connection represented by a cloud
- 1 Remote Internet Server

**Topology:** A basic LAN connecting the two PCs and network printer through a central switch, with the switch connected to the office router. The router provides connectivity to the external network.

## Implementation

### 1. Physical Network Setup

- Powered on the end devices and office router.
- Connected the Admin PC, Manager PC, and printer to the office switch.
- Connected the office switch to the router.
- Established the router's connection to the internet cloud.
- Used copper straight-through Ethernet cables for the device connections.
- Verified physical connectivity through the link indicators in Packet Tracer.

### 2. IPv4 Address Configuration

Configured the end devices according to their addressing requirements.

**Dynamic IP Addressing (DHCP):**
- Configured the Admin PC to obtain its IPv4 configuration automatically through DHCP.
- Configured the Manager PC to obtain its IPv4 configuration automatically through DHCP.
- Verified that both PCs received their IP addresses, subnet masks, default gateway, and DNS server information.

**Static IP Addressing:**
- Manually configured the network printer's IPv4 address using the FastEthernet0 interface.
- Used a static address to ensure the printer remained accessible at a consistent network address.

**Network Addressing:**
- LAN Network: `192.168.1.0/24`
- Subnet Mask: `255.255.255.0`
- Address Assignment: DHCP for PCs; static IPv4 configuration for printer.

### 3. Connectivity Verification

Performed connectivity tests to confirm that the LAN was functioning correctly.

- Used the `ping` command from the Admin PC to test connectivity with the network printer.
- Repeated the connectivity test from the Manager PC.
- Verified successful responses, confirming communication between the PCs and printer.
- Accessed the remote internet server using its IP address through the PCs' web browsers.
- Repeated the test using the server's URL to verify DNS-based name resolution and external connectivity.

### 4. Network Information and Route Analysis

Used command-line networking utilities to examine host configurations and network paths.

**Commands executed:**

| Command | Purpose |
|---|---|
| `ipconfig` | Displays basic IP configuration, including IPv4 address, subnet mask, and default gateway. |
| `ipconfig /all` | Displays detailed network configuration, including DHCP, DNS, and physical adapter information. |
| `ping` | Tests connectivity between network devices using ICMP echo requests. |
| `tracert` | Identifies the network hops taken by packets travelling to a remote destination. |

Used `tracert` with the remote web server's URL to examine the route taken from the local PC to the external destination.

## Results

The activity was successfully completed.

- Established physical connectivity between the router, switch, PCs, and printer.
- Successfully configured DHCP on both PCs.
- Assigned a static IPv4 address to the network printer.
- Verified local network connectivity using ICMP ping tests.
- Successfully accessed the remote web server using both its IP address and URL.
- Examined host network configurations using `ipconfig` and `ipconfig /all`.
- Investigated the route to a remote destination using `tracert`.

## Skills Demonstrated

- Cisco Packet Tracer network simulation
- Basic LAN topology and device connectivity
- IPv4 addressing and subnet masks
- DHCP configuration and dynamic address assignment
- Static IP configuration
- Default gateway and DNS concepts
- ICMP and connectivity testing
- Network troubleshooting fundamentals
- Command-line network diagnostics
- Traceroute and network path analysis

## Tools Used

- Cisco Packet Tracer
- Command Prompt (Packet Tracer PC environment)

## Key Learning Outcomes

This activity strengthened my understanding of how devices communicate within a local network and how a LAN connects to external networks through a router.

It also provided practical exposure to the relationship between DHCP, static addressing, DNS, default gateways, and network connectivity testing. Using `ping`, `ipconfig`, and `tracert` helped develop familiarity with fundamental network administration and troubleshooting techniques.
