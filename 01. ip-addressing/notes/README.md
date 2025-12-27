
IP Addressing — Networking Notes

1. Introduction to IP Addressing

An IP address (Internet Protocol address) is a logical identifier assigned to a device on a network. It allows devices to identify each other and communicate across local networks and the internet.

In networking, IP addressing is essential because it defines:

Who a device is on the network

Where the device is located

How data should be delivered to it


These notes focus on IPv4, which is still widely used in most networks today.



2. Structure of an IPv4 Address

An IPv4 address:

Is 32 bits long

Is divided into four octets

Each octet contains 8 bits

Is written in decimal format separated by dots


Example:

192.168.1.10

Each octet ranges from 0 to 255 because 8 bits can represent 256 values.


3. Binary and Decimal Representation

Although humans read IP addresses in decimal, network devices process them in binary.

Decimal to Binary Example:

192 = 11000000
168 = 10101000
1   = 00000001
10  = 00001010

Full binary representation:

11000000.10101000.00000001.00001010

Why this matters:

Subnetting depends entirely on binary logic

Network calculations are based on bit values

Understanding binary prevents configuration errors


4. Classes of IP Addresses

IPv4 addresses were originally divided into classes to organize networks by size.

Class	Range	Default Subnet Mask	Purpose

A	1.0.0.0 – 126.255.255.255	255.0.0.0	Very large networks
B	128.0.0.0 – 191.255.255.255	255.255.0.0	Medium networks
C	192.0.0.0 – 223.255.255.255	255.255.255.0	Small networks
D	224.0.0.0 – 239.255.255.255	N/A	Multicast
E	240.0.0.0 – 255.255.255.255	N/A	Experimental


> Note: Modern networking uses CIDR, but classful addressing is still important for learning fundamentals.


5. Public vs Private IP Addresses

Private IP Addresses

Used inside local networks and cannot be routed on the internet.

Class	Private Range

A	10.0.0.0 – 10.255.255.255
B	172.16.0.0 – 172.31.255.255
C	192.168.0.0 – 192.168.255.255


Public IP Addresses

Assigned by ISPs

Used to access the internet

Must be unique globally


Why this matters:

Private IPs improve security and conserve public IP space through NAT (Network Address Translation).


6. Reserved and Special IP Addresses

Some IP addresses have special purposes:

Address	Purpose

0.0.0.0	Default route / unknown network
127.0.0.1	Loopback (localhost)
255.255.255.255	Broadcast to all devices
Network address	Identifies the network
Broadcast address	Reaches all hosts


These addresses must never be assigned to hosts.


7. Network and Host Identification

An IP address is divided into:

Network portion → identifies the network

Host portion → identifies the device


Example:

192.168.1.0/24

Network address: 192.168.1.0

Broadcast address: 192.168.1.255

Usable hosts: 192.168.1.1 – 192.168.1.254


Understanding this concept is critical before learning subnetting.



8. Practical Importance

IP addressing is used in:

Network design

Router and switch configuration

Packet Tracer simulations

Troubleshooting connectivity issues


Without proper IP addressing, network communication is impossible.


9. Summary

IP addressing forms the foundation of all networking concepts. Mastery of IPv4 structure, binary representation, address classes, and reserved ranges is essential before moving on to subnetting, Routing,and TCP/IP protocols. 
