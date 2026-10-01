# DEBIAN NETFILTER FIREWALL V2
By Daniel Tobar
- Github: https://github.com/venorant/Debian_Netfilter_FirewallV2

## OBJECTIVE
The purpose of this project is to demonstrate both knowledge and practical skills regarding firewall design and rule implementation using the Linux Netfilter framework and nftables. The project focuses primarily on filtering traffic passing through the firewall as well as traffic directed at the firewall itself. The test lab uses several Debian virtual machines to simulate a LAN/WAN environment and evaluate the firewall's security policies. The project also aims to demonstrate proficiency in network segmentation, network troubleshooting, and Linux administration.

## TASKS & RESPONSABILITIES
- Design and implement a secure WAN/LAN network architecture using multiple Debian virtual machines.
- Configure and manage a Debian-based firewall using the Linux Netfilter framework and nftables.
- Implement stateful IPv4 and IPv6 traffic filtering.
- Configure firewall policies for INPUT, OUTPUT, and FORWARD traffic.
- Configure IPv4 and IPv6 packet forwarding.
- Implement IPv4 NAT using MASQUERADE for the private LAN.
- Restrict administrative access to authorized network segments.
- Implement event logging and traffic monitoring for security analysis.
- Conduct network and security tests using tools such as Nmap and tcpdump.
- Troubleshoot network connectivity issues and firewall rule behavior.
- Document the configuration, testing process, and results using Git, GitHub, and Visual Studio Code.

## SKILLS & TOOLS
- Oracle VirtualBox
- Debian Linux
- Netfilter
- Nftables
- IPv4/IPv6
- TCP/IP networks
- Network segmentation
- Routing
- NAT
- Stateful firewall configuration
- Nmap
- tcpdump
- Git
- GitHub
- Visual Studio Code

## ACHIVMENTS & IMPACT
- Designed a virtual WAN/LAN topology using three Debian virtual machines: FV2 (firewall), WAN_FV2 (external host), and LAN_FV2 (internal client).
- Configured VirtualBox network adapters to separate the external WAN network from the internal LAN.
- Configured network connection profiles using NetworkManager ("nmcli").
- Configured the firewall WAN interface to obtain IPv4 and IPv6 settings automatically.
- Assigned static IPv4 and IPv6 addresses to the firewall's LAN interface and the internal client.
- Verified IPv4 and IPv6 connectivity between the internal client and the firewall.
- Enabled IPv4 and IPv6 packet forwarding using Linux 'sysctl' settings.
- Configured persistent forwarding settings in '/etc/sysctl.d/99-firewall.conf'.
- Verified that both IPv4 and IPv6 forwarding are enabled.
