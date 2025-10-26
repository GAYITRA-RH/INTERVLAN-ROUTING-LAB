# INTERVLAN-ROUTING-LAB
Hands-on lab demonstrating Inter-VLAN routing using Cisco IOS, trunking, and router-on-a-stick configuration.”
 Inter-VLAN Routing Lab

 Topology Overview
- **Switch1: VLANs 10 (Sales), 20 (HR), 30 (IT)
  Router1: Sub-interfaces for each VLAN
- PCs: Assigned to different VLANs

 Key Configurations

Switch1
interface FastEthernet0/1
 switchport mode trunk
 switchport trunk allowed vlan 10,20,30
 ROUTER
 interface FastEthernet0/0.10
 encapsulation dot1Q 10
 ip address 192.168.10.1 255.255.255.0
 
