```bash
# === Getting Started ===

# --- Connecting Using VPN ---

# connect to a vpn
sudo openvpn user.ovpn

# display currently active network interfaces
ifconfig

# display networks accessible by VPN
netstat -rn


# --- Basic Tools ---

# ssh into a server (username@host)
ssh Bob@10.10.10.10

# scan a server port with netcat
netcat 10.10.10.10 22


# --- Service Scanning ---

# basic nmap scan
# * PORT - port number and kind (TCP/UDP)
# * STATE - port state
# * SERVICE - typical service (not actual service, requires more in-depth scan)
nmap 10.129.42.253

# detailed nmap scan
# * -sC - obtain more detailed info
# * -sV - perform a version scan
# * -p- - scan all 65,535 ports
nmap -sV -sC -p- 10.129.42.253

# ftp into a server
ftp 10.129.42.253
```
