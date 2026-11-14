# Multi-Campus Network Design & Configuration Using Cisco Packet Tracer

## Project Overview

This project demonstrates the design, configuration, and simulation of a multi-campus enterprise network infrastructure using **Cisco Packet Tracer**. Developed as part of the **CSE405 – Computer Networks** course at East West University, the project focuses on implementing an interconnected network environment capable of supporting communication across eight geographically distributed university campuses.

The network architecture incorporates multiple IP subnets, dynamic routing using **Open Shortest Path First (OSPF)**, centralized DHCP services, DNS resolution, HTTP web hosting, and wired and wireless connectivity.

The primary objective is to create a structured, manageable, and scalable network simulation that demonstrates fundamental enterprise networking principles and practical network administration techniques.

## Project Objectives

- Design a complete network topology connecting eight university campuses.
- Implement structured IP addressing and subnetting to separate campus networks.
- Configure OSPF dynamic routing to enable communication between different subnets.
- Establish centralized DHCP services for automatic IP address allocation.
- Implement DHCP relay using the `ip helper-address` command to support remote networks.
- Configure DNS services for domain name resolution.
- Deploy a centralized HTTP web server accessible from multiple campuses.
- Integrate wired and wireless network connectivity.
- Verify network communication using ICMP ping testing.

## Technologies and Tools

**Network Simulation:** Cisco Packet Tracer

**Routing Protocol:** OSPF (Open Shortest Path First)

**Networking Concepts:** TCP/IP, IP Addressing, Subnetting, LAN, WAN, Routing and Switching

**Network Services:** DHCP, DNS, HTTP

**Network Devices:** Routers, Cisco 2960 Switches, Wireless Access Points, PCs, Laptops, and Servers

**Configuration and Testing:** Cisco IOS CLI, DHCP Relay, ICMP Ping

## Network Architecture

The network consists of eight interconnected campus networks, each operating within its own IP subnet.

Routers provide inter-network connectivity, while switches connect end-user devices within individual campus LANs. Wireless access points extend connectivity to supported wireless devices.

OSPF dynamic routing is configured to facilitate communication between networks and automate route selection.

A separate server network provides centralized DHCP, DNS, and HTTP services, allowing devices from different campuses to access shared network resources.

### IP Addressing Scheme

The simulation uses the following campus network addresses:

| Campus | Network Address |
|---|---|
| Campus 1 | 10.0.0.0 |
| Campus 2 | 20.0.0.0 |
| Campus 3 | 30.0.0.0 |
| Campus 4 | 40.0.0.0 |
| Campus 5 | 50.0.0.0 |
| Campus 6 | 60.0.0.0 |
| Campus 7 | 70.0.0.0 |
| Campus 8 | 80.0.0.0 |

Additional networks are assigned for router-to-router communication and centralized server connectivity.

### Centralized Server Configuration

| Service | IP Address | Purpose |
|---|---|---|
| DNS Server | 129.1.1.10 | Domain name resolution |
| Web Server | 129.1.1.20 | University website hosting |
| DHCP Server | 129.1.1.30 | Automatic IP address allocation |

## Key Implementations

### 1. OSPF Dynamic Routing

Implemented OSPF routing to establish communication between multiple campus networks.

OSPF enables participating routers to exchange routing information and determine paths between interconnected networks without relying exclusively on manually configured static routes.

### 2. Centralized DHCP and DHCP Relay

Configured a centralized DHCP server to distribute IP addresses to client devices across multiple subnets.

Since DHCP requests are initially broadcast within local networks, the `ip helper-address` command is used on relevant router interfaces to forward client requests to the remote DHCP server.

This implementation demonstrates centralized IP address management in a routed network environment.

### 3. DNS Configuration

Configured a centralized DNS server to translate the university website's domain name into its corresponding web server IP address.

**Configured domain:** `abc.apex.edu.bd`

**Web server address:** `129.1.1.20`

This allows client devices to access the simulated university website using a human-readable domain name.

### 4. HTTP Web Server

Deployed an HTTP web server to host a basic university website using HTML.

The web service is accessible to clients from different campuses through the configured routing and DNS infrastructure.

### 5. Wired and Wireless Connectivity

Integrated switches and wireless access points to support communication between desktop computers, laptops, and other networked devices.

The architecture demonstrates both wired LAN connectivity and wireless access within the simulated campus environment.

## Network Testing and Validation

Network connectivity was evaluated using ICMP ping tests between devices located in different campus subnets.

According to the project testing report, the tested communication paths were successful, with zero packet loss observed during the documented tests.

These results demonstrate successful inter-subnet communication within the tested Cisco Packet Tracer simulation scenarios.

## Project Limitations

The project was developed in a simulated networking environment rather than deployed on physical enterprise networking equipment.

Some wireless devices occasionally associated with unintended access points, creating configuration inconsistencies.

Additionally, Cisco Packet Tracer does not reproduce every characteristic of physical networking devices or real-world wireless environments.

Advanced wireless configuration, network security controls, redundancy, and performance monitoring remain areas for future development.

## Future Improvements

Potential enhancements include:

- VLAN configuration and inter-VLAN routing.
- Access Control Lists (ACLs) for traffic filtering.
- Firewall integration and network segmentation.
- Network Address Translation (NAT).
- More advanced wireless access point configuration.
- Redundant network paths and failover testing.
- Network monitoring and performance analysis.
- Migration to private IP addressing for an enterprise-oriented deployment.

## Learning Outcomes

Through this project, I strengthened my understanding of network topology design, router configuration, dynamic routing, IP addressing, DHCP relay, DNS administration, web server integration, and network connectivity troubleshooting.

The project also provided practical experience using Cisco Packet Tracer to simulate interconnected networks and explore the fundamentals of enterprise network administration.

## Project Information

**Project:** Multi-Campus Network Design & Configuration

**Course:** CSE405 – Computer Networks

**Institution:** East West University, Dhaka, Bangladesh

**Semester:** Spring 2026

**Developed By:** Md Shadman Shakib Dip

**Project Type:** Academic Networking Project

**Simulation Platform:** Cisco Packet Tracer

## Conclusion

The project demonstrates a multi-campus networking environment that integrates dynamic routing, subnetting, centralized network services, and wired/wireless communication.

By combining OSPF, DHCP relay, DNS, and HTTP services, the simulation illustrates how multiple campus networks can communicate and share centralized resources.

This project reflects my practical interest in **Computer Networking, Network Administration, Network Infrastructure, and Network Security**, and serves as a foundation for further learning in enterprise networking and cybersecurity.
