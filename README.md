# University Network Design  

## Project Overview  
This project is about designing a secure and efficient network for a university, covering two main locations and a separate server area. The goal is to ensure strong connectivity, security, and smooth communication between all departments.  

## Features  

### Network Segmentation  
I divided the network into multiple VLANs to improve security and manage traffic better.  

### Security Implementations  
- **Port Security** to prevent unauthorized devices from connecting.  
- **Disabled unused ports** to reduce security risks.  
- **ARP Snooping** and **DHCP Snooping** to stop spoofing attacks.  
- **DMZ (Demilitarized Zone)** to isolate and secure public-facing services.  
- **Access Control Lists (ACLs)** for better traffic filtering.  
- **PortFast and BPDU Guard** to enhance **Spanning Tree Protocol (STP)** and protect against loops.  
- **Site-to-Site VPN** to secure communication between both locations.  

### Connectivity Configurations  
- **DHCP** for automatic IP allocation.  
- **OSPF routing** to make inter-network communication more efficient and scalable.  

### High Availability and Redundancy  
- **Spanning Tree Protocol (STP)** using **Rapid PVST** mode to prevent network loops.  
- **HSRP (Hot Standby Router Protocol)** for backup and failover support.  

## Topology Diagram  
_(I'll add a network topology diagram here, showing VLANs, server placement, and connections.)_  

## Equipment and Tools  
- **Switches:** Cisco 2960 (or similar)  
- **Routers:** Cisco 1941 (or similar)  
- **Firewalls:** _(if applicable, I'll specify)_  
- **Simulation Tools:** Cisco Packet Tracer, GNS3  

## Implementation Details  
- **Network Segmentation:** Configured VLANs to keep department traffic separate.  
- **Security Configurations:** Applied port security, ACLs, DMZ, and VPN to enhance protection.  
- **Routing and Connectivity:** Used OSPF for dynamic routing and DHCP for easy IP management.  
- **High Availability:** Set up HSRP to provide backup and failover support.  
- **Spanning Tree Protocol:** Enabled Rapid PVST to improve network stability and prevent loops.  

## Challenges and Solutions  

### Challenge 1: Managing VLANs across multiple switches  
**Solution:** I used **VTP (VLAN Trunking Protocol)** to simplify VLAN management.  

### Challenge 2: Preventing loops in a complex topology  
**Solution:** I applied **Rapid PVST** and **BPDU Guard** to prevent loops and optimize STP.  

## How to Run the Simulation  
1. Open the **.pkt** or **.gns3** file in **Cisco Packet Tracer** or **GNS3**.  
2. Use the included configuration files and follow the testing instructions to explore the network.  

## Conclusion  
With this design, the university gets **secure, reliable, and scalable connectivity**. In the future, I might improve it by **adding wireless networks** and **exploring software-defined networking (SDN)** for even better performance.  
