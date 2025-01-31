# Faculty of Engineering Network Project

## Overview
This project is a simulation of the **Faculty of Engineering Network** using **Cisco Packet Tracer**. The goal is to design and implement a network that connects the **main building** and **workshops**, ensuring connectivity, security, and efficient resource allocation.

## Network Topology
The network consists of two main areas:
1. **Main Building**
   - **Four floors**, each containing:
     - **Camera Switch:** Connects security cameras.
     - **Device Switch:** Connects PCs, printers, and other devices.
   - A dedicated **security switch** in the security office connects all camera switches.
   - Cameras are isolated from the internet and other networks.
  
![Picture1](https://github.com/user-attachments/assets/aa91d6b2-b971-48f4-aacb-544eaa151bfa)

2. **Workshops**
   - Connected to the main building via a **router-to-router connection**.
   - Each floor has local switches connected to a **main switch**, which is linked to a **DHCP server** for dynamic IP assignment.
  
![Picture8](https://github.com/user-attachments/assets/e5a1b0ec-ab37-4990-84b0-970a25c6d971)

## Network Configuration
- **Camera Network:**
  - Isolated from the main network.
  - Uses **static IP addressing**.
- **Device Network:**
  - Connected to the main building router.
  - Uses **DHCP for dynamic IP allocation**.
- **Subnetting:**
  - Library uses a subnet mask of `255.255.255.192` to allocate 64 addresses.

## Setup Instructions
1. **Open the Project**
   - Download and open the `.pkt` file in **Cisco Packet Tracer**.
2. **Explore the Topology**
   - Check router, switch, and end-device connections.
3. **View IP Assignments**
   - Use `show ip interface brief` in the CLI to inspect configurations.
4. **Test Network Connectivity**
   - Ping between devices to verify communication.

## Future Enhancements
- Implement **VLANs** for improved segmentation.
- Configure **firewall rules** for better security.
- Add **remote access (VPN)** for monitoring.

## License
This project is open-source. Feel free to use and modify it!



