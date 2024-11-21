![Screenshot 2024-11-20 144114](https://github.com/user-attachments/assets/3c4902d0-e7b8-4b22-b396-70fd0fb372c4)


https://github.com/user-attachments/assets/cfe96d66-402d-430f-9690-617a6866eb58


This project involves designing and implementing a **VoIP-enabled network** for a newly acquired branch of Turtle Consultancy Limited. The company specializes in delivering IT infrastructure solutions to medium-sized organizations worldwide. With the expansion, a scalable and highly available network infrastructure is required to support the business demands and technological challenges.

---

## **Project Overview**

### **Requirements**
1. **IP Addressing**:
   - **Data Network**: 192.168.100.0/24
   - **Voice Network**: 172.16.100.0/24
   - **Router Connections**: 10.10.10.0/24
2. **Departments**:
   - **Finance**: 20 Phones, 20 PCs, and 1 Printer
   - **HR**: 20 Phones, 20 PCs, and 1 Printer
   - **Sales**: 20 Phones, 20 PCs, and 1 Printer
   - **ICT**: 20 Phones, 20 PCs, and 1 Printer
3. **VoIP Configuration**:
   - Use Cisco **2811 Routers** and **2960 Switches**.
   - Enable **VoIP** with dial numbers:
     - Finance (1xx)
     - HR (2xx)
     - Sales (3xx)
     - ICT (4xx)
   - Configure **dial-peering** for cross-department IP phone communication.

---

## **Network Design Specifications**

1. **Topology**:
   - Use **Packet Tracer** to design a network connecting three departments with centralized server-side resources.
   - Use **serial connections** between routers, straight-through cables for router-to-switch, switch-to-hosts, and phone-to-PC connections.

2. **Subnets**:
   - Each department will access **two subnetworks**: one for data and one for voice.
   - IP phones will reside in **VLAN 100**.

3. **Basic Settings**:
   - Set hostnames, console passwords, enable passwords, and banner messages.
   - Encrypt all passwords and disable IP domain lookup.

4. **Dynamic IP Allocation**:
   - **Data**: Use a centralized DHCP server.
   - **Voice**: Use routers as DHCP servers.

5. **VLAN Configuration**:
   - Each department will have separate VLANs for **data** and **voice**.
   - Use **Inter-VLAN Routing** (router-on-a-stick) with subinterfaces.

6. **Routing**:
   - Use **OSPF** as the dynamic routing protocol for route advertisements.

7. **Remote Access**:
   - Configure **SSH** for secure remote management.

8. **VoIP Configuration**:
   - Enable **VoIP services** and assign dial numbers by department.
   - Configure **dial-peering** for inter-department IP phone communication.

9. **Testing**:
   - Test and verify communication between all devices to ensure full functionality.

---

## **Technologies Implemented**

- **Network Topology Design** using Cisco Packet Tracer.
- **Hierarchical Network Design**.
- Proper cabling and connectivity for networking devices.
- Basic device configurations (hostnames, passwords, banners, etc.).
- VLAN creation and port assignments for **data** and **voice** networks.
- Subnetting and IP addressing.
- **Inter-VLAN Routing** using router-on-a-stick.
- Centralized DHCP server configuration for **data** network.
- Router-based DHCP configuration for **voice** network.
- **SSH Configuration** for secure remote access.
- **OSPF Configuration** for routing protocol.
- **VoIP/Telephony Services** configuration on routers.
- Dial-peering setup for inter-department IP phone communication.
- Host device configurations (PCs, phones, and printers).
- Comprehensive testing and verification of network communication.

---

## **Final Network Design**
The network design supports scalability and high availability with features such as:
1. Separate VLANs for data and voice traffic.
2. Dynamic IP allocation for efficient device management.
3. Secure remote access via SSH.
4. Seamless routing using OSPF for interdepartmental communication.
5. VoIP-enabled communication across departments with dial numbers.
