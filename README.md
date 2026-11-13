# Enterprise Network Redundancy and VLAN Routing

## Project Overview

This project demonstrates the design and implementation of a redundant enterprise network using **Cisco Packet Tracer**. It focuses on Layer 2 switching, VLAN segmentation, centralized VLAN management, Layer 3 inter-VLAN routing, link aggregation, and network loop prevention.

The network is designed to improve network organization, communication between different VLANs, bandwidth utilization, and redundancy through multiple interconnected switches.

## Technologies & Protocols

- Cisco Packet Tracer
- Virtual LANs (VLANs)
- VLAN Trunking Protocol (VTP)
- IEEE 802.1Q Trunking
- Inter-VLAN Routing using SVIs
- LACP EtherChannel
- Spanning Tree Protocol (STP)
- Cisco IOS Configuration
- IPv4 Addressing and Subnetting

## Network Features

### 1. VLAN Segmentation
- Created multiple VLANs to logically separate network departments.
- Assigned access ports to their respective VLANs.
- Configured trunk links to carry multiple VLANs between switches.

### 2. VLAN Trunking Protocol (VTP)
- Configured a multilayer switch as the VTP Server.
- Configured access switches as VTP Clients.
- Implemented consistent VTP domain and password settings.
- Verified VLAN propagation across switches.

### 3. Inter-VLAN Routing
- Configured Switched Virtual Interfaces (SVIs) on the multilayer switch.
- Assigned gateway IP addresses to each VLAN.
- Enabled IP routing for communication between different VLANs.

### 4. LACP EtherChannel
- Configured EtherChannel using Link Aggregation Control Protocol (LACP).
- Bundled multiple physical links into logical port-channel interfaces.
- Tested connectivity after disconnecting a physical member link.

### 5. Spanning Tree Protocol (STP)
- Verified STP operation and root bridge election.
- Observed port states and topology changes.
- Tested network behavior during link failures.

## Network Verification

The following commands were used to verify network configurations and operation:

```bash
show vlan brief
show vtp status
show interfaces trunk
show etherchannel summary
show spanning-tree
show ip interface brief
show ip route
show running-config
ping <destination-ip>
```

## Project Files

```text
Enterprise-Network-Redundancy-and-VLAN-Routing/
│
├── README.md
├── Enterprise-Network-Redundancy-and-VLAN-Routing.pkt
│
└── screenshots
```

## Learning Outcomes

- Practical experience with enterprise switching configurations.
- Understanding VLAN segmentation and trunking.
- Implementing centralized VLAN management using VTP.
- Configuring Layer 3 routing using SVIs.
- Understanding link aggregation and redundancy using LACP.
- Analyzing STP behavior and preventing Layer 2 switching loops.
- Performing network connectivity testing and troubleshooting.

## Tools Used

**Cisco Packet Tracer | Cisco IOS CLI**

[Download Enterprise Network Packet Tracer File (.pkt)](./Enterprise-Network-Redundancy-and-VLAN-Routing.pkt)

[View All Project Screenshots](./screenshots/)

## Author

**Lakshmi Dissanayake**

This project represents practical learning and hands-on implementation of enterprise networking concepts.
