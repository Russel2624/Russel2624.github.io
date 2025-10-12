# Network Diagrams

## Physical Topology
- Core layer: Cisco 4331 routers with redundant links
- Distribution layer: Cisco 3560 switches with EtherChannel
- Access layer: Multiple access switches per floor
- Wireless: WLC-300 with multiple access points

## Logical Design
- VLAN segmentation across departments
- Routing protocol boundaries
- Security zones and trust levels
- Wireless network mapping

## IP Addressing Scheme
- Infrastructure: 100.x.x.x/24
- User networks: 172.16.x.x/24 - 172.18.x.x/24
- Management: 192.168.1.0/24
