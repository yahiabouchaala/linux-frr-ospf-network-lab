# Linux Router Lab with FRRouting (OSPF)

## 📌 Overview

This project demonstrates a multi-router network built using Linux virtual machines running **FRRouting (FRR)** to implement **OSPF dynamic routing**.

The lab simulates a real-world routed network with multiple routers and segmented LANs, enabling end-to-end communication between hosts across different subnets.

---

## 🖥️ Network Topology
<img width="1045" height="637" alt="Topology" src="https://github.com/user-attachments/assets/31c3f413-4e87-4835-baac-e592e3ef3071" />
---

## 🌐 Network Design
|------------------|-----------------------------|
| Network          |              Description    |
|------------------|-----------------------------|
| 192.168.10.0/24  | LAN1 (PC1 ↔ R1)             |
| 10.0.12.0/30     | Point-to-point link R1 ↔ R2 |
| 10.0.23.0/30     | Point-to-point link R2 ↔ R3 |
| 192.168.20.0/24  | LAN2 (R3 ↔ PC2)             |
|------------------|-----------------------------|

## ⚙️ Technologies Used

- Linux (Ubuntu)
- FRRouting (FRR)
- OSPF (Open Shortest Path First)
- VirtualBox
- Linux networking tools (`ip`, `netplan`)
- FRR CLI (`vtysh`)
- Packet analysis (`tcpdump`)

---

## 🔧 Configuration Highlights

- Configured **3 Linux routers** using FRRouting
- Established **OSPF adjacency (Area 0)** between routers
- Implemented **point-to-point /30 subnets**
- Enabled **IP forwarding on all routers**
- Configured **static IP addressing on hosts**
- Verified routing with dynamic route propagation

---
