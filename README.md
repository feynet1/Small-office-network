
# 📘 Small Office Network Design

## 🚀 Project Overview

This project demonstrates the design and implementation of a **secure and scalable small office network** using:

* VLAN Segmentation
* Subnetting
* Inter-VLAN Routing
* Core Network Services

The network is designed and simulated using **Cisco Packet Tracer**, following real-world enterprise networking practices.

---

## 🎯 Objectives

* Design a structured network for multiple departments
* Implement VLAN segmentation for security and efficiency
* Apply subnetting to optimize IP address usage
* Enable inter-VLAN communication
* Configure DHCP for automatic IP assignment
* Secure the network using SSH and ACL

---

## 🏢 Network Scenario

A small office environment with three departments:

* 👨‍💼 **Admin**
* 💻 **IT**
* 📶 **Guest**

Each department is logically separated using VLANs while maintaining controlled communication between networks.

---

## 🗺️ Network Topology

```
        [ Router ]
            |
        [ Switch ]
        /    |    \
   Admin    IT   Guest
    PCs     PCs    PCs
```

---

## 🗂️ VLAN Configuration

| VLAN ID | Name  | Department |
| ------- | ----- | ---------- |
| 10      | ADMIN | Admin      |
| 20      | IT    | IT         |
| 30      | GUEST | Guest      |

---

## 🌐 IP Addressing Scheme (/26 Subnetting)

| VLAN | Subnet           | Gateway       | Usable Range                  |
| ---- | ---------------- | ------------- | ----------------------------- |
| 10   | 192.168.1.0/26   | 192.168.1.1   | 192.168.1.1 – 192.168.1.62    |
| 20   | 192.168.1.64/26  | 192.168.1.65  | 192.168.1.65 – 192.168.1.126  |
| 30   | 192.168.1.128/26 | 192.168.1.129 | 192.168.1.129 – 192.168.1.190 |
| —    | 192.168.1.192/26 | Reserved      | Future Expansion              |

---

## ⚙️ Technologies Used

* VLAN (Virtual LAN)
* Inter-VLAN Routing (Router-on-a-Stick)
* DHCP (Dynamic Host Configuration Protocol)
* SSH (Secure Shell)
* ACL (Access Control List)
* Subnetting (/26)

---

## 🔧 Configuration Highlights

### 🔹 VLAN Segmentation

* Logical separation of departments
* Improved security and traffic management

### 🔹 Inter-VLAN Routing

* Communication between VLANs via router subinterfaces

### 🔹 DHCP

* Automatic IP assignment for all VLANs

### 🔹 SSH Security

* Secure remote access to the router

### 🔹 ACL Implementation

* Guest VLAN is restricted from accessing Admin VLAN

---

## 🔐 Security Features

* VLAN isolation
* Access Control Lists (ACL)
* SSH encrypted access

---

## 🧪 Testing & Verification

| Test Scenario            | Result       |
| ------------------------ | ------------ |
| Admin ↔ IT communication | ✅ Successful |
| Guest → Admin access     | ❌ Blocked    |
| DHCP IP assignment       | ✅ Working    |
| SSH remote login         | ✅ Working    |

---


## 🚀 How to Run This Project

1. Open **Cisco Packet Tracer**

2. Load the `.pkt` file

3. Verify configurations:

   * VLANs
   * Router subinterfaces
   * DHCP pools

4. Test connectivity:

```
ping <destination-ip>
```

---

## 📈 Future Improvements

* Implement NAT for internet access
* Add firewall rules
* Upgrade to Layer 3 switching
* Add redundancy (STP, EtherChannel)

---

## 💡 Key Learning Outcomes

* Practical VLAN and subnetting implementation
* Network segmentation and security
* Real-world routing configuration
* Troubleshooting connectivity issues

