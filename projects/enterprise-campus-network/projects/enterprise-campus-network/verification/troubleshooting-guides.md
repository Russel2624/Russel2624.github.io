# Troubleshooting Guides

## Connectivity Issues
### No Internet Access
1. Check BGP neighbor status: `show bgp summary`
2. Verify PPPoE connection: `show pppoe session`
3. Confirm NAT translation: `show ip nat translations`

### Inter-VLAN Routing Failure
1. Check router interfaces: `show ip interface brief`
2. Verify routing table: `show ip route`
3. Test ACL filtering: `show access-lists`

## Routing Protocol Issues
### EIGRP Neighbor Problems
1. Verify neighbor relationships: `show eigrp neighbors`
2. Check network statements: `show run | section eigrp`
3. Validate K-values match: `show eigrp protocols`

### OSPF Adjacency Issues
1. Check area configuration: `show ip ospf interface`
2. Verify hello/dead timers: `show ip ospf neighbor`
3. Confirm network types match

## Switching Problems
### VLAN Issues
1. Verify VLAN database: `show vlan brief`
2. Check trunk configuration: `show interface trunk`
3. Confirm VTP status: `show vtp status`

### Port Security Violations
1. Check violation counters: `show port-security`
2. Review MAC address table: `show mac address-table`
3. Verify aging configuration

## Wireless Troubleshooting
### Client Connectivity
1. Check AP status: `show ap summary`
2. Verify client associations: `show client summary`
3. Confirm RF environment: `show rf-profile`

### SSID Issues
1. Verify WLAN configuration: `show wlan summary`
2. Check VLAN mapping: `show wlan id <wlan-id>`
3. Validate security settings

## Methodology
1. **Bottom-up approach**: Physical → Data Link → Network
2. **Divide and conquer**: Isolate problem domains
3. **Document findings**: Maintain troubleshooting logs
