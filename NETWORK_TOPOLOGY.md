# Network Topology Design

## Overview
This document outlines the network topology design for the Cisco LAN setup, detailing the various LAN segments, routers, switches, wireless access points, and the cloud firewall.

## LAN 1: Office Network
- **Purpose**: The primary network for office operations, supporting all internal services and employee devices.
- **Devices**:
  - Routers: 1 Main Router connecting to the internet.
  - Switches: Core Switch (Layer 3) for interconnecting devices and distribution.
  - Wireless Access Points: 3 APs strategically placed for full coverage.

## LAN 2: Guest Network
- **Purpose**: A separate, secure network for guests to access the internet without the ability to reach internal resources.
- **Devices**:
  - Routers: Isolated from the office LAN, connected to a secondary router.
  - Switches: 1 dedicated switch for guest devices.
  - Wireless Access Points: 2 APs dedicated to guest connectivity.

## LAN 3: IoT Network
- **Purpose**: Dedicated to Internet of Things devices to segregate them from office traffic for security.
- **Devices**:
  - Routers: Connected to the main router with firewall rules applied.
  - Switches: 1 switch for IoT devices.

## Network Devices
- **Routers**:
  - Main Router: Provides access to the internet and connects all LANs.
  - Secondary Router: Serves the guest network and isolates guest traffic.
- **Switches**:
  - Core Switch: Connects devices within the Office Network and routes traffic between VLANs.
  - Additional Switches: One for guest and one for IoT.
- **Wireless Access Points**: Placed across all LANs to provide Wi-Fi coverage.
- **Cloud Firewall**: Protects all networks from unauthorized access and monitors traffic.

## Diagram
![Network Diagram](link_to_diagram_image)

## Conclusion
The described network topology ensures efficiency, security, and proper segregation of network traffic among various user groups and device types. Further updates to this document will be made as the network evolves.