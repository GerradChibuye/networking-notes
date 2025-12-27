
Networking Notes — Subnetting

Subnetting is the process of dividing a larger IP network into smaller, more efficient sub-networks (subnets). It improves network performance, enhances security, and allows better utilization of IP addresses.
These notes build directly on IP addressing and are essential for routing, switching, and real-world network design.


1. Subnet Masks

A subnet mask defines which part of an IP address represents the network and which part represents the host.

Example:

IP Address: 192.168.1.10
Subnet Mask: 255.255.255.0

255 = network portion

0 = host portion


In binary:

255.255.255.0
11111111.11111111.11111111.00000000

Why subnet masks matter:
They allow devices to determine whether a destination is on the same network or must be reached via a router.


---

2. CIDR Notation

CIDR (Classless Inter-Domain Routing) replaces class-based addressing with a slash notation.

Example:

192.168.1.0/24

/24 means 24 bits are used for the network

Remaining bits are for hosts


Common CIDR examples:

/8 → 255.0.0.0

/16 → 255.255.0.0

/24 → 255.255.255.0


Why CIDR is important:
It allows flexible subnet sizes and efficient IP address allocation.


3. Custom Subnet Masks

Custom subnet masks are created by borrowing bits from the host portion to create more subnets.

Example:

Default Class C: /24
Custom Mask: /26

Borrowed 2 bits

Creates 4 subnets

Each subnet has fewer hosts


This is commonly used in enterprise and campus networks.



4. Borrowing Bits

Borrowing bits determines:

Number of subnets

Number of hosts per subnet


Formulas:

Subnets: 2^borrowed bits

Hosts: 2^remaining bits – 2


Example:

/26 from /24
Borrowed bits = 2
Subnets = 2² = 4
Hosts = 2⁶ – 2 = 62

Why this matters:
It allows precise control over network size and scalability.



5. Network, Broadcast, and Usable Host Calculations

Each subnet contains:

Network Address: First address (all host bits = 0)

Broadcast Address: Last address (all host bits = 1)

Usable Hosts: Addresses between network and broadcast


Example:

Subnet: 192.168.1.64/26
Network: 192.168.1.64
Broadcast: 192.168.1.127
Usable Hosts: 192.168.1.65 – 192.168.1.126

These calculations are critical for router configuration and troubleshooting.


6. VLSM (Variable Length Subnet Masking)

VLSM allows different subnet sizes within the same network, based on actual requirements.

Example use case:

Large subnet for servers

Smaller subnets for departments

Minimal wastage of IP addresses


Why VLSM is powerful:

Efficient IP utilization

Scalable network design

Required for modern routing protocols (OSPF, EIGRP)

Subnetting transforms IP addressing from theory into practical network engineering.
Mastery of subnet masks, CIDR, bit borrowing, and VLSM enables efficient network segmentation, improved performance, and secure design—skills essential for Packet Tracer labs and real-world networking.
