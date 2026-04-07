📘 Small Office Network Design (Enterprise-Level)
🚀 Project Overview

This project demonstrates the design and implementation of a secure and scalable small office network using VLAN segmentation, subnetting, and essential network services.

The network is built and simulated using Cisco Packet Tracer, following real-world networking practices.

🎯 Objectives
Design a structured network for multiple departments
Implement VLAN segmentation for security and efficiency
Apply subnetting to optimize IP address usage
Enable inter-VLAN communication
Configure DHCP for automatic IP assignment
Secure the network using SSH and ACL
🏢 Network Scenario

A small office environment with three departments:

👨‍💼 Admin
💻 IT
📶 Guest

Each department is isolated using VLANs while maintaining controlled communication.

🗺️ Network Topology
           [ Router ]
               |
           [ Switch ]
        /      |      \
    Admin     IT     Guest
     PCs      PCs      PCs
🗂️ VLAN Configuration
VLAN ID	Name	Department
10	ADMIN	Admin
20	IT	IT
30	GUEST	Guest
🌐 IP Addressing Scheme (Subnetting /26)

The network 192.168.1.0/24 is subnetted into four /26 subnets:

VLAN	Subnet	Gateway	Usable Range
10	192.168.1.0/26	192.168.1.1	192.168.1.1 – 192.168.1.62
20	192.168.1.64/26	192.168.1.65	192.168.1.65 – 192.168.1.126
30	192.168.1.128/26	192.168.1.129	192.168.1.129 – 192.168.1.190
—	192.168.1.192/26	Reserved	Future use
⚙️ Technologies Used
VLAN (Virtual LAN)
Inter-VLAN Routing (Router-on-a-Stick)
DHCP (Dynamic Host Configuration Protocol)
SSH (Secure Shell)
ACL (Access Control List)
Subnetting (/26)
🔧 Configuration Highlights
🔹 VLAN Segmentation
Logical separation of departments
Improved security and traffic management
🔹 Inter-VLAN Routing
Enabled communication between VLANs via router subinterfaces
🔹 DHCP
Automatic IP assignment for all VLANs
🔹 SSH Security
Secure remote access to the router
🔹 ACL Implementation
Guest VLAN is restricted from accessing Admin VLAN
🔐 Security Features
VLAN isolation
Access Control Lists (ACL)
SSH encrypted access
🧪 Testing & Verification
Test Scenario	Result
Admin ↔ IT communication	✅ Successful
Guest → Admin access	❌ Blocked
DHCP IP assignment	✅ Working
SSH remote login	✅ Working
📸 Screenshots

(Add your screenshots here)

Network topology
VLAN configuration
Router configuration
DHCP assignment
Ping tests (success & failure)
🚀 How to Run This Project
Open Cisco Packet Tracer
Load the .pkt file
Verify configurations:
VLANs
Router subinterfaces
DHCP pools

Test connectivity using:

ping <destination-ip>
📈 Future Improvements
Implement NAT for internet access
Add firewall rules
Upgrade to Layer 3 switch
Add redundancy (STP, EtherChannel)
💡 Key Learning Outcomes
Practical VLAN and subnetting implementation
Network segmentation and security
Real-world routing configuration
Troubleshooting connectivity issues
👨‍💻 Author

Mesay Fey
Aspiring Network Engineer

⭐ Project Status

✅ Completed
🔄 Open for improvements
