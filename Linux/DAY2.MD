# Day 2
14-06-2026
## Linux Networking

Learned:

- ping (ICMP connectivity testing)
- curl (HTTP/HTTPS requests)
- FTP basics
- SCP (Secure Copy over SSH)
- rsync (File synchronization)
- Package Management
  - apt
  - dpkg
  - rpm
  - yum
  - dnf
- systemctl `start` vs `enable`
- Local Git Repository
- Hostname lookup
- DNS lookup
  - dig
  - host
  - nslookup
- Google Public DNS (`8.8.8.8`)
- NTP (Network Time Protocol)
- Chrony (`chronyd`)

## Important Concepts

- `8.8.8.8` is a **DNS server**, not the IP address of `google.com`.
- `google.com` resolves to different IP addresses (e.g., `142.250.x.x`) using DNS.
- `systemctl start` starts a service **now**.
- `systemctl enable` makes a service start **automatically on boot**.
- `chronyd` is software that implements the **NTP protocol** to keep system time synchronized.
- `rsync` copies only changed files, making it efficient for backups and synchronization.



## Ports to Remember

- FTP → **21/TCP**
- SSH / SCP → **22/TCP**
- Telnet → **23/TCP**
- HTTP → **80/TCP**
- HTTPS → **443/TCP**
- NTP → **123/UDP**

## Next

- DHCP
- ARP
- TCP vs UDP
- CIDR Notation
- `ss` command
- `tcpdump`