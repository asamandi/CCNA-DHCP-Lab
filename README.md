DHCP Relay (IP Helper Address)

TOPOLOGY
----------------------------------------------
PC1 ── VLAN 10 ── R1 ── R2 ── DHCP Server

Roles:
----------------------------------------------
PC1 → DHCP client

R1 → default gateway for PC1

R2 → holds the DHCP server

R1 must relay DHCP to R2

IP Addressing Plan
----------------------------------------------
PC LAN (VLAN 10)

Network: 192.168.10.0/24

Gateway: 192.168.10.1

R1–R2 Link

R1 g0/1 → 10.0.12.1/30

R2 g0/1 → 10.0.12.2/30

DHCP Server LAN

Network: 172.16.1.0/24

Server IP: 172.16.1.50

R2 g0/0 = 172.16.1.1
