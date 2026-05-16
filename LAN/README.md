# Enterprise Campus Network Topology – Cisco Packet Tracer

## Overview

This project is a complete enterprise campus network topology designed and implemented in Cisco Packet Tracer using the hierarchical network model (Core, Distribution, and Access layers).

The goal of this project was to simulate a real enterprise infrastructure while focusing on:

* Scalability
* Redundancy
* High availability
* Secure management
* Network segmentation
* Dynamic routing
* Enterprise security practices

The topology integrates routing, switching, wireless networking, VoIP, redundancy protocols, and network services into a single enterprise design.

---

# Network Architecture

## 1. Core Layer

The Core Layer provides fast and reliable transport between distribution switches.

### Implemented Features

* Layer 3 switching
* Routed links
* EtherChannel aggregation
* LACP configuration
* High-speed backbone connectivity

### Purpose

* Fast packet forwarding
* Redundant paths
* Reliable connectivity between network sections

---

## 2. Distribution Layer

The Distribution Layer acts as the boundary between the core and access layers.

### Implemented Features

* Inter-VLAN routing using SVIs
* HSRP gateway redundancy
* Rapid PVST+
* OSPF routing
* ACL implementation
* DHCP relay (`ip helper-address`)
* SSH management
* VLAN trunking

### Purpose

* Policy enforcement
* VLAN routing
* Traffic control
* Redundancy and failover

---

## 3. Access Layer

The Access Layer connects end-user devices to the network.

### Implemented Features

* VLAN assignment
* Access and trunk ports
* Port Security
* PortFast
* Voice VLANs
* SSH configuration
* Disabled unused ports
* Authentication and accounting

### Connected Devices

* PCs and laptops
* Smartphones
* Cisco IP Phones
* Wireless clients

---

# VLAN Structure

| VLAN     | Purpose         |
| -------- | --------------- |
| VLAN 10  | HR              |
| VLAN 20  | IT              |
| VLAN 30  | AI Department   |
| VLAN 50  | Servers         |
| VLAN 99  | Management      |
| VLAN 100 | Voice           |
| VLAN 150 | Cisco IP Phones |

---

# Routing Protocols

## OSPF

Used for dynamic routing between Layer 3 devices.

### Configurations Included

* OSPF neighbor establishment
* Route advertisement
* Inter-network communication

---

## EIGRP

EIGRP concepts and redistribution were also explored within the topology design.

---

# Redundancy & High Availability

## HSRP

Configured to provide gateway redundancy for VLANs.

### Features

* Active/Standby gateway
* Preemption
* Reduced downtime during failure

---

## EtherChannel

Implemented using LACP.

### Benefits

* Increased bandwidth
* Link redundancy
* Load balancing

---

## Rapid PVST+

Configured to prevent Layer 2 loops and optimize traffic paths.

### Features

* STP root bridge placement
* Faster convergence
* VLAN load balancing

---

# Security Features

## ACLs

Applied to control communication between VLANs.

### Objectives

* Restrict unauthorized access
* Improve network segmentation
* Protect sensitive VLANs

---

## Secure Management

* SSH enabled on routers and switches
* Management VLAN implementation
* Local authentication configuration

---

## Access Layer Security

* Port Security
* Disabled unused interfaces
* Controlled VLAN access

---

# Wireless Infrastructure

## Wireless LAN Controller

Configured to manage Lightweight Access Points.

## Lightweight Access Points

Used to provide wireless connectivity to clients within the enterprise environment.

---

# VoIP Integration

## Cisco IP Phones

Integrated into the topology using dedicated Voice VLANs.

### Features

* Voice traffic separation
* Improved QoS structure
* IP Telephony simulation

---

# Network Services

The topology includes multiple enterprise services:

| Service      | Function                         |
| ------------ | -------------------------------- |
| DHCP         | Automatic IP assignment          |
| DNS          | Name resolution                  |
| AAA          | Authentication and authorization |
| Gmail Server | Mail service simulation          |

---

# Skills Demonstrated

* Enterprise Network Design
* Routing & Switching
* VLAN Segmentation
* Dynamic Routing
* HSRP Configuration
* EtherChannel & LACP
* STP Optimization
* ACL Security
* SSH Management
* Wireless Networking
* VoIP Integration
* Network Troubleshooting

---

# Troubleshooting Performed

During implementation, several networking issues were analyzed and resolved, including:

* STP convergence issues
* VLAN trunking problems
* Routing adjacency failures
* HSRP failover testing
* ACL communication restrictions
* Inter-VLAN connectivity problems

---

# Tools & Technologies

* Cisco Packet Tracer
* Cisco Routers
* Cisco Layer 2 & Layer 3 Switches
* Wireless LAN Controller
* Lightweight Access Points
* OSPF
* EIGRP
* HSRP
* EtherChannel
* VLANs
* ACLs
* SSH

---

# Author

Nouran Mohamed

