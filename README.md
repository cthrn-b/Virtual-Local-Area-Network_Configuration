# VLAN Configuration

## Objective
This focuses on creating and configuring **Virtual Local Area Networks (VLANs)** to achieve network segmentation, inter-VLAN communication, and trunking between switches.

## Overview
- Configure VLANs on managed switches.
- Establish trunk links for VLAN traffic between switches.
- Set up inter-VLAN routing using a router or Layer 3 switch.
- Verify VLAN connectivity and troubleshoot issues.

## Network Topology
- **Switch 1** ↔ **Switch 2** (Trunk Link)
- **Router** ↔ **Switch 1** (Inter-VLAN Routing)
- **Computers** connected to switch ports assigned to VLANs.

## VLAN and IP Addressing Plan
| VLAN | Network Address    |
|------|--------------------|
| 10   | 192.168.10.0/24    |
| 20   | 192.168.20.0/24    |
| 30   | 192.168.30.0/24    |

## Configuration Steps
1. **Configure VLANs on Switches**
   - Assign ports to VLANs: `vlan [VLAN ID]`
2. **Set Up Trunk Links**
   - Enable trunking on inter-switch ports: `switchport mode trunk`
3. **Configure Inter-VLAN Routing**
   - Set up router interfaces: `interface [interface]`
4. **Verify Connectivity**
   - Test with `ping` between VLANs.
5. **Optional Enhancements**
   - Configure DHCP for dynamic IP assignment.
   - Implement VLAN Trunking Protocol (VTP) for centralized VLAN management.

## Tools Required
- **Cisco Packet Tracer**

---

## Author
This project was created by the repository owner.
