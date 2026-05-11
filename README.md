Multi-Branch Secure Enterprise Network & Smart System Design

Project Overview
This project simulates a high-security, redundant, and mobile-integrated network infrastructure connecting **Istanbul (HQ)** and **Ankara (Branch)**. The design focuses on high availability, logical segmentation, and multi-layered security to ensure seamless business operations.



Technical Implementation Details

 1. High Availability & OSPF Routing
    
Dual-Link Redundancy: Istanbul and Ankara routers are connected via **dual physical links** to prevent a single point of failure. If one cable is disconnected, the secondary link takes over immediately.

Dynamic Routing:"OSPF" is configured to manage traffic between branches, ensuring fast convergence and automatic failover.

 2. VLAN Segmentation (VLAN 10, 20 & 99)
   
The network is segmented to isolate traffic and enhance security:

VLAN 10 & 20:Designated for different department users.
VLAN 99 (Management):A restricted network for administrative tasks.
Inter-VLAN Routing: Enabled to allow communication between these segments under controlled policies.

3. Admin PC & Access Control
   
Dedicated Management: A specific "Admin PC" is configured to manage the entire network infrastructure.

Security: Critical network devices are protected with "Username and Password" authentication. Management access is strictly limited to authorized personnel.

4. Wireless Connectivity & IoT Integration
   
Wireless Access Point:Established a secure Wi-Fi zone within the office.
Smartphone Integration: A "Smartphone" is connected to the wireless network to demonstrate mobile business capabilities.
Web Server Access: The smartphone can successfully browse and access the "Internal Web Site" hosted on the enterprise server.

5. Layer 2 Security (Port Security)
   
Intrusion Prevention: "Port Security" is active on all access switches.
Violation Policy:*If an unauthorized "Laptop" is plugged into a secure port, the switch identifies the unknown MAC address and immediately "shuts down" the port (err-disabled).

6. Automated IP Management (DHCP Relay)
   
Centralized DHCP: IP addresses are assigned automatically by the central server in Istanbul.
DHCP Relay: The Ankara router acts as a relay agent, allowing branch devices to get their IP configurations (IP, Mask, Gateway, DNS) automatically from the HQ.



🛠 Features Summary
| Feature    | Implementation |
| :---       | :--- |
| Redundancy | Dual-Cable / Fault Tolerant |
| Routing    | OSPF Dynamic Routing |
| Security   | Port Security (Shutdown) & Credentials |
| Wireless   | Smartphone & Access Point |
| Web Service| Internal Web Site Hosting |
| Automation | DHCP Relay Agent |

## 📸 Project Visuals

1. Network Infrastructure & Routing
 <br><br>
  Topology
 <br><br>
![Topology](Topology.png)
<br><br>
  OSPF Routes
<br><br>
![OSPF Routes](ospf-routing-table.png)
<br><br>
  Interface Status
<br><br>
![Interface Status](ip-address-inventory.png)
<br><br>
   VLAN Status
   <br><br>
![VLAN Status](switch-vlan-segmentation.png)
<br><br>

3. Security Implementations
   <br><br>
   Login Prompt
   <br><br>
![Login Prompt](secure-device-login.png)
<br><br>
    Port Security Status
   <br><br>
![Port Security Status](port-security-status.png)
<br><br>
    Security Violation
   <br><br>
![Security Violation](port-security-violation.png)
<br><br>
   Admin Telnet
   <br><br>
![Admin Telnet](admin-telnet-access.png)
<br><br>

5. Network Services & Connectivity
   <br><br>
   Ping Test
   <br><br>
![Ping Test](successfull-ping-result.png)
<br><br>
    DHCP Config 1
   <br><br>
![DHCP Config 1](automatic-ip-config1.png)
<br><br>
    DHCP Config 2
   <br><br>
![DHCP Config 2](automatic-ip-config2.png)
<br><br>
   Web Access
   <br><br>
![Web Access](SmartPhone.png)
