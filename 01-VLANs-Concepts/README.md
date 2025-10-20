# VLANs Concepts – Small Office Network

## 🧭 Overview
This project demonstrates VLAN segmentation, inter-VLAN routing using a Router-on-a-Stick configuration, DHCP relay, and NAT for Internet access in a small office environment.  
It’s designed to simulate a realistic multi-department setup with Admin, Sales, and IT VLANs connected to a central router and ISP.

---

## 🧩 Topology Summary
- **3 VLANs:**  
  - VLAN 10 – Admin – `192.168.10.0/24`  
  - VLAN 20 – Sales – `192.168.20.0/24`  
  - VLAN 30 – IT – `192.168.30.0/24`
- **Router R1:** Handles inter-VLAN routing and connects to ISP using NAT overload.  
- **Server:** Acts as a DHCP/DNS server for the VLANs (in VLAN 10).  
- **ISP Router:** Simulates external Internet connection.  

---

## ⚙️ Tools Used
- Cisco Packet Tracer  
- Cisco IOS CLI  

---

## 🧠 What I Built
- Created VLANs on two switches and configured trunk links.  
- Set up router subinterfaces for inter-VLAN routing.  
- Configured DHCP server and helper addresses for dynamic addressing.  
- Applied NAT for Internet access simulation.  
- Verified network connectivity and VLAN isolation.  

---

## 🧾 Key Verification Commands
- `show vlan brief`  
- `show interfaces trunk`  
- `show ip interface brief`  
- `show ip route`  
- `show ip nat translations`  
- `show ip dhcp binding`

---

## 🚀 Results
- All VLANs successfully communicated through router-on-a-stick.  
- DHCP and NAT operations verified.  
- Clients from all VLANs accessed simulated Internet through ISP router.  

---

## 🧩 Future Enhancements
- Implement ACLs between VLANs.  
- Add QoS for voice/data separation.  
- Integrate a small VoIP setup with CME on the router.
