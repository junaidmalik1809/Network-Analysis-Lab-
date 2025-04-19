# 📊 Protocol Analysis Summary

## 🛰️ ICMP (ping)
- Used: `ping -c 3 8.8.8.8`
- Captured Type 8 (Echo Request) and Type 0 (Echo Reply)
- Proves that the host is reachable and packets are successfully routed

## 🌐 DNS
- Used: `dig google.com` and `nslookup google.com`
- Captured DNS query to resolve `google.com`
- Response included multiple A records (IPv4 addresses)
- Protocol used: UDP, Port 53

## 🌐 HTTP
- Used: `curl http://neverssl.com`
- Captured HTTP GET request and 200 OK response
- Payload visible in TCP stream (plain text)
- Protocol: TCP, Port 80

## 🔐 TCP SYN
- Used: `telnet google.com 80`
- Captured `SYN` packet from Ubuntu to remote server
- Filter used: `tcp.flags.syn == 1 && tcp.flags.ack == 0`
- Proves the first step of a TCP 3-way handshake (SYN)

---

These observations demonstrate live traffic generation, capture, and filtering of essential internet protocols — all skills relevant to real-world intrusion detection and network forensics.
