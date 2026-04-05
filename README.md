✅ SMALL OFFICE NETWORK DESIGN
Enterprise-Level Simulation in Cisco Packet Tracer

📘 Project Overview
A secure and scalable small office network built with VLAN segmentation, /26 subnetting, inter-VLAN routing, DHCP, SSH, and ACL.
Status: ✅ Completed | 🔄 Open for Improvements

🎯 Objectives

VLAN segmentation for 3 departments (Admin, IT, Guest)
Efficient IP utilization using subnetting
Inter-VLAN routing with controlled access
Automatic IP assignment (DHCP)
Secure remote access (SSH)
Guest VLAN restricted from Admin VLAN (ACL)


🗺️ Network Topology
text[ Router ]
              |
          [ Switch ]
         /   |   \
     Admin  IT  Guest
      PCs   PCs   PCs
Router-on-a-Stick configuration.

🗂️ VLAN Configuration

























VLAN IDNameDepartment10ADMINAdmin20ITIT30GUESTGuest

🌐 IP Addressing Scheme (/26 Subnetting)



































VLANSubnetGatewayUsable Range10192.168.1.0/26192.168.1.1192.168.1.1 – 192.168.1.6220192.168.1.64/26192.168.1.65192.168.1.65 – 192.168.1.12630192.168.1.128/26192.168.1.129192.168.1.129 – 192.168.1.190–192.168.1.192/26–Reserved for Future Use

⚙️ Technologies Used

VLAN + Trunk (802.1Q)
Router-on-a-Stick
DHCP Server
SSH + RSA Keys
Extended ACL
Subnetting (/26)


🧪 Testing Results

























TestResultAdmin ↔ IT communication✅ SuccessGuest → Admin access❌ BlockedDHCP IP assignment✅ WorkingSSH remote login✅ Working

📸 Screenshots
(Add your Packet Tracer screenshots here: topology, VLANs, router config, DHCP, ping tests)

🚀 How to Run

Open Cisco Packet Tracer
Load the .pkt file
Verify VLANs, router subinterfaces & DHCP pools
Test with ping


📈 Future Improvements

NAT for internet access
Layer 3 switching
STP + EtherChannel redundancy
Advanced firewall


Prepared by:
Mesay Fey
Aspiring Network Engineer
Date: April 2026
