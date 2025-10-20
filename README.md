# 🏢 Inter-Office Network Connectivity using Cisco Packet Tracer

## 📘 Project Overview
This project demonstrates the design and simulation of a **two-office enterprise network** using **Cisco Packet Tracer**.  
The goal is to establish communication between two geographically separate offices — **Head Office** and **Branch Office** — through routers connected via a **Wide Area Network (WAN)** link.  

The project highlights fundamental **network design, IP addressing, and routing concepts**, enabling devices in both offices to communicate effectively.

---

## 🎯 Objective
To design and configure a **secure and efficient inter-office communication network** using Cisco Packet Tracer by:
- Creating two separate LANs for Head Office and Branch Office.
- Connecting them via a WAN link using routers.
- Implementing routing to enable cross-office communication.
- Testing connectivity and packet transfer between PCs.

---

## 🖥️ Tools & Technologies Used
- **Cisco Packet Tracer** (Network simulation and configuration)
- **Routers and Switches**
- **End Devices (PCs)**
- **WAN and LAN Connections**

---

## 🧩 Network Design Overview

### 🏢 Office 1 – Head Office
| Device | IP Address | Description |
|--------|-------------|--------------|
| Router (R1) | 192.168.1.1 | LAN Gateway |
| PC0 | 192.168.1.2 | Workstation |
| PC1 | 192.168.1.3 | Workstation |
| Network | 192.168.1.0/24 | Head Office LAN |

---

### 🏢 Office 2 – Branch Office
| Device | IP Address | Description |
|--------|-------------|--------------|
| Router (R2) | 192.168.2.1 | LAN Gateway |
| PC2 | 192.168.2.2 | Workstation |
| PC3 | 192.168.2.3 | Workstation |
| Network | 192.168.2.0/24 | Branch Office LAN |

---

### 🌐 WAN Connection (Between Routers)
| Interface | Router | IP Address |
|------------|---------|------------|
| Serial0/0/0 | R1 | 10.0.0.1 |
| Serial0/0/0 | R2 | 10.0.0.2 |

Routing Protocol Used: **Static Routing / RIP**

---

## ⚙️ Configuration Steps

1. **Assign IP addresses** to all PCs and router interfaces.  
2. **Connect LAN devices** (PCs and switches) using copper straight-through cables.  
3. **Connect routers** using a serial cable to establish the WAN link.  
4. **Configure static routes** (or RIP) on both routers to enable communication between networks.  
5. **Test connectivity** using the `ping` command from one office to another.  
6. **Use “Add Simple PDU”** tool to visualize packet movement between devices.

---

## 📶 Working Explanation

- Each office acts as an independent **Local Area Network (LAN)**.  
- The routers connect both LANs through a **WAN link**.  
- When a PC in Office 1 sends a message to Office 2, data packets travel:
  1. From PC → Switch → Router (R1)  
  2. Across the WAN → Router (R2)  
  3. To destination Switch → PC  
- Routing tables in routers ensure data reaches the correct destination network.

---

## ✅ Output / Results

- **Successful ping replies** between PCs from different offices.  
- **Packet delivery simulation** using “Add Simple PDU” tool shows proper flow across routers and switches.  
- Demonstrates a **real-world enterprise inter-branch network** with proper routing and connectivity.

---

## 🧠 Learning Outcomes

- Understanding of LAN and WAN configuration.  
- Static and dynamic routing setup.  
- IP addressing and subnetting concepts.  
- Data flow visualization using PDUs in Cisco Packet Tracer.

---

## 📂 Project File
You can open the project file in Cisco Packet Tracer:


---

## 🚀 How to Run the Project

1. Open **Cisco Packet Tracer**.  
2. Go to **File → Open**, and load the `.pkt` file.  
3. Check IP configurations of PCs and routers.  
4. Test the network by:
   - Pinging devices between offices.
   - Using the **Add Simple PDU** tool for packet transmission.
5. Switch to **Simulation Mode** to observe packet flow.

---

## 🏁 Conclusion
This project successfully simulates **inter-office connectivity** using Cisco networking devices. It represents a **real-world scenario** where two corporate branches communicate securely and efficiently using **routers, switches, and proper routing protocols** in Cisco Packet Tracer.

---

## 👨‍💻 Author
**Manju Setty**  
*Dayananda Sagar College of Engineering*  
B.E. – Artificial Intelligence and Machine Learning  

