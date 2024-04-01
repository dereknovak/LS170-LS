# The Internet

## Network
https://launchschool.com/lessons/4af196b9/assignments/268243e5

"At the most basic level, it's two devices connected in such a way that they can communicate or exchange data."

## Local Area Network (LAN)
https://launchschool.com/lessons/4af196b9/assignments/268243e5

"...multiple computers and other devices connected via a network bridging device such as a hub or, more likely, a switch. The computers are all connected to this device via network cables, and this forms the network."

## Router

"Routers are network devices that can route network traffic to other networks. Within a Local Area Network, they effectively act as gateways into and out of the network."'

## Protocol

"In simple terms, we can think of a protocol as a *system of rules*."

"In terms of computer networks, we can be a bit more specific: A set of rules that govern the exchange or transmission of data."

Why so many protocols?

1. "Different protocols were developed to address different aspects of network communication."
2. "Different protocols were developed to address the same aspect of network communication but differently for a specific use case."

### OSI Model

Wikipedia: https://en.wikipedia.org/wiki/OSI_model
- "The Open Systems Interconnection model (OSI model) is a reference model from the International Organization for Standardization (ISO) that "provides a common basis for the coordination of standards development for the purpose of systems interconnection."

- Layer 1: Application
- Layer 2: Presentation
- Layer 3: Session
- Layer 4: Transport
- Layer 5: Network
- Layer 6: Data Link
- Layer 7: Physical

## Protocol Data Units (PDU)
https://launchschool.com/lessons/4af196b9/assignments/21ef33af

"...a Protocol Data Unit (PDU) is an amount or block of data transferred over a network. Different protocols or protocol layers refer to PDUs by different names. At the Link/ Data Link layer, for example, a PDU is known as a frame. At the Internet/ Network layer it is known as a packet. At the Transport layer, it is known as a segment (TCP) or datagram (UDP)."

### Encapsulation of Data

Quiz Answers:

- "Encapsulation is implemented through the use of Protocol Data Units (PDUs)."
- "Encapsulation creates separation between protocols operating at different networks layers."
- "With encapsulation, the entire PDU from one layer forms the data payload for the PDU at the layer below."

### Header/Trailer

"The exact structure of the header and, if included, trailer varies from protocol to protocol, but the purpose of them is the same in each case: to provide protocol-specific metadata about the PDU."

# Wires, Cables, and WiFi (Khan Academy)
https://www.khanacademy.org/computing/code-org/computers-and-the-internet/internet-works/v/the-internet-wires-cables-and-wifi

### Bit
Khan Academy
"A bit can be described as any pair of opposites: on or off, yes or no. We typically use a 1 (on) or a 0 (off)"
"These are the atoms of information."
"Today, we physically send bits by electricity, lights, and radio waves."

### Bandwidth

"Bandwidth is the amount of data that can be sent in a particular unit of time (typically, a second)."

### Bit Rate

"The number of bits that we can send over a given period of time, usually measured in seconds."

### Latency

"...latency is a measure of the time it takes for some data to get from one point in a network to another point in a network."

## Methods of Transportation

### Electricity (Copper wires)

- Cheap
- Signal loss

### Fiber Optic Cable

"A thread of glass engineered to reflect light."
- Really fast
- No signal loss
- Expensive

### Radio Waves
"Uses radio signal to send bits from one place to another."
- Translates 1's and 0's from binary to radio waves and back.
- Totally mobile
- Short range

### Fault Tolerant

Because a package can take a variety of routes from one IP address to another, the system is fault tolerant, as a distruption in one path can be avoiding by following another path.

### Hop

Each time a package is sent to a different router, a *hop* is performed. Each IP package keeps track of its hop count, preventing bugs in the path from halting a delivery using the hop limit.

## Ethernet
https://launchschool.com/lessons/4af196b9/assignments/81df3782

- "An Ethernet Frame adds logical structure to this binary data."
- "Two of the most important aspects of Ethernet are framing and addressing."

## MAC Address
https://launchschool.com/lessons/4af196b9/assignments/81df3782

- Media Access Control address
- "Since this address is linked to the specific physical device, and (usually) doesn't change, it is sometimes referred to as the physical address or burned-in address. MAC Addresses are formatted as a sequence of six two-digit hexadecimal numbers, e.g. 00:40:96:9d:68:0a, with different ranges of addresses being assigned to different network hardware manufacturers."

## Internet Protocol (IP) address
https://launchschool.com/lessons/4af196b9/assignments/b222ecfb

- "This means that they are not tied to a specific device, but can be assigned as required to devices as they join a network."
- "The Protocol Data Unit (PDU) within the IP Protocol is referred to as a packet."
- "Within both models, the primary function of protocols at this layer is to facilitate communication between hosts (e.g. computers) on different networks."

# The Transport Layer

## Communication Between Processes
https://launchschool.com/lessons/2a6c7439/assignments/41113e98

### Multiplexing

- "In the context of a communication network, this idea of transmitting multiple signals over a single channel is known as multiplexing, with demultiplexing being the reverse process."

### Port

- "In simple terms a port is an identifier for a specific process running on a host. This identifier is an integer in the range 0-65535."
- "Ports are used in the process of multiplexing and demultiplexing."
- The source and destination port numbers can be seen in the Transport layer PDUs.

### Socket

- Combination of the IP address and port number
- During implementation, a socket can be instantiated as a socket object.
- "A socket is a communication end-point."
- A socket is used to establish connection between applications.

## TCP (Transmission Control Protocol)
https://launchschool.com/lessons/2a6c7439/assignments/d09ddd52

### Included

- Connection-oriented protocol
- Multiplexing/Demultiplexing
- In-order delivery
- De-duplication
- Message acknowledgements and retransmission
- Error detection (checksum)

### Three-way Handshake

A three-way handshake is used within TCP to establish a working connection between two applications.

### Flow Control

- "Flow Control is a mechanism to prevent the sender overwhelming the receiver with more data than it can process. Each participant in a connection lets the other participant know how much data it is willing to accept using a field in the TCP header."

### Congestion Avoidance

- "Congestion avoidance is a process by which TCP uses data loss (based on the volume of retransmissions required) as a feedback mechanism to determine how congested the network is, and adjusts the amount of data being sent accordingly."

## UDP (User Datagram Protocol)
https://launchschool.com/lessons/2a6c7439/assignments/9bb82c9b

- "The Protocol Data Unit (PDU) of UDP is known as a Datagram."
- "This simplicity provides two things to a software engineer: speed and flexibility."

### Included:

- Connectionless protocol
- Multiplexing/Demultiplexing
- Error detection (checksum)

### What it doesn't do:

- "It provides no guarantee of message delivery"
- "It provides no guarantee of message delivery order"
- "It provides no built-in congestion avoidance or flow-control mechanisms"
- "It provides no connection state tracking, since it is a connectionless protocol"

# HTTP

## The Application Layer
https://launchschool.com/lessons/cc97deb5/assignments/c604eb60

- "We can perhaps think of Application layer protocols as being the rules for how applications talk to each other at a syntactical level."

## The World Wide Web
https://launchschool.com/lessons/cc97deb5/assignments/e3d85587

- "The World Wide Web, or web for short, is a service that can be accessed via the internet. In simple terms it is a vast information system comprised of resources which are navigable by means of a URL (Uniform Resource Locator)."

### HTML

- "Hypertext Markup Language (HTML) was the means by which the resources in this system should be uniformly structured."

### URI

- "A Uniform Resource Identifier (URI), is a string of characters which identifies a particular resource."

### HTTP
- "Hypertext Transfer Protocol (HTTP) is the set of rules which provide uniformity to the way resources on the web are transferred between applications."


