# University Network Simulation Project (Cisco Packet Tracer)

## Project Overview

This project demonstrates a scalable and secure university network architecture, designed and simulated using **Cisco Packet Tracer**. The network replicates a real-world academic infrastructure divided into **Main Campus** and **Branch Campus**, with multiple departments segmented using **VLANs** and interconnected via **Layer 3 routing**. The setup includes DHCP, ACLs, and wireless device integration to ensure efficient communication, IP address management, and security enforcement.

---

## Campus Structure

### 🔷 Main Campus

Consists of **three buildings**: A, B, and C.

- **Building A:**
  - VLAN 10: Admin Department – Full network access
  - VLAN 20: HR Department – Secure employee records handling
  - VLAN 30: Finance Department – Highly secure financial operations
  - VLAN 40: Business Department – Academic/business resources

- **Building B:**
  - VLAN 50: Electronics and Computer Department – Technical lab network
  - VLAN 60: Arts and Design – Multimedia and creative access

- **Building C:**
  - VLAN 70: Student Lab – Controlled student workspace
  - VLAN 80: IT Department – Backbone support and full-access control

### 🔷 Branch Campus

Consists of **one building**: Honors and Science

- VLAN 90: Staff – Admin/Academic operations
- VLAN 100: Student Library – Shared academic resources with limited internet access

---

## Technologies Used

- **Cisco Packet Tracer** – Network design and simulation
- **VLANs** – Logical segmentation of departments
- **Inter-VLAN Routing (L3 Switch)** – Controlled communication across VLANs
- **DHCP** – Dynamic IP address assignment per VLAN
- **ACLs** – Security through access restriction
- **RIPv2** – Routing protocol for simplicity and simulation
- **Wireless Integration** – Devices connected with appropriate access control

---

## Key Features

- 🔐 **Departmental Isolation** via VLANs  
- 🌐 **Controlled Inter-VLAN Communication** using ACLs  
- ⚙️ **Dynamic IP Assignment** through DHCP pools  
- 📶 **Wireless Access Points** configured per use case  
- 🛡️ **Security Policies** applied to block unauthorized access  
- 🔄 **RIPv2 Routing** ensures communication between campuses

---

## Configuration Highlights

### VLAN Configuration
```bash
vlan 10
name ADMIN
exit
...
switchport access vlan 10
