# DEBIAN NETFILTER FIREWALL V2
By Daniel Tobar
- **Github:** https://github.com/venorant/Debian_Netfilter_FirewallV2

## OBJECTIVE
Designed and implemented a stateful Linux firewall using Debian, Netfilter, and nftables in a virtual WAN/LAN environment. The project focuses on network segmentation, IPv4/IPv6 traffic filtering, access control, NAT, and security testing.

## TASKS & RESPONSABILITIES
- Built a virtual network using three Debian machines: FV2 (firewall), WAN_FV2 (external host), and LAN_FV2 (internal client).
- Configured WAN and LAN interfaces using VirtualBox and NetworkManager.
- Enabled persistent IPv4 and IPv6 packet forwarding.
- Implemented stateful nftables rules with default-deny INPUT and FORWARD policies.
- Allowed established and related connections, dropped invalid traffic, and restricted SSH access to the LAN.
- Configured IPv4 masquerading and IPv6 NAT66 for outbound LAN connectivity.
- Tested firewall behavior using Nmap, SSH, ping, and tcpdump.

## SKILLS & TOOLS
- **Operating Systems & Virtualization:** Debian Linux, Oracle VirtualBox
- **Networking:** IPv4/IPv6, TCP/IP, routing, NAT, network segmentation, NetworkManager
- **Security:** Netfilter, nftables, stateful packet filtering, firewall access control
- **Testing:** Nmap, SSH, tcpdump, ping
- **Version Control & Documentation:** Git, GitHub, Visual Studio Code

## TESTING & RESULTS
The following tests were performed to evaluate firewall security policies and network connectivity.
| Tests | Results | Evidence |
|---|---|---|
| Firewall rules | Verified active filtering and NAT rules | [Screenshot](screenshots/nftables-rules.png) |
| WAN port scanning | Nmap reported filtered TCP ports over IPv4 and IPv6 | [Screenshot](screenshots/nmap-wan.png) |
| WAN SSH access | IPv4 and IPv6 connection attempts timed out | [Screenshot](screenshots/ssh-wan-blocked.png) |
| LAN SSH access | Successfully connected from the LAN | [Screenshot](screenshots/ssh-lan-allowed.png) |
| LAN-to-firewall connectivity | Verified IPv4 and IPv6 communication | [Screenshot](screenshots/lan-firewall-connectivity.png) |
| LAN-to-Internet connectivity | Verified outbound IPv4 and IPv6 connectivity | [Screenshot](screenshots/lan-internet-connectivity.png) |
| LAN traffic monitoring | Captured traffic on the internal interface | [Screenshot](screenshots/tcpdump-lan.png) |
| WAN traffic monitoring | Captured traffic on the external interface | [Screenshot](screenshots/tcpdump-wan.png) |

## ACHIEVEMENTS & IMPACT
- Implemented a dual-stack, stateful Linux firewall with default-deny security policies.
- Restricted inbound SSH access while allowing authorized connections from the internal LAN.
- Configured IPv4 masquerading and IPv6 NAT66 for outbound LAN connectivity.
- Validated firewall behavior using port scanning, connectivity testing, and packet captures.
- Developed practical experience in Linux firewall administration, network security, and troubleshooting.