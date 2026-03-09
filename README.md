# 🌐 Internet Networking CA-2 – Enterprise Network Infrastructure Design

![Topology](https://img.shields.io/badge/Network-Hybrid%20Topology-green?style=for-the-badge)
![Routing](https://img.shields.io/badge/Routing-Dynamic%20Routing-orange?style=for-the-badge)
![RIP](https://img.shields.io/badge/Protocol-RIP-red?style=for-the-badge)
![IPv4](https://img.shields.io/badge/IP-IPv4-purple?style=for-the-badge)

This project presents the **design and implementation of a network infrastructure for a five-floor office building at SSL Securities**. The objective is to create a **scalable, efficient, and fault-tolerant enterprise network** using a structured **hybrid topology**, **dynamic routing**, and **VLSM-based IP addressing**.

The design ensures **optimized network performance, efficient IP utilization, and seamless communication between departments across all floors**.

---

# 📌 Table of Contents

- Introduction  
- Network Architecture  
- Network Topology  
- IP Addressing Scheme  
- Server Placement  
- Routing Strategy  
- Connectivity Testing  
- Network Devices  
- Project Components  
- Innovations Implemented  
- Future Enhancements  
- Author  
- License  

---

# 📖 Introduction

Modern enterprise networks require **high reliability, scalability, and efficient resource utilization**.  

This project focuses on designing a **multi-floor office network** for SSL Securities that supports:

- Seamless inter-floor communication  
- Efficient IP address allocation  
- Reliable routing between departments  
- Expandability for future networking technologies

The implementation integrates **dynamic routing using RIP** and **Variable Length Subnet Masking (VLSM)** to optimize both performance and network management.

---

# 🏢 Network Architecture

The office building consists of **five floors**, each representing different organizational departments connected through switches and routers.

The architecture includes:

- End-user workstations
- Network switches
- Inter-floor routers
- Centralized servers
- Structured subnet allocation

Each floor operates as an individual **LAN segment**, while routers provide communication between these LANs.

---

# 🔗 Network Topology

A **hybrid topology** is implemented to balance **simplicity, reliability, and scalability**.

### Floors 1–4: Bus Topology
- Provides simple network structure
- Efficient for departmental communication
- Reduced infrastructure complexity

### Floor 5: Mesh Topology
- Direct connections between devices
- Provides **maximum fault tolerance**
- Ensures alternative data paths in case of link failure

### Router Interconnection
Routers are strategically interconnected to allow **efficient routing across floors** while maintaining redundancy and flexibility.

---

# 🌍 IP Addressing Scheme

The network uses a **VLSM-based IPv4 addressing strategy** to maximize address utilization and support varying device requirements across floors.

### Floors 1–2
- Assigned **Class A Public IPv4 addresses**
- Supports connectivity with external networks

### Floors 3–5
- Assigned **Class A Private IPv4 addresses**
- Optimized for secure internal communication

### VLSM Implementation
- Subnets allocated according to floor requirements
- Efficient IP address utilization
- Defined **subnetwork address, host range, and broadcast address** for each floor

---

# 🖥 Server Placement

To support enterprise services, servers are strategically distributed across different floors:

| Server | Location | Purpose |
|------|------|------|
| DNS Server | Floor 1 | Domain name resolution for the entire network |
| DHCP Server | Floor 2 | Automatic IP assignment to network devices |
| FTP Server | Floor 3 | File transfer services |
| Email Server | Floor 5 | Corporate email communication |
| HTTP Server | Floor 5 | Internal web services |

This distribution improves **network efficiency and service accessibility**.

---

# 🔀 Routing Strategy

The network uses **Dynamic Routing** through the **Routing Information Protocol (RIP)**.

### Key Characteristics

- Automatic route discovery
- Adaptive route updates
- Reduced manual configuration
- Improved scalability

### Network Routing Setup

- **4 routers** deployed to connect different floors
- Each floor has a **default gateway**
- Gateways correspond to the **first usable IP address of each subnet**

Dynamic routing ensures that **route updates occur automatically when network conditions change**.

---

# 📡 Connectivity Testing

Connectivity was validated through **extensive ping tests** across devices located on different floors.

Testing confirmed:

- Successful **inter-floor communication**
- Proper **routing table updates**
- No packet loss during transmission
- Stable network performance

These results confirm the **correctness and reliability of the network design**.

---

# 🖧 Network Devices

The following network devices are used in the architecture:

### Switches
- Installed on each floor
- Connect end-user devices within the LAN

### Routers
- Interconnect different floors
- Manage routing between subnetworks

### Access Points
- Reserved for future **wireless network expansion**

---

# 📂 Project Components

The project repository includes:

- **Network Topology Diagram**  
  Detailed visual representation of the entire office network.

- **Router Configuration Files**  
  Configuration scripts implementing RIP dynamic routing.

- **Network Design Documentation**  
  Explanation of topology, addressing scheme, and routing logic.

---

# 💡 Innovations Implemented

### VLSM Optimization
Efficient IP address allocation based on the number of hosts required per floor.

### Future-Proof Design
Network structure prepared for **VLAN integration and wireless networking expansion**.

### Dynamic Fault Recovery
RIP enables automatic route recalculation in case of link or router failure.

---

# 🚀 Future Enhancements

Potential improvements for the network include:

- Implementing **VLAN segmentation** for improved network security
- Adding **Load Balancers** to distribute traffic across servers
- Deploying **Wireless Access Points** for BYOD environments
- Upgrading to **RIP v2** for classless routing and improved convergence
- Implementing **network monitoring systems**

---

# 👤 Author

**Ayushman Behera**

🎓 B.Tech – Computer Science & Engineering (Data Science)  
🏫 Lovely Professional University  

🔗 GitHub: https://github.com/ayubeh1513  
📧 Email: ayushmanbehera689@gmail.com

---

# 📄 License

This project is licensed under the **MIT License**.
