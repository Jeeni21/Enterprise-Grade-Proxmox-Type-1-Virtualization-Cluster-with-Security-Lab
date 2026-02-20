📌 Project Overview

This project demonstrates the design, deployment, and management of a 2-node Proxmox VE (Type-1 Hypervisor) cluster simulating an enterprise infrastructure environment.

The lab was built to simulate:

Enterprise virtualization architecture

Security monitoring & logging

Centralized storage

Domain-based authentication

Network segmentation

Infrastructure documentation and control validation

The cluster maintains quorum and operates in a distributed configuration.

🏗️ Architecture Overview
🧱 Cluster Configuration

Cluster Name: SecX

Nodes:

pve – 192.168.1.105

xds – 192.168.1.104

Quorum: Enabled

Total CPU Cores: 32

Total Memory: ~54GB

Total Storage: 1.34TB

Both nodes are online and synchronized.

💻 Virtual Machines Deployed
🔹 Infrastructure Services
VM ID	System	Purpose
100	Windows 11	Domain-joined endpoint testing
101	TrueNAS	Centralized storage
103	Security Testing VM	Adversary simulation & analysis
🔹 Security Stack

Wazuh (SIEM)

Elastic Stack

Suricata (IDS)

OPNSense Firewall

Zenarmor NGFW plugin

Tailscale Zero-Trust VPN

🔐 Security Capabilities Implemented

Centralized log ingestion

IDS log forwarding to SIEM

Endpoint monitoring agents

Network traffic inspection

VPN-secured remote management

Firewall rule documentation

Detection rule testing mapped to MITRE ATT&CK

Secure VM segmentation

🌐 Networking Design

Layered network segmentation

Static IP management

Firewall rule enforcement

Secure VPN overlay (WireGuard/Tailscale)

DNS filtering via AdGuard Home

📂 Storage Design

TrueNAS deployed for centralized storage

VM disk management via Proxmox storage pools

Logical separation between:

ISO storage

VM disks

Backup targets

📊 Monitoring & Resource Management

From the cluster dashboard:

CPU usage: ~1%

Memory usage: ~53%

Storage usage: ~20%

3 VMs running

Cluster quorum maintained

Monitoring performed via:

Proxmox dashboard

SIEM dashboards

System logs

Elastic/Kibana visualization

⚙️ Skills Demonstrated

Type-1 virtualization deployment

Cluster formation & quorum management

Linux system administration

Windows domain integration

Firewall configuration

IDS deployment

SIEM log pipeline creation

Secure remote access configuration

Infrastructure documentation

Security control validation
