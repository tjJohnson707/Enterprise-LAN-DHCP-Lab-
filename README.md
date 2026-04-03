# Enterprise LAN DHCP Lab

This lab focuses on building a small enterprise LAN and validating interfaces, DHCP behavior, and switch/router connectivity.

## Objectives
- Build an enterprise-style LAN in Packet Tracer
- Bring interfaces up correctly
- Validate switch and router links
- Confirm DHCP behavior on client segments
- Practice reading interface counters and physical status

## Included Files
- `lab-files/Enterprise-LAN-DHCP-conft.pkt`
- `assets/interface-output.png`

## Key Verification Habits
- `show ip interface brief`
- `show interfaces`
- `show vlan brief`
- `show interfaces trunk`
- `show ip dhcp binding`

## Interface Review
The included interface output was part of the lab validation process. I used interface counters and line protocol state to check whether links were actually up and whether the switchports were behaving as expected.


## What This Lab Reinforced
- A VLAN can be configured correctly on paper and still fail if the port is down, mispatched, or assigned incorrectly
- DHCP success depends on end-to-end path health, not just pool configuration
- Interface counters help separate logical configuration issues from physical/link issues

## Common Troubleshooting Flow Used
1. Verify cabling and link lights
2. Check port mode and VLAN membership
3. Confirm trunking between infrastructure devices
4. Validate router gateway/subinterface configuration
5. Renew DHCP on client and verify lease
6. Test with ping and inspect ARP/MAC learning

