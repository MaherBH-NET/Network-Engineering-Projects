# 🏢 Enterprise Network Recovery & Security Hardening

## 📘 Overview
This self-made project simulates the design and configuration of a **secure and resilient enterprise network** for a company recovering from an internal outage.  
It focuses on VLAN segmentation, inter-VLAN routing, link redundancy, secure management, and network backup strategies — representing a full small-to-medium business (SMB) network scenario.

---

## ⚙️ Tools Used
- Cisco Packet Tracer  
- Cisco IOS CLI  

---

## 🧩 Network Design Summary
The network consists of **five switches and one router**, segmented by department using VLANs.  
Each department has its own subnet, managed through a **router-on-a-stick** setup.

### VLAN Layout
| VLAN ID | Department / Purpose | Subnet | Example IP Range |
|----------|----------------------|---------|------------------|
| 99 | Management | 10.10.99.0/24 | 10.10.99.2–254 |
| 2 | Senior Engineering | 10.10.2.0/24 | 10.10.2.2–254 |
| 3 | Business Team | 10.10.3.0/24 | 10.10.3.2–254 |
| 4 | Video Editors | 10.10.4.0/24 | 10.10.4.2–254 |
| 5 | Marketing | 10.10.5.0/24 | 10.10.5.2–254 |
| 6 | Social Media | 10.10.6.0/24 | 10.10.6.2–254 |
| 7 | Team Leads | 10.10.7.0/24 | 10.10.7.2–254 |
| 8 | Software Engineers | 10.10.8.0/24 | 10.10.8.2–254 |
| 10 | HR | 10.10.10.0/24 | 10.10.10.2–254 |
| 11 | Meeting Rooms | 10.10.11.0/24 | 10.10.11.2–254 |
| 12 | Vendors & Investors | 10.10.12.0/24 | 10.10.12.2–254 |

---

## 🔐 Key Implementations

### 1️⃣ VLAN Segmentation & Trunking
- Each floor/department assigned to a dedicated VLAN  
- Trunk links between switches using **EtherChannel (LACP)** for redundancy and scalability  

### 2️⃣ Inter-VLAN Routing
- Implemented **Router-on-a-Stick** configuration on R1  
- Subinterfaces created for all VLANs with IP helper addresses for DHCP relay  

### 3️⃣ Secure Management
- SSH-enabled remote access  
- Encrypted local user authentication  
- MOTD banners and disabled unneeded services  

### 4️⃣ Backup & Recovery
- Configured **TFTP server** for automatic configuration and IOS backups from all network devices  

### 5️⃣ DHCP Services
- Centralized DHCP server providing address pools for each VLAN via relay agents on R1  

---

## 🧠 Skills Demonstrated
- Enterprise-level VLAN planning and subnetting  
- EtherChannel (LACP) for link aggregation  
- Router-on-a-stick inter-VLAN routing  
- SSH and encryption configuration  
- DHCP relay and centralized management  
- IOS and config backup automation  

---

## 🏁 Outcome
This project recreates a realistic enterprise environment emphasizing **resilience, security, and manageability**.  
It reflects the full process of recovering and securing a network after an outage — from infrastructure rebuilding to access hardening and disaster recovery.

---

## 📂 Files Included
- `Enterprise-Network-Recovery-and-Security-Hardening.pkt`
