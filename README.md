# Company System Network Design 
---

## 📌 Project Overview

This project simulates a secure and scalable enterprise network for a trading floor support center using Cisco Packet Tracer. A hierarchical three-tier topology with VLANs, OSPF, DHCP, NAT/PAT, and security features like SSH and ACLs ensures smooth communication, redundancy, and future scalability.

---

## 🧩 Features

- **3-Tier Hierarchical Design**  
  Core, Distribution, and Access layers for scalability and efficient traffic flow.  

- **High Availability**  
  Dual ISPs, dual routers, and multilayer switches for redundancy and failover.  

- **VLAN Segmentation**  
  Separate VLANs for Sales, HR, Finance, Admin, and ICT with inter-VLAN routing.  

- **Dynamic IP Management**  
  DHCP server for automated IP assignment; static IPs for critical servers.  

- **Dynamic Routing**  
  OSPF protocol for optimized routing and fault tolerance.  

- **Security Features**  
  - SSH for secure remote administration  
  - NAT/PAT for safe internet connectivity  
  - ACLs & Port Security for controlled access  
 

---

## 🗺️ Network Topology Highlights

- **Core Layer:** Two redundant routers and multilayer switches with backup links  
- **Distribution Layer:** VLAN-based departmental switches for Sales, HR, Finance, Admin, and ICT  
- **Access Layer:** End-user devices and Cisco APs for wired and wireless connectivity  
- **Servers:** DNS and HTTP servers hosted in Server VLAN (60) with static IPs  
- **DHCP Server:** Provides dynamic IP allocation for client devices  

---

## 💻 IP Configuration

**Base Network:** `192.168.0.0/22`

| Link              | Network Address | Subnet Mask       | IP Range               | Broadcast Address |
|-------------------|-----------------|-------------------|------------------------|------------------|
| Core R1 – MLTSW1  | 10.10.10.0      | 255.255.255.252   | 10.10.10.1 – 10.10.10.2 | 10.10.10.3  |
| Core R1 – MLTSW2  | 10.10.10.4      | 255.255.255.252   | 10.10.10.5 – 10.10.10.6 | 10.10.10.7  |
| Core R2 – MLTSW1  | 10.10.10.8      | 255.255.255.252   | 10.10.10.9 – 10.10.10.10 | 10.10.10.11 |
| Core R2 – MLTSW2  | 10.10.10.12     | 255.255.255.252   | 10.10.10.13 – 10.10.10.14 | 10.10.10.15 |

---

## 🛡️ Security Features

- **VLAN Isolation** for departmental segmentation  
- **ACLs** to regulate inter-department communication  
- **SSH** for encrypted administrator logins  
- **NAT/PAT** to secure internal addresses from direct internet exposure  
- **Redundant Links** for fault tolerance and reliability  

---

## ✅ Testing & Results

- **ICMP Ping Tests** – Verified connectivity across all VLANs and devices  
- **Traceroute** – Validated OSPF routing across the network  
- **DHCP Allocation** – Successfully assigned IP addresses dynamically

---

## 📚 Conclusion

The **Company System Network Design** project successfully models a **robust, secure, and scalable enterprise network**. With configurations validated in Cisco Packet Tracer, the system ensures reliable communication, secure segmentation, redundancy, and readiness for future technological integration.

---


