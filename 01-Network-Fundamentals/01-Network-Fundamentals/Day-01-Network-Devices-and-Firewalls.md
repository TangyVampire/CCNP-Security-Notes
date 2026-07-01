Day 01 - Network Devices and Firewalls
Learning objectives
Understand different network devices.
Difference between Switch, Router, and Firewall.
Learn firewall types.
Learn the 5-Tuple mechanism.
Introduction to Cisco ASA and Cisco FTD.

**1. Switch**
2. 
**Layer 2 Switch**
Works at OSI Layer 2.
Uses a MAC Address Table.
Forwards frames based on MAC addresses.

**Layer 3 Switch**
Works at Layer 2 and Layer 3.
Uses:
MAC Address Table
Routing Table
Can perform routing between VLANs.

**2. Router**

**Purpose**
Connects multiple networks.
Operates at Layer 3.

**Uses**
Routing Table
Best path selection
Internet connectivity

**Default Behavior**
Permit Any → Any

Meaning:
By default, routers forward all traffic if a route exists.

**3. Firewall**

**Purpose**
Connects multiple networks securely.
Controls network traffic using security policies.

**Uses**
Routing Table
Security Policies

**Default Behavior**
Deny Any → Any

Meaning:
Traffic is blocked unless explicitly allowed.

**Router vs Firewall**
Router	                  Firewall
Connects networks       	Connects & secures networks
Default: Permit	          Default: Deny
Routing                 	Routing + Security

**Packet Information**

A packet contains:

Source IP
Destination IP
Source MAC
Destination MAC
Source Port
Destination Port
Protocol (TCP/UDP)

Example:

Source IP: 10.3.3.3
Destination IP: 53.63.54.86
Source Port: 12568
Destination Port: 443
Protocol: TCP

**Traditional Firewall**

Can filter traffic using:

Source IP
Destination IP
Source Port
Destination Port
Protocol

This is known as the **5-Tuple Check Mechanism.**

**Next Generation Firewall (NGFW)**

Additional security features include:

URL Filtering
Content Filtering
Geo-Location Policies
Application Awareness
Threat Prevention

Example:

Cisco ASA
Cisco FTD (Cisco Secure Firewall)

**Firewall Types**
**1.Stateless Firewall**
Examines each packet independently.
Does not remember previous packets.

**2.Stateful Firewall**
Maintains connection state.
More secure.
Allows return traffic automatically.

**Firewall Modes**
**1.Routed Mode**
Firewall acts as a Layer 3 device.
Uses IP addresses.

**2.Transparent Mode**
Firewall acts like a Layer 2 bridge.
Minimal changes to the existing network.

**Key Takeaways**
Switch → MAC-based forwarding.
Router → Routing between networks.
Firewall → Security enforcement.
Router default = Permit.
Firewall default = Deny.
Traditional Firewall = 5-Tuple filtering.
NGFW = Advanced security features.
Cisco ASA = Traditional firewall.
Cisco FTD = Next-Generation Firewall.
