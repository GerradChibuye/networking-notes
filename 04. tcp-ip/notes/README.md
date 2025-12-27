Subnetting Explained 

Subnetting is the process of dividing a large network into smaller, manageable subnetworks (subnets). It improves network performance, security, and efficient IP address utilization.

1. Subnet Masks 

A subnet mask determines which part of an IP address identifies the network and which part identifies the host.

Example:

IP Address: 192.168.1.10 Subnet Mask: 255.255.255.0 Network portion: 192.168.1 Host portion: .10 

Subnet masks work by masking the IP address using binary values.

2. CIDR Notation 

CIDR (Classless Inter-Domain Routing) uses a slash notation to represent the subnet mask.

Example:

192.168.1.0/24 /24 means the first 24 bits are network bits Remaining bits are for hosts 

CIDR allows flexible subnet sizes beyond traditional IP classes.

3. Custom Subnet Masks 

Custom subnet masks are used to create subnets of varying sizes based on requirements.

Example:

255.255.255.192 = /26 

This allows:

More networks Fewer hosts per network 

Custom masks are essential in real-world network design.

4. Borrowing Bits 

Borrowing bits involves taking bits from the host portion and using them as network bits.

More borrowed bits = more subnets Fewer borrowed bits = more hosts per subnet 

This concept is the foundation of subnetting calculations.

5. Network, Broadcast, and Usable Hosts 

For every subnet:

Network address: first address (all host bits = 0) Broadcast address: last address (all host bits = 1) Usable hosts: addresses between network and broadcast 

Example for /26:

Total addresses: 64 Usable hosts: 62 6. VLSM (Variable Length Subnet Masking) 

VLSM allows the use of different subnet sizes within the same network.

Benefits:

Efficient IP address usage Better scalability Common in enterprise networks 

VLSM is widely used with modern routing protocols like OSPF and EIGRP.

Reflection 

Subnetting is a critical skill for network segmentation and efficient design. Mastery of these concepts enables proper IP planning and supports advanced routing configurations in Packet Tracer.

Switching and Routing Switching and Routing Fundamentals 

Switching and routing enable data movement within and between networks, forming the backbone of modern communication systems.

1. Switching Fundamentals 

Switching occurs at Layer 2 (Data Link Layer) of the OSI model.

Switches connect devices within a LAN They reduce collisions and improve efficiency 2. MAC Addresses and Forwarding 

Each device has a unique MAC address.

Switches:

Learn MAC addresses dynamically Store them in a MAC address table Forward frames only to the intended destination port 

This improves network performance.

3. VLANs (Virtual Local Area Networks) 

VLANs logically separate devices within the same physical network.

Benefits:

Improved security Reduced broadcast traffic Better network organization 

Devices in different VLANs require routing to communicate.

4. Static Routing 

Static routes are manually configured by a network administrator.

Advantages:

Simple Predictable 

Disadvantages:

Not scalable Requires manual updates 5. Dynamic Routing Protocols 

Dynamic routing allows routers to learn routes automatically.

Common protocols:

RIP OSPF EIGRP BGP 

These protocols improve scalability and fault tolerance.

Reflection 

Understanding switching and routing is essential for building functional networks. These concepts are foundational for future Packet Tracer labs and real-world deployments.

TCP/IP Suite The TCP/IP Model and Protocols 

The TCP/IP suite defines how data is transmitted across networks, including the internet.

1. The Four-Layer TCP/IP Model Layer Function Application User services (HTTP, FTP, DNS) Transport End-to-end communication Internet Logical addressing and routing Network Access Physical data transmission 2. Encapsulation and Decapsulation Encapsulation: Data is wrapped with headers as it moves down the layers. Decapsulation: Headers are removed as data moves up the layers at the destination. 

This process ensures accurate data delivery.

3. Common TCP/IP Protocols TCP – Reliable, connection-oriented UDP – Fast, connectionless ICMP – Error reporting and diagnostics ARP – Resolves IP to MAC addresses DHCP – Automatically assigns IP addresses DNS – Resolves domain names to IP addresses 4. TCP vs UDP Comparison Feature TCP UDP Reliability High Low Speed Slower Faster Connection Required Not required Use cases Web, email Streaming, gaming Reflection 

The TCP/IP suite governs all modern network communication. Understanding these protocols demonstrates strong foundational knowledge of how data flows across networks.
