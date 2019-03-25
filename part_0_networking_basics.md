### Logical and Physical Topologies
Topologies - Shape of Network
* **Physical Topology** - Actual shape or layout of the wires in a Network
* **Logical Topology** - Pattern of data flow in the network
A network can have one physical topology but an entirely different logical topology.

### Various examples of Topology
#### Mesh
* **Full Mesh** - all devices directly connected to all other devices, hence requires
multiple NICs and cables for each node. It is very expensive and provides full redundancy. Found in WAN environment. E.g. Connection between cities.
* **Partial Mesh** - each device is connected to at least two other devices. It provides
strong redundancy but not Full redundancy. Comparatively less expensive. Found in WAN
Environment. E.g. Internet

#### Bus
This is the oldest network topology. All devices are connected to a main cable called bus.
Simple to put together. Disadvantages: only one device can send data through the bus at one
time. *Contention* is used to determine which node sends signal. Node listen to the network.
If it does not hear any signal, the node sends one. Now, here if two nodes are
simultaneously active, do not hear any signal, and send their own. The signals will collide
and effectively gets cancelled. If sufficient number of collisions, referred to as *network
storm*, can bring down the entire network. This is the idea behind many of their
**denial-of-service** attack heard in network security.

This topology is recommended for 30 or less nodes. This is the least expensive topology.
It is not a part of current TIA/EIA 568-C standard for LAN networks.  or terminating
resistor is required on either sides of the cable.

#### Ring
Similar to bus topology. The backbone is a ring.Packets are available to move around in a
ring pattern. As packet moves through the ring, it stops at each node and gives it an
opportunity to send a signal. Hence there is no contention. During heavy traffic, the network
slows down but does not break. A single damaged node can bring down the entire network.
This is not a part of the current TIA/EIA 568-C standard for LAN networks. 
