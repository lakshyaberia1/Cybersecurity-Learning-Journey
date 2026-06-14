# 🌐 Networking (Day 1–Day 5)

Learned:

- Networking Basics
- PAN, LAN, MAN, WAN
- Client-Server Model
- Peer-to-Peer Model
- Router
- Switch
- Hub
- Firewall
- Access Point
- OSI Model (7 Layers)
- TCP/IP Model
- IPv4 Addressing
- Private vs Public IP
- Loopback Address (`127.0.0.1`)
- MAC Address
- ARP (Address Resolution Protocol)
- DNS (Domain Name System)
- DHCP (Dynamic Host Configuration Protocol)
- NTP (Network Time Protocol)
- Chrony (`chronyd`)
- Common Networking Ports

## Important Concepts

- `IP Address` identifies a device across networks.
- `MAC Address` identifies a device on the local network.
- `ARP` converts an IP address to a MAC address.
- `DNS` converts domain names (e.g., `google.com`) into IP addresses.
- `8.8.8.8` is Google's **public DNS server**, not the IP address of `google.com`.
- `DHCP` automatically assigns IP addresses and other network settings.
- `NTP` synchronizes system time across devices.
- `Chrony` is a modern Linux implementation for time synchronization.
- `TCP` provides reliable communication, while `UDP` is faster but connectionless.

## Ports to Remember

- FTP → **20/21 TCP**
- SSH → **22 TCP**
- Telnet → **23 TCP**
- SMTP → **25 TCP**
- DNS → **53 TCP/UDP**
- DHCP → **67/68 UDP**
- HTTP → **80 TCP**
- HTTPS → **443 TCP**
- NTP → **123 UDP**
- SMB → **445 TCP**
- RDP → **3389 TCP**

## Anki

- DNS → Converts domain names to IP addresses.
- DHCP → Automatically assigns IP addresses.
- ARP → IP to MAC mapping.
- MAC Address → Physical address of a device.
- IP Address → Logical address of a device.
- OSI Layer 2 → Data Link Layer.
- OSI Layer 3 → Network Layer.
- Loopback IP → `127.0.0.1`
- NTP → Synchronizes time.
- Chrony → Linux time synchronization service.

## Next

- Subnetting
- CIDR Notation
- TCP vs UDP (Deep Dive)
- ICMP
- Routing
- NAT
- VLANs
- Wireshark Basics