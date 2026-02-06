# VLAN & Router-on-a-Stick Lab

## Objective
Implement network segmentation using VLANs and enable inter-VLAN routing using a router-on-a-stick configuration.

## Network Design
- VLAN 10 – HR (192.168.10.0/24)
- VLAN 20 – IT (192.168.20.0/24)
- Cisco 2960 Layer 2 Switch
- Router with 802.1Q sub-interfaces

## Configuration Summary
- Access ports assigned to VLANs
- Trunk link between switch and router
- Sub-interfaces configured with dot1Q encapsulation
- Static IP addressing on hosts

## Testing
- Ping HR → Default Gateway ✔️
- Ping IT → Default Gateway ✔️
- Inter-VLAN communication HR ↔ IT ✔️

## Skills Demonstrated
- VLAN segmentation
- Trunking (802.1Q)
- Inter-VLAN routing
- Network troubleshooting (Layer 1–3)
