# 🌐 Networking Essentials Lab for Cybersecurity

This lab demonstrates foundational network traffic analysis skills using Wireshark and core Linux tools in a virtual lab environment. The purpose is to understand how protocols behave at the packet level — essential knowledge for security analysts and network defenders.

## 🔧 Lab Setup
- **Host Firewall**: pfSense (VirtualBox)
- **Client OS**: Ubuntu (192.168.1.10)
- **Tools Used**: Wireshark, ping, dig, curl, telnet

## 📡 Protocols Captured and Analyzed

| Protocol | Description | Screenshot |
|----------|-------------|------------|
| ICMP     | Captured echo requests and replies using `ping` to 8.8.8.8 | [icmp.png](screenshots/icmp.png) |
| DNS      | Captured domain resolution using `dig` / `nslookup` for `google.com` | [dns.png](screenshots/dns.png) |
| HTTP     | Captured GET requests and 200 OK responses using `curl http://neverssl.com` | [http.png](screenshots/http.png) |
| TCP SYN  | Captured TCP connection initiation using `telnet google.com 80` | [tcp-syn.png](screenshots/tcp-syn.png) |

## 📝 Documentation

See [`protocol-analysis.md`](protocol-analysis.md) for detailed breakdowns of each protocol observed and insights from the captured traffic.

## 🎯 Outcome

This project serves as the foundation for:
- Packet-level threat detection
- Firewall and IDS rule creation
- SOC analysis techniques

It forms part of a broader hands-on cybersecurity training journey aimed at SOC Analyst, Security Engineer, and Incident Responder roles.
