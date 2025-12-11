# SOHOnetwork
2+1-departments SOHO network with DNS, DHCP, and HTTP servers 

# Cisco Packet Tracer - SOHO Network Project

## Overview 
This project simulates a Small Office / Home Office network using Cisco Packet Tracer. It features a centralized DHCP server managing multiple subnets, including a wired LAN and a wireless guest network.

## Topology
<img width="1247" height="678" alt="image" src="https://github.com/user-attachments/assets/568bb7d1-bf4a-40af-b801-e7529690c15d" />

## Features

* **DHCP Relay:** Configured `ip helper-address` on the router interfaces to forward broadcast DHCP requests across subnets to a centralized server.
* **DNS Server:** Implemented Domain Name System resolution to allow users to access the Intranet via domain name rather than IP.
* **HTTP Server:** Hosted a simulation of a company Intranet site for connectivity testing.
* **VLAN/Subnet Segmentation:** Separated traffic into logical departments for better management and security.

Network Segmentation:

The network is segmented into three distinct subnets handled by a central Gateway Router:

| Department | Network ID | Subnet Mask | Gateway |
| :--- | :--- | :--- | :--- |
| **Sales Dept** | `192.168.10.0` | `/24` | `.1` |
| **HR Dept** | `192.168.20.0` | `/24` | `.1` |
| **Server Farm** | `192.168.30.0` | `/24` | `.1` |

* **Test HTTP Server IP:** `192.168.30.2`
## How to Run

1.  **Download:** Get the `SOHO_Network1.pkt` file from this repository.
2.  **Launch:** Open the file in **Cisco Packet Tracer** (v8.2 or newer).
3.  **Verify DHCP:** Click any PC in Sales or HR, go to **Desktop > IP Configuration**, and toggle "DHCP" to confirm it receives an IP address automatically.
4.  **Test Connectivity:**
    * Open a PC's Web Browser and navigate to the server IP (or domain if configured).
    * Toggle **Simulation Mode** (Shift+S) to visualize the packet flow across the router.

## Screenshots
<h3>DHCP setup</h3>
<img width="867" height="861" alt="image" src="https://github.com/user-attachments/assets/14c3fb03-6c17-41fc-9cce-ea249d38c0d4" />

<h3>Cross sub-network ping (ICMP) [Sales -> HR]</h3>
<img width="501" height="540" alt="image" src="https://github.com/user-attachments/assets/aace6d5e-da9a-4c49-9135-197a9d124afc" />

<h3>HTTP server access</h3>
<img width="863" height="684" alt="image" src="https://github.com/user-attachments/assets/2832f2b7-d691-47ed-890c-945a88a68247" />






