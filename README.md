# Packet-Tracer---Project-2-Simple-Routing

![Project 2 Screenshot](https://github.com/pinoechalle-lang/Packet-Tracer---Project-2-Simple-Routing/blob/main/Screenshot%202026-10-18%20214256.png?raw=true)


## In this project, the network admin must configure the two routers for Layer 3 routing and configure the following requirements for the Routers and Switches:

<hr>

## Requirements

### Switch
Switch SW-LAN-A and SW-LAN-B must be configured with a hostname, banner message, CLI access and EXEC access with a password and session limited to 3 minutes and 30 seconds, have the passwords encrypted in the config file, and enable the no IP domain look-up.


### Router
Router R1 and R2 must be configured with a hostname, banner message, CLI access and EXEC access with a password and session limited to 5 minutes, have the passwords encrypted in the config file, and enable the no IP domain look-up.


### Network Addresses and IP Configuration on Interfaces/End Devices

| Router | Interface | IP Address | Subnet Mask | Purpose |
|--------|-----------|------------|-------------|---------|
| R1 | G0/0 | 192.168.50.254 | 255.255.255.0 | Link to LAN A |
| R1 | G0/1 | 172.27.39.1 | 255.255.255.252 | Link to R2 |
| R2 | G0/0 | 172.27.39.2 | 255.255.255.252 | Link to R1 |
| R2 | G0/1 | 192.168.66.254 | 255.255.255.0 | Link to LAN B |
<hr/>

<hr>
## Verification
<hr/>

