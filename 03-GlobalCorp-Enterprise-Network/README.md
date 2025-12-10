# GlobalCorp Enterprise Network Simulation

A large-scale, multi-campus enterprise network designed in **Cisco Packet Tracer**.  
This project simulates two geographically separated campuses (HQ + R&D), connected over a WAN, implementing **enterprise-grade routing, redundancy, security, and services**.

---

## 🏢 Topology Overview
- **Campus A (HQ):** 5 floors, 4 access switches, 2 core L3 switches  
- **Campus B (R&D):** 3 floors, 3 access switches, 2 core L3 switches  
- **Internet Backbone:** 2 routers simulating ISP/core routes  
- **40+ devices total**

---

## 🔧 Technologies Implemented

### **Switching & VLANs**
- 18 VLANs per campus  
- 802.1Q trunking  
- EtherChannel (LACP) between core switches  
- Inter-VLAN routing via SVIs  

### **Routing & Redundancy**
- **EIGRP (AS 100):** dynamic routing across entire topology  
- **HSRP:** gateway redundancy and load balancing  
- Dual-path WAN connectivity  

### **Enterprise Services**
- Centralized **DHCP** for all VLANs  
- Secure **SSH v2** management  
- **TFTP** configuration backups  
- Layered campus design: Core → Distribution → Access  

---

## 🎯 Key Features
- **High Availability**: HSRP failover, EtherChannel link redundancy  
- **Security**: VLAN segmentation, SSH-only access, port security, native VLAN 999  
- **Cross-Campus Connectivity**: full routing between HQ and R&D  
- **Full Documentation**: addressing tables, VLAN map, configurations, testing screenshots  

---

## 📁 Project Structure

03-GlobalCorp-Enterprise-Network/
│
├── README.md
├── GlobalCorp_Final.pkt
│
├── Documentation/
│ ├── Network-Diagram.png
│ ├── IP-Addressing-Table.xlsx
│ └── VLAN-Assignments.pdf
│
├── Configurations/
│ ├── Routers/
│ ├── L3-Switches/
│ ├── L2-Switches/
│ └── Servers/
│
└── Screenshots/
├── EIGRP-Neighbors.png
├── HSRP-Status.png
├── DHCP-Leases.png
├── SSH-Connection.png
└── Ping-Tests.png

---

## 🧪 Testing & Verification
- ✔ Intra-VLAN & Inter-VLAN communication  
- ✔ Cross-campus connectivity  
- ✔ HSRP failover  
- ✔ EtherChannel link failure recovery  
- ✔ DHCP, SSH, and TFTP service validation  

---

## 🎓 Learning Outcomes
- Enterprise network architecture  
- EIGRP + HSRP configuration  
- Redundant campus designs  
- VLAN security & segmentation  
- Professional documentation and testing workflows  

---

*This is a self-made project designed to simulate a real enterprise environment using Cisco Packet Tracer.*


