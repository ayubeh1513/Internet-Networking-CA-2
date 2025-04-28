# Internet Networking CA-2

## Overview
This project outlines the **network infrastructure** for a **five-floor office building** at **SSL Securities**, ensuring efficient communication, scalability, and fault tolerance. The network is designed using a **hybrid topology approach**, dynamic routing for inter-floor communication, and a structured **IP addressing scheme** based on **VLSM**.

## Network Topology
The office network follows a **hybrid topology model** to balance performance, scalability, and fault tolerance:
- **Floors 1-4:** Bus topology, providing straightforward setup and efficient data transmission for departmental needs.
- **Floor 5:** Mesh topology, delivering maximum fault tolerance with direct interconnections between all network devices.
- **Router Connectivity:** Routers are interconnected to maintain seamless communication across floors with redundancy considerations.

## IP Addressing Scheme
- **Floors 1-2:** Assigned **Class A Public IPv4 addresses**, ensuring broad connectivity with external networks.
- **Floors 3-5:** Assigned **Class A Private IPv4 addresses**, optimizing internal communication and security.
- **VLSM (Variable Length Subnet Masking):** Implemented to optimize IP address utilization for each floor based on actual requirements.
- Each floor is allocated a unique subnet with properly assigned **subnetwork address**, **host IP range**, and **broadcast address**.

## Server Placement
- **DNS Server:** Deployed on Floor 1 to handle domain name resolution for the entire enterprise.
- **DHCP Server:** Installed on Floor 2 for automatic IP assignment across devices.
- **FTP Server:** Installed on Floor 3 to manage file transfers efficiently.
- **Email & HTTP Servers:** Configured on Floor 5 to manage corporate communications and web services.

## Routing Strategy
- **Dynamic Routing** is implemented using the **RIP (Routing Information Protocol)** to enable scalable and adaptable inter-floor communication.
- **Routers Used:** A total of **4 routers** are deployed to connect different floors efficiently while minimizing complexity.
- **Default Gateways:** Defined separately for each floor, aligned with the first usable IP address in each subnet.
- **Interdepartment Communication:** Designed to be seamless through dynamic route updates and router interconnections.

## Connectivity Testing
- Conducted extensive **ping tests** between all floors to verify proper inter-LAN and inter-floor communication.
- Successful results confirm that packets traverse the network efficiently without packet loss or delays.

## Network Devices and Placement
- **Switches:** Used on each floor to connect end devices.
- **Routers:** Strategically placed to interconnect floors.
- **Access Points:** Planned for future wireless expansion, currently reserved for enhancements.

## Project Files
- **Network Diagram:** Complete labeled topology showcasing server placement, routers, and end devices.
- **Configuration Scripts:** Router configuration for RIP dynamic routing and basic switch configurations (to be added if required).

## Innovations Implemented
- **VLSM Optimization:** Applied to save IP address space and enhance network manageability.
- **Future-Proof Design:** Structured with scope for easy VLAN implementation and wireless network integration.
- **Dynamic Fault Recovery:** Through RIP, enabling dynamic updates in case of route failure, enhancing network resilience.

## Future Enhancements
- Implementing **VLAN segmentation** for better network security and broadcast control.
- Introducing **Load Balancers** to optimize traffic management across servers.
- Adding **Wireless Access Points** for BYOD (Bring Your Own Device) environments.
- Upgrading to **RIP v2** for classless routing and more efficient network convergence.

## Contributors
- **Ayushman Behera** – Network Architecture, Design & Implementation

For any issues, suggestions, or contributions, feel free to open a pull request or raise an issue.
