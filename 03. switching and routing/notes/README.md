Networking Notes — Switching and Routing 

Switching and routing are core networking functions that enable data to move efficiently within a network and between different networks. These notes cover both Layer 2 (Switching) and Layer 3 (Routing) concepts and serve as a foundation for future Packet Tracer configurations and real-world network design.

1. Switching Fundamentals 

Switching operates at Layer 2 (Data Link Layer) of the OSI model. A switch connects devices within the same local network and forwards data based on MAC addresses.

Key characteristics of switching:

Reduces network collisions by creating separate collision domains Enables efficient internal network communication Operates faster than hubs by intelligently forwarding frames 

Why it matters:
Switches form the backbone of Local Area Networks (LANs) and are essential for scalable and efficient network design.

2. MAC Addresses and Frame Forwarding 

A MAC (Media Access Control) address is a unique 48-bit identifier assigned to a network interface card (NIC).

Switches use a MAC address table to make forwarding decisions:

The switch learns the source MAC address of incoming frames. It stores the MAC address with the corresponding port. When a destination MAC is known, the frame is forwarded only to the correct port. If unknown, the frame is flooded to all ports except the source. 

Why it matters:
Understanding MAC learning and forwarding is crucial for troubleshooting connectivity issues and preventing unnecessary network traffic.

3. VLANs (Virtual Local Area Networks) 

A VLAN logically separates a physical network into multiple virtual networks.

Benefits of VLANs:

Improved security by isolating traffic Reduced broadcast traffic Better network organization Flexibility without changing physical cabling 

Each VLAN acts as a separate broadcast domain, and communication between VLANs requires routing.

Why it matters:
VLANs are widely used in enterprise networks to segment departments, improve performance, and enforce security policies.

4. Static Routing 

Static routing involves manually configuring routes on a router.

Characteristics:

Administrator defines the path to a network Low overhead High control Not scalable for large networks 

Example use cases:

Small networks Backup routes Stub networks 

Why it matters:
Static routing helps build a strong understanding of routing logic before moving to dynamic protocols.

5. Dynamic Routing Protocols 

Dynamic routing protocols allow routers to automatically learn and update routes.

Common examples:

RIP (Routing Information Protocol) OSPF (Open Shortest Path First) EIGRP (Enhanced Interior Gateway Routing Protocol) BGP (Border Gateway Protocol) 

Advantages:

Automatic route updates Scalable for large networks Fault tolerance through route recalculation 

Why it matters:
Dynamic routing is essential for modern, large-scale, and resilient networks.
Mastering switching and routing concepts is critical for building functional and scalable networks. These topics directly support:

Packet Tracer simulations Network troubleshooting Enterprise network design Progression into advanced routing and security concepts 

These notes prepare me for hands-on configurations, certification studies, and real-world networking environments.
