# Packet-Tracer---Project-2-Simple-Routing

![Project 2 Screenshot](https://github.com/pinoechalle-lang/Packet-Tracer---Project-2-Simple-Routing/blob/main/Screenshot%202026-10-19%20124852.png?raw=true)

---

## Requirements
This project requires configuring the two routers for Layer 3 routing and meeting the following requirements for the Routers and Switches:


### Switch
Switch SW-LAN-A and SW-LAN-B must be configured with a hostname, banner message, disable IP domain look-up, CLI access with the password "*hi*" and EXEC access with the password "*hello*", a session limited to 3 minutes and 30 seconds, and encrypt the plaintext passwords in the running configuration file.

 #### SW-LAN-A Remote Configuration
 Configure SW-LAN-A for secure remote management using the following parameters:
 
Domain Name: hellcomA.edu
 
Local User Account:
Username: SWA-Rem-Admin
Password: Joker
 
Remote Access Requirements:
- SSH Version 2 only
- Maximum of 5 simultaneous VTY sessions
- Session timeout: 3 minutes and 30 seconds
- RSA Key Size: 1024 bits

 
Management Interface:
- VLAN 1 (SVI)
- IPv4 Address: 192.168.50.8/24
- Default Gateway: 192.168.50.254

 #### SW-LAN-A Remote Configuration
 Configure SW-LAN-A for secure remote management using the following parameters:
 
 Domain Name: hellcomB.edu
 
 Local User Account:
 Username: SWB-Rem-Admin
 Password: Midas
 
 Remote Access Requirements:
 - SSH Version 2 only
 - Maximum of 16 simultaneous VTY sessions
 - Session timeout: 3 minutes and 0 seconds
 - RSA Key Size: 1024 bits
 
 Management Interface:
 - VLAN 1 (SVI)
 - IPv4 Address: 192.168.66.10/24
 - Default Gateway: 192.168.66.254

<b><b>
<b><b>
<b><b>

### Router
Router R1 and R2 must be configured with a hostname, banner message, disable IP domain look-up, CLI access with the password "*hi*" and EXEC access with the password "*hello*", a session limited to 5 minutes, and encrypt the plaintext passwords in the running configuration file.
### Network Addresses and IP Configuration on Interfaces/End Devices

| Router | Interface | IP Address | Subnet Mask | Description |
|--------|-----------|------------|-------------|-------------|
| R1 | G0/0 | 192.168.50.254 | 255.255.255.0 | Link to LAN A |
| R1 | G0/1 | 172.27.39.1 | 255.255.255.252 | Link to R2 |
| R2 | G0/0 | 172.27.39.2 | 255.255.255.252 | Link to R1 |
| R2 | G0/1 | 192.168.66.254 | 255.255.255.0 | Link to LAN B |

---

## Verification

```bash
show ip interface brief
show running-config
show interfaces
show ip route

ping 192.168.66.1
traceroute 192.168.66.1
```
// if in Global Configuration Mode, make sure to include "do"

##### show ip interface brief
> Show interfaces status whether up or down

##### show running-config
> Show current active configurations you made

##### show interfaces
> Show detailed information about all interfaces including packet statistics, speed, and duplex

##### show ip route
> Show the router's routing table

> Only in a router device

##### ping <ipv4-address>
> Sends ICMP packets to a given address destination to test reachability

##### traceroute <ipv4-address>
> Shows the path (hops) a packet takes to reach a destination
