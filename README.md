# SOHOnetwork
3-departments SOHO network with DNS, DHCP, and HTTP servers 

# Cisco Packet Tracer - SOHO Network Project

## Overview This project simulates a Small Office / Home Office network using Cisco Packet Tracer. It features a centralized DHCP server managing multiple subnets, including a wired LAN and a wireless guest network.

## Topology

## Features

DHCP Relay: Configured IP helper-address on the router to forward DHCP requests to a central server.
DNS Server: Domain name system for HTTP test server
HTTP Server: Simulate the company's intranet

Network Segmentation:

Sales Department network: 192.168.10.0/24 (Gateway: .1)

HR Department network: 192.168.20.0/24 (Gateway: .1)

Test HTTP server : 192.168.30.2/24 (Gateway: .1)

## How to Run

1. Download SOHO_Network1.pkt.
2. Open in Cisco Packet Tracer (v8.2 or newer).
3. Toggle PCs to "DHCP" to verify automatic IP assignment.
4. Toggle Simulation Mode to visualize packet transportation.

## Screenshots
<h3>Network Overview</h3>
<img width="1247" height="678" alt="image" src="https://github.com/user-attachments/assets/568bb7d1-bf4a-40af-b801-e7529690c15d" />

<h3>DHCP setup</h3>
<img width="867" height="861" alt="image" src="https://github.com/user-attachments/assets/14c3fb03-6c17-41fc-9cce-ea249d38c0d4" />

<h3>Cross sub-network ping (ICMP) [Sales -> HR]</h3>
<img width="501" height="540" alt="image" src="https://github.com/user-attachments/assets/aace6d5e-da9a-4c49-9135-197a9d124afc" />

<h3>HTTP server access</h3>
<img width="1351" height="658" alt="image" src="https://github.com/user-attachments/assets/a206e88f-d41b-4f82-9859-a2ad89d06b25" />





