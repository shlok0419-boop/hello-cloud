# Networking Cheat Sheet
## My Environment
- VM IP address: 192.168.0.112 (interface enp0s3, bridged adapter)
- Default gateway: 192.168.0.1 (first hop in traceroute)
- Docker bridge: 172.17.0.1 (docker0, internal only)

## CIDR Calculation
- 10.0.0.0/24: 2^8 = 256 total addresses, 254 usable
  (first address 10.0.0.0 is the network, last address 10.0.0.255 is the broadcast)

## Public vs Private IPs
- Private (RFC 1918): 192.168.x.x, 10.x.x.x, 172.16.x.x to 172.31.x.x
- Public: Google's servers, for example 192.178.173.138 from dig

## Ports
- 22: SSH
- 80: HTTP
- 443: HTTPS

## DNS
- nslookup and dig resolved google.com to several IPs
- 127.0.0.53 is Ubuntu's local resolver (systemd-resolved)

## Commands Used
- ip addr, ip route, ss -tulpn
- ping, traceroute, nslookup, dig, ipcalc
- ssh, ssh-keygen, ssh-copy-id
