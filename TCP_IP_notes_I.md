The TCP/IP guide notes

P1 NETWORKING FUNDAMENTALS 
Ch1 networking introduction
The network functions are often divided into layers of hardware and software, each of which perform a particular type of task and interact with layers above and below it. Layers are conceptually arranged in a vertical stack.

Lower layers perform concrete tasks like hardware signalling and component communication, while higher layers implement more abstract functions like implementing user applications.

Layers allow technology to be reused, and for this there has to be a universal standard.

The networking model defines the layers of a network, their functions and interaction.

The most common networking model is the OSI (Open Systems Interconnection) Reference Model, which consists of 7 stacked layers: physical layer 1 at the bottom in responsible for low-level signalling, and level 7 that implements application software.


An architecture is a rule set, usually defined in a specification  or standard, describing how technology should behave.

TCP/IP is a protocol suite that runs the internet.

TCP stands for Transmission Control Protocol and operates at level 4 of the OSI model. 

IP stands for Internet Protocol and runs at OSI model level 3.

Protocols define a language and a set of rules and procedures that ensure devices and systems communicate. In the OSI R Model, a protocol defines communication standards between entities of the same layer.


The term protocol is vague.

A protocol suite is a set or a stack of protocols, for example, TCP/IP.

Microsoft Windows uses the word protocol to refer to a full networking stack, like TCP/IP or IPX/SPX. Installing a Microsoft Windows protocol installs a software module that supports the full protocol suite.


In the circuit switching networking method, a connection called a circuit, which is used for the whole communication, is established between two devices. A new circuit containing the hardware available is set up for each new connection.

Circuit switching is used in PSTN.

In the packet switching networking method, no fixed path is created between communicating devices, data is divided into packets that are sent individually, each taking a different route. At the destination, packets are reassembled to form the original data.

Data packets are also called frames, datagrams, cells, or segments.

Packet switching is a better option than circuit switching when resources are shared, like in a LAN, because no dedicated connection is made and all transmissions can be serviced at once.

During packet switching, data can be reordered or lost in transit.

In modern networks, circuit switching and packet switching are often combined.

A connection-oriented protocol is one in which a logical connection is established between devices prior to data being sent. In a connectionless protocol, data is sent without a connection being created.

All circuit-switched networks are connection-oriented, but others, like packet switching protocols, can be connection-oriented as well.

TCP IP File Transfer Protocol requires forming a connection for passing commands and logins.
Telnet protocol requires a connection, allowing remote control over a machine.

Both work over IP, which is packet-switched.

Packet switching can be used as a bottom layer and a logical connection can be created in the top layers.

TCP IP has two main protocols that operate at the transport layer of the OSIRM. 
TCP is connection oriented and UDP - user datagram protocol - is connectionless.

UDP is used for applications that do not require a connection for their features because it can offer faster performance.

A connectionless protocol can be implemented over a connection-oriented protocol at a lower level. Connectionless IP can run over connection oriented ATM Asynchronous Transfer Network.

In packet switching messages are sent from one device to another.

Different terms exist to indicate the contents of each message, but they are not used consistently. 

A packet is a message sent by protocols operating at the network layer of the OSI RM (IP packet). It is also used instead of the term message.

A datagram is another word for packet. It is also used for messages sent at higher levels of the OSI RM.

A frame is a message sent at a low level if the OSI RM, physical layer, data link layers. Higher level data is framed with a header and footer.

A cell is fixed in size. An ATM cell is always 53 bytes long. Cells are usually sent at lower levels.

protocol data unit and service data units are formal terms using the OSI reference model to describe protocol messages. A PDU consists of a layer's header and an encapsulated message from the layer above. The encapsulated message without the header and footer is called the SDU of the layer above.

PDU of a layer = SDU of layer above + header of current layer

In TCP messages are called segments.
In ethernet messages are called frames.

every protocol uses a special formatting method that determines the structure of the messages.

typically a message contains a header data and a footer. The header normally contains a small number of control information bytes.

The data is sometimes called the payload some messages. Some messages do not have a payload because they are used for control and communication. 

The photo comes after the data it is a control field just like a header. It is used for information that is calculated using the values of the data itself like cyclic redundancy checks most common and lower layer protocols especially at the data link layer .

As data is passed down a protocol stack, headers and footers are nested. 

The header is found in most protocol messages and the footer is only found in some.

Three basic methods are used to address and transmit data between networked devices. 
A unicast transmission goes from one device to exactly one other. This is the most common method used for most message transactions. 
A broadcast transmission is sent from one device to all connected devices on a network. 
A multicast transmission is addressed and sent to a select group of devices. 

In some networks, only two devices are connected together, forming what is often called a point-to-point network. In this situation, everything sent by one device is implicitly intended for the other, so no addressing of messages is strictly necessary. 

The any-cast message is a new type of message addressing method that was defined as part of IPv6. This identifies a message that should be sent to the closest member of a group of devices.

Networks are configured to share resources using one of two basic structural models. 

In a peer-to-peer network, each device is equal and none are assigned particular jobs. It is simple and cost effective, used for smaller networks.

In a client-server network, devices are assigned roles. A small number of powerful computers are set up as servers and respond to request from other devices,which are clients. 
Client-server computing also refers to the interaction between complementary protocol elements and software programs. Advantages in the areas of performance, scalability, security, and reliability. 
The client-server structural model is dominant and becoming popular for even relatively small networks. It is the model used for the Internet. 

Client-server architecture is the basis for most TCP/IP protocols and service services. 

The term web browser is another name for a web client and a website really a web server.

Networks are often divided by size and general communication method into three classes. 
Local area networks (LANs) generally connect approximate devices usually using cables. Wireless LANS (WLANs) use radio frequency or light technology to connect devices without wires. 
Wide area networks connect distant devices or LANs to each other.
Campus area networks (CANs) and Metropolitan area networks (MANs) fall between LANs and WANs in terms of overall size. 
Personal area networks (PANs) are like very small LANs and often appear as wireless PANs (WPANs).

Several terms are used to describe the relative sizes of networks and parts of networks. 
The most basic term is network itself which can refer to most anything but often means a set of device is connected using an OSI layer 2 technology. 
A subnetwork is a part of a network or Internet network, as is a segment, though the latter often has a more specific meaning in certain technologies. 
Internetwork refers either genetically to a very large network, or specifically to a set of layer 2 networks connected using routers at layer 3.

Subnet and internet are abbreviations. Subnet can have a specific meaning in the context of TCP. Internet can be confused with the proper noun Internet.

Some LAN technologies including Ethernet use the term segment to refer to a collection of geographically proximate machines that are connected directly to each other either by a single cable or single device such as a hub. 

Such technologies have specific rules about how many devices can be on a segment how many segments can be connected together and so on.

In Ethernet, a segment used to refer to a specific cable. Earliest forms of Ethernet used coaxial cables, and the coaxial cable segment was shared and became the collision domain for the network. Collision domain refers to a collection of hardware devices in which only one can transmit at a time. devices like hubs and repeaters were used to extend collision domains by connecting together segments of cable into wider networks. Over time, the term collision domain and segment started to be used interchangeably. 

Today, a segment can refer either to a specific piece of cable or to a collection of cables connected electrically that represent a single collision domain.

The generic noun internet is a short form of the word internetwork, while the proper noun Internet refers to the global network of TCP/IP networks that we all know and use.
The term intranet refers to an internal network that uses TCP/IP technologies as the Internet does. 

An extranet is like an intranet that is extended to individuals or organisations outside a company. 
However, these terms are ambiguous.

Ch2 network performance issues and concepts

Increasing network performance costs money or compensating on nonperformance components, so it should not be done meaninglessly.

While performance is one of the most important characteristics of any network, there are others that are equally important. In many cases, you must weight the quality, reliability, expandability, maintainability, and other attributes of a network against overall performance. The faster want your network to go, the more difficult it is to ensure that these other attributes are kept at sufficiently high levels.

The three terms used most to refer to the overall performance of a network are speed, bandwidth, and throughput.
Speed is the most generic and often refers to the rated or nominal speed of a networking technology.
Bandwidth can mean either the width of the frequency bands used by a by technology, or more generally, data capacity, where it's used as more of a theoretical measure.
Throughput is a specific measure of how much data flows over a channel in a given period of time, it is usually a practical measurement.

Latency describes the nature of how data is conveyed. It describes the delay between the time that data is requested and the time when it arrives; the lag. 

An important issue closely related to latency is quality of service, a general term that refers, among other things, to the ability of networks to deliver necessary bandwidth and reliable data transfer for applications that need it.

Bytes can be called octets.

Capital B stands for bytes and little b for bits. This is not used consistently by everyone.

Bandwidth is almost always given in bits per second, bps, b/s. Throughput may sometimes be in Bytes/s. 

Networking speeds use the decimal, not binary, prefixes like kilo, mega, giga.

cps is character per second, a character is usually 1 byte, cps = Bps.

The baud and bits per second units are often treated equivalently but are not the same. Baud measures not the throughput of a network but it's signalling rate, the number of times the signal changes each second. Since modern encoding and modulation techniques often encode either greater or less than one bit value into each transition, throughput and baud rate of network technologies are usually different.

Benchmark programs used to measure throughputs can produce performance scores which usually have little to do with how a network will actually operate. Such measures are best used for comparison purposes. 

The difference between theoretical and practical performance can never be negligible. 
Every network has some degree of normal network overhead. Some bits sent are used to package and address data, some bits are used for general overhead activities and deal with collisions on transmissions and other issues. Any network transaction involves a number of different hardware and software layers, and overhead exist at each of them. These overheads mean that at least 20% of the rated speed of a LAN technology is lost.
External performance limiters include the ability of the hardware to process the data and also any bandwidth limitations that exist in the chain of data transmission. The entire network can run only as fast as it slowest link. 
Some technology do not always operate at a constant fixed speed, such as an analog modem which depends on the quality of the line over which it operates.
The third issue is misconfiguration. This is when slowdowns occur because hardware or software has not been set up correctly. like poor cabling, misconfigured interface guards,or bad drivers. 

Many tech technologies are asymmetric, offering higher speed of one direction than the other and often the larger number is the one that is advertised. Common tech technologies with asymmetric performance include 56K modems, asymmetric digital subscriber line (ADSL), cable modems, and satellite Internet.
Most communications, even though they seem unidirectional. Internet access technology often has much higher download bandwidth than upload bandwidth. When using TCP/IP to download data, acknowledgements must be sent and if the upstream band with this too low, this may make it impossible to fully exploit the download bandwidth of the link.

There are three basic operating modes that describe how data sent between connected devices on a network. 
In a Simplex operation, data can flow in only one direction between two devices.
Half duplex networks allow any device to transmit, but only one may do so at the time.
Full duplex operation means two attached devices can each transmit and receive simultaneously. This offers the greatest potential performance because forcing one device to wait for another before sending data does not decrease throughput.

The term quality of service (QoS) describes the characteristics of how data is transmitted between devices rather than how quickly it is sent. QoS features seek to provide more predictable streams of data rather than faster ones. Examples of such features include bandwidth reservation, latency minimums, traffic prioritisation and sharing, and congestion limitation. QoS is more important for specialty applications, such as multimedia, than for routine applications, such as those that transfer files or messages.

Many newer technologies have been developed to add QoS features to them. This includes the ability to support isochronous transmissions that can receive a specific amount of bandwidth over time to support real time transmissions. 
One technology that has received a lot of attention for its QoS features is asynchronous transfer mode (ATM).
Ethernet is not optimised of QoS features.


Ch3 network standards and standards organisations

Networking standards can be classified as proprietary, open or de facto. 
Proprietary standards are owned by one particular organisation. If that organisation has sufficient market cloud and the industry lacks alternatives to its standard, it may be adopted by the whole industry, becoming a de facto standard. Usually, however, differing proprietary standards compete with each other, resulting in fragmented market.

Open standards are not owned by anyone. They are created by neutral organisations to ensure that compatible products can be designed and developed by many different companies. This makes life easier for the customer and promotes the market as a whole.

Open standards are most successful.

List of standards organisations

International Organisation for Standardisation - ISO: one of the biggest standards organisations in the world; a Federation of standards organisations for many nations; known for its OSI reference model, chose the name ISO from the Greek word isos - equal

American National Standards Institute - ANSI: the main organisation responsible for coordinating and publishing computer information technology standards in the US; credits the organisations that actually create the standards, not developing and maintaining them; qualifying orgs. as Standards Developing Organisations or SDOs; publishes standards and documents created by the SDOs; serves as the US's representative to the ISO.

Information Technology Industry Council - ITIC: an SDO approved by ANSI to develop and process standards related to many computer related topics; formerly known as the Computer and Business Equipment Manufacturers Association (CBEMA)

National Committee for Information Technology - NCITS: established by the ITIC to develop and maintain standards related to IT; formerly known as Accredited Standards Committee X3 Information Technology or X3

Institute of Electrical and Electronics Engineers - IEEE, I triple E: created the IEEE 802 project, which contains many networking technologies like Ethernet.

Electronic Industries Alliance - EIA: an international industry association known for publishing electrical wiring and transmission standards.

Telecommunications Industry Association - TIA: the communication sector of the EIA, responsible for developing communication standards.
Standards produced by the EIA or TIA are often labelled with the combined pre EIA/TIA.

International Telecommunication Union - Telecommunication Standardisation Sector - ITU-T: large international body that develop standards for the telecommunications industry; formerly named the International Telephone and Telegraph Consultative Committee (CCITT, abbreviation is French)

European Telecommunication Standard Institute - ETSI: organisation with members for many countries both within and outside Europe, dedicated to developing telecommunication standards for the European market and elsewhere; known for regulating the use of radio bandwidth in Europe; developing standards such as HiperLAN.
Most of these are oversight organisations, they do not develop the standards themselves.

A group of related organisations is responsible for the development of TCP/IP standards and Internet technologies.
Internet society ISOC has overall responsibility for many Internet activities, including standard development. It oversees the Internet Architecture Board IAB, which makes high-level decisions about Internet technology development. Most of the actual work of creating current Internet standards is performed by the Internet Engineering Task Force IETF, which is managed by the Internet Engineering Steering Group IESG. Long-term research is done by the IETF's sibling organisation, the Internet Research Task Force IRTF, which is led by the Internet Research Steering Group IRSG.

Internet registration authorities are centralised organisations responsible for coordinating protocol parameters and globally assigned resources such as IP addresses. 
The first organisation was the Internet Assigned Numbers Authority IANA, which was initially in charge of IP assignment DNS domain name management, and protocol parameters. It was effectively one man - Jonathan B. Postel - one of the most important pioneers of Internet and TCP/IP technologies. Jon Postel ran ANA until his untimely death in 1998. 
Today, the Internet Corporation for Assigned Names and Numbers ICANN has overall responsibility for these activities; the IANA also operates under the auspices of ICANN and is still responsible for IP address assignment and parameter coordination.

in the original IP addressing scheme, addresses were assigned organisations directly by IANA in address blocks classes A, B, and C. Today, a hierarchical classless addressing system called Classless Inter-Domain Routing CIDR is used instead. IANA, as the organisation in charge of all IP addresses, assigns the largest blocks of addresses to regional Internet Registries RIRs that are responsible for further allocation activities. Each RIR manages IP addresses and other Internet number resources for particular region. 

The four regional registries are Asia Pacific Network Information Centre APNIC, American Registry for Internet Numbers ARIN, Latin American and Caribbean Internet Addresses Registry LACNIC, Résaux IP Européens Network Coordination Centre RIPE NCC.
Each registry may assign address blocks to Internet service providers directly or further delegate them to national Internet registries or local Internet registries.
Name registration is no longer a part of IANA's responsibilities, and ICANN has opened up the name registration business, so it is no longer the province of a single organisation such as InterNIC/NSI/VeriSign.

In the early days of the Internet, standardisation was achieved through building consensus through discussion about new technologies and protocols. If someone had an idea about a new idea, they would create a memorandum describing it and circulate it to others. These memos were called Requests for Comments. 

The documents defining early standards were originally called Internet Engineering Notes IENs before they were called RFCs.

The process of creating an RFC is formal organised. The IETF is a standard body that is most directly responsible for the creation of Internet standards. It's working groups, overseen by the IESG and the IAB, develop new protocols and technologies continuously, and these developments are formalises in RFCs.
The office of the RFC Editor handles the publishing of RFCs. The RFC editor was Internet pioneer John Postel until his death and then the function was assigned to the networking division of the USC Information Sciences Institute ISI, where Jon Postel was a director.
Access to RFCs is free and open.

Internet standards are described in a series of documents called Requests for Comments RFCs. 
The RFC process describes how an Internet standard is usually created. An idea for technology enhancement begins with the creation of an Internet draft ID. After review and feedback, if the proposal has support, it may be placed on the Internet standard track, and its status will be changed to proposed standard. As the fledging standard matures, status may advance to draft standard and eventually, Internet standard
However many RFCs are implemented in products without reaching Internet standard status. There are also other RFCs that define experimental technologies or provide information without describing official Internet standards.

Ch4 data repr

Setting a bit is changing it to one; resetting or clearing a bit is changing it to 0.

Number of bits : common representation terms
1: bit/digit/flag
4: nybble/nibble
8: byte/octet/character
16: double byte/word
32: double word/long word
64: very long word

Formally, an octet is the correct term for exactly 8 bits, while a byte is the smallest number of bits that can be accessed in the computer system, which may or may not equal 8. In practice, modern computers use eight bit bytes and the terms are used interchangeably, with bytes being more common in North America and octet being preferred in Europe.

The term hexadecimal was not the first name used for base 16 numbers in computing. Originally, these were called sexadecimal numbers. This is actually the correct term since the Latin prefixes (sexa-) are normally used for numbers not, Greek ones (hexa-). However, in the early 1950s, IBM decided that the word sexadecimal was just a little too provocative for their taste, so they changed it to hexadecimal. IBM being IBM - especially back then - meant everyone else followed suit.

Hex numbers use prefix 0x or suffix h.

OR sets bits, AND clears bits, XOR inverts bits in but masking.


Part 2 OPEN SYSTEMS INTERCONNECTION REFERENCE MODEL

Ch5 General OSI RM issues and concepts

The Open Systems Interconnection Reference Model (OSI Reference Model or OSI model) was originally created as the base for designing a universal sets of protocols called OSI protocol suite. This suite never achieved widespread success, but the model became a very useful tool for both education and development. The model defines a set of layers and a number of concepts for their use that makes understanding networks easier. 

It was published in 1984 by the ISO as standard ISO 7498 and the ITU-T as standard X.200.

The model is theoretical, but its concepts are employed regularly to describe the operation of real-world networks.


The most fundamental concept in the OSI reference model is the division of networking functions into a set of layers, from layer 1 at the bottom to layer 7 at the top.
As you go down the layer stack, you move away from concrete, hardware-specific functions to ones that are increasingly abstract until you reach the realm of user applications at layer 7.
The seven layers are sometimes divided into grouping: the lower layers 1 through 3, and the upper layers 4 through 7. There is some disagreement on whether layer 4 is a lower or upper layer.

From 1 to 7, the layers are: physical, data link, network, transport, session, presentation, application.

The four lower layers of the OSI model are most often discussed individually because the boundaries between them are reasonably clear-cut. In contrast, the lines between the session, presentation, and application layers are somewhat blurry. As a result, sometimes the protocol span 2 or even all 3 of these layers. This is especially true for TCP/IP application protocols, since the TCP/IP model three layers 5-7 as a single layer.

Some of the layers are divided into sublayers, this is commonly done at the lower layers.

Layers are referred to in a variety of ways: they may have their name spelt out in full, they may be abbreviated, or simply referenced by their layer number. 

N is used to genetically refer to a number within the computer world. 

It can be used to generically refer to a layer number and describe relationships between layers like layer N+1, N-1.

Layer names and numbers are often used as adjectives to describe protocols and technologies.

A protocol represents communication between logical or physical devices of the same layer of the model. Interface represents information moving between adjacent layers within the same device. A network stack or protocol stack is a set of layers in a model or suite of technologies, or a partial set.

Entities and functions are specific operations or jobs done at layer N.

Facilities and services are what a layer provides to the layers above it. The N+1 layer uses a set of N services or N facilities provided by the N layer.

Interfaces are for communicating vertically between the layers within a particular host. Notation example: the layer 2/3 interface is used by a layer two and layer three protocol to pass data and control information.

Vertical communication is done up and down the protocol stack every time anything is sent across a network because higher levels are implemented as logical functions and software and there is no actual physical connection.

The existence of well defined interfaces between layers is what permits a higher layer to use the services of any number of lower layer layers without requiring knowledge of how those layers are implemented.

In the OSI reference model, a protocol refers specifically to a set of rules or procedures that define communication between software or hardware elements running at the same layer on network devices.

Physical layer protocols are responsible for the actual transmission and reception of data at layer one, protocols at higher layer layers pass data down through the layers below them to layer one for transmission, then across the network and back up to the corresponding entity at the same layer on the receiving device. The result is that software processes running at, say, layer 4 on each of two devices can communicate logically as if they were directly connected at layer 4, even though they are not.


The message used to communicating information for a particular protocol is called its protocol data unit PDU. That PDU is passed down to the next lower layer for transmission. Since that layer is providing the service of handling that PDU, it is called the lower layer's Service Data Unit SDU. SDU is in encapsulated into that layer's own PDU and, in turn, sent to the next lower layer in the stack, proceeding until the physical layer is reached. The process is reversed on the recipient device. 

A layer N PDU is a layer N-1 SDU, which is encapsulated into a layer N-1 one PDU.

The process of routing occurs when data is sent not directly from transmitter to ultimate recipient, but indirectly through the use of an intermediate system. That device, called a router, connects two or more physical networks, thus has multiple interfaces to layer 2. When it receives data, the data passes up only to the network layer where it is repackaged and then sent on the next leg of its journey over the appropriate layer 2 interface.


Ch6 osi rm layers 

Layer 1, Physical layer, PHY
responsible for networking hardware specifications and is the place where technologies that perform data encoding, signalling, transmission, and reception functions reside. The physical layer is closely related to the data link layer.
Also called transport method.


Layer 2, Data link layer, link layer, DLL
where most LAN and WLAN technologies are defined. Responsible for Logical Link Control LLC, Media Access Control MAC, hardware addressing (hardware/MAC address), error correction and handling (CRC), and defining physical layer standards. Divided into LLC and MAC sublayers based on IEEE 802 project arhitecture.

Protocols - Ethernet, Token Ring, FDDI (+CDDL), IEEE 802.11, HomePNA, ATM, TCP/IP's Serial Line Interface Protocol SLIP, Point-to-Point Pryocol PPP.

Hardware - Network interface cards, bridges, switches, brouters

LLC - establishment and control of logical links between local devices on a network, sublayer creating abstraction. Most LAN tech use IEEE 802.2 LLC protocol

MAC - controlling access of devices to the network medium. Ethernet uses (used?) CSMA/CD, Token Ring uses token passing.


Layer 3, Network layer
responsible for the tasks that link together networks into internetworks. Functions include internetwork-level addressing, routing, datagram encapsulation, fragmentation and reassembly, certain types of errorhandling and diagnostics. 

Most common layer 3 protocol is IP. Others that work with it are IPsec, IP NAT, Mobile IP. Internet Control Message Protocol ICMP is the main error-handling and conteol protocol.
Other than IP there is also Novell Internetworking Packet Exchange (IPX) protocol.

Hardware - routers, brouters, layer 3 switches

Layer 4, Transport layer
Represents the transition point between the lower layers that deal with data delivery issues and the higher ones that work with application software. Responsible for enabling end-to-end (host-to-host) communication between application processes, which accomplishes through the use of process level addressing and multiplexing/demultiplexing. Transport layer protocols are responsible for segmenting application data into blocks for transmission and may be either connection-oriented or connectionless. protocols at this layer also often provide data to delivery management services such as reliability and flow control. (avknowledgements / retransmission timers)

Layers 3 and 4 are closely connected. Common protocol stacks are often named after the layer three and four protocols in the suite, for example TCP/IL or the Novell NetWate suite called IPX/SPX. They normally come in pairs.

Protocols: TCP and UDP from TCP/IP, SPX from NetWare, NetBEUI from NetBIOS/NetBEUI/NBF


Layer 5, Session
provides functions for establishing and managing sessions between software processes. Session technologies are often implemented as a set of software tools called application program interfaces (APIs), which provide a consistent set of services that allow programmers to develop networking applications without needing to worry about lower-level details of transport, addressing and delivery.


Layer 6, Presentation
takes care of manipulation tasks that transform data from one representation to another, such as translation, compression, and encryption. In many cases, no such functions are required in a particular networking stack; if so, there may not be any protocol active at layer 6, so layer 7 may deal with layer 5.

An encryption scheme associated with the presentation layer is secure socket layer SSL protocol. Somee encryption is done at lower levels in the protocol sack in technologies such as IPsec.


Layer 7, Application
define application protocols that implement specific user applications and other high-end functions protocols include HTTP, FTP, SMTP, DHCP, NFS, Telnet, SNMP, POP3, NNTP, IRC.



PART 3 TCP/IP PROTOCOL SUITE AND ARCHITECTURE

Ch8
TVP/IP was initially developed in the 1970s as a part of an effort to define the set of technologies to operate the ARPAnet, a research network developed by the United States Defence Advanced Research Projects Agency in 1973. They began developing a system of internetworking protocols to account for a potentiom increase in size of the network. 

The first version of TCP was written in 1973 and revised and documented in RFC 675, Specification of Internet Transmission Control Program, published in December 1974. Version two came out in March 1977.

In August 1977, Jon Postel published a set of comments on the state of TCP in the document known as Internet Engineering Note number two or IEN2. He stated that the version of TCP was trying to do too much, abandoning the principle of layering, essentially, by encompassing both OSI layers 3 and 4 activities. That redefined TCP/IP architecture and in 1978, version three of TCP came out, where the process dividing TCP into two portions started.

TCP was split into Transmission Control Protocol TCP and Internet Protocol IP, first modern version of these two key protocols were documented in the 1980 as TCP version four and IP version four respectively.


Some factors that led to TCP/IP's success include its technical features, such as routing-friendly design and scalability, its historical role as the protocol suite of the Internet, and iys open standards and development process, which reduce barriers to acceptance of TCP/IP protocols. 

The TCP/IP protocol suite is oriented around the notion of client/server network communication. Rather than all devices and protocol software elements being designed as peers, they are constructed as matched sets. Clients normally initiate communication by sending requests, and servers respond to such requests, providing the client with the desired data or an informative reply. 

The terms client and server can refer to hardware roles – designation is given to hardware devices based on whether they usually function as clients or servers. The terms can also refer to software roles, meaning whether protocol software component function as clients or servers. And they can refer to transactional roles, meaning whether a device and program functions as a client or server in any given exchange of data. 

With the rise of powerful personal computers and widespread Internet access, especially always-on broadband connectivity, the boundary between client and server hardware and software has become blurred. Many client machines now include server software that allows them to respond to World Wide Web queries for other clients. Also, many file-sharing programs allow clients to communicate using the perr-to-perr structural model. However, most TCP/IP communication is still client/server. 

The architecture of the TCP/IP protocol suites are often described in terms of a layered reference model called the TCP/IP model, DARPA model, or DoD model. TCP/IP was developed before the OSI reference model.

The TCP/IP model includes four layers: 

Network interface layer; link layer; network access layer
responsible for interfacing the suite to the physical hardware on what runs
on many networks, there is no TCP/IP protocol running at all on this layer because it is not needed. For example, if you run TCP/IP over Ethernet, then Ethernet handles layer 1 and layer 1 functions. However, the TCP/IP standards do define protocols for TCP/IP networks that do not have their own  layer 2 implementations. These protocols, the Serial Line Internet Protocol (SLIP) and the Point-to-Point protocol (PPP), fill the gap between the network layer and the physical layer. They are used to facilitate TCP/IP over direct serial line connections, such as dial up telephone networking, and other technologies that operate directly at the physical layer.

Internet layer; network layer;
where device addressing, basic data ground communication, and routing take place
IP, IPv6, and also support protocols such as the Internet Control Message Protocol (ICMP) and the routing protocols (RIP, OSFB, BGP, and so on).

Host-to-host transport layer
where connections are managed and reliable communication is insured
allows logical connections to be made between devices that allow data to be sent other unreliably, with no guarantee that it gets there, or reliably, where the protocol keeps track of the data sent and received in order to make sure it arrives, and resend it if necessary.
Key protocols at this layer are TCP and UDP.
includes certain elements that are arguably part of the OSI session layer; for example, TCP establishes a connection that can persist for a long period of time, which makes it more like a session.

Application layer
where end user applications and services reside
Application protocols such as HTTP, FTP, SMTP for providing and user services as well as administrative protocols like simple network management protocol (SNMP), dynamic host configuration protocol (DHCP), And domain name system

The first three layers correspond to layers two through four of the OSI reference model respectively; the application layer is equivalent to OSI layers 5 to 7.



A summary of each of the TCP/IP protocols: 

Network interface layer 

1. Serial line Internet protocol, SLIP
Provides basic TCP/IP functionality by creating a layer to connection between two devices over a serial line 

2. Point to point protocol, PPP
Provides layer to connectivity, which is much more sophisticated and capable. PPP itself as a suite of protocols that's allow for functions such as authentication data capitulation encryption and aggregation thereby facilitating TCP/IP operation over WAN links.

Network interface layer/Internet

1. Address resolution protocol, ARP
Used to map layer 3 IP address addresses to layer 2 physical network addresses 

2. reverse address resolution protocol, RARP.
Determines the layer three address of a machine from a layer to address. Now mostly superseded by BOOTP and DHCP. 

Internet layer 

1. Internet protocol, IPv6
Provide encapsulation and connections delivery of transport layer messages over TCPIP network. Also responsible for addressing and routing functions. 

2. IP network address translation, IPNAT. 
Allows addresses on a private network to be automatically translated to different addresses on a public network, thereby providing address sharing and security benefits 

3. IP security, IPsec
A set of IP related protocol that improve the security of IP transmissions 

4. Internet protocol mobility support, mobile IP
Resolves certain problems with IP associated with mobile devices.

5. Internet control message protocol, ICMP 
A support protocol for IP and IP V6 that provides error reporting and information request and reply capabilities to hosts

6. Neighbour discovery protocol, NDP
A new support protocol for IP6 that includes several functions performed by ARP and ICMP and conventional IP. 

7. routing information protocol RIP, open shortest path first OSPF, gateway to gateway protocol GGP, HELLO protocol, interior gateway routing protocol IGRP, enhanced interior Gateway routing protocol EIGRP, border gateway protocol BGP, exterior gateway protocol EGP
Protocols used to support the routing of IP data grounds and the exchange of routing information.

Host to host transport layer 

1. Transmission control protocol, TCP. 
The main transport layer protocol for TCP/IP. establishes a managers connections between devices and reliable and Flo controlled delivery of data using IP. 

2. User datagram protocol, UDP
A transport protocol that can be considered a severely stripped version of TCP. It is used to send data in a simple way between application processes without many reliability and flow management features of TCP but often with greater efficiency. 

Application layer
1. Domain name system, DNS
Provides the ability to refer to IP devices using names instead of just numerical IP addresses allows machines to resolve these names into their corresponding IP addresses. 

2. Network file system NFS. 
Allows files to be shared seamlessly across TCP/IP networks 

3. Boots strap protocol, BOOTP
Developed to address some of the issues with RARP and used in a similar manner: to allow the configuration of a TCP/IP device that startup. generally superseded by DHCP

4. dynamic house configuration protocol, DHCP
A complete protocol for configuring TCP/IP devices and managing IP addresses the successor to RARPNBOOTP, it includes numerous features and capabilities. 

five simple network management protocol, SNMP
A full featured protocol for remote management of networks and devices.

Six remote monitoring, RMON
A diagnostic protocol, really a part of SNMP, used for remote monitoring of network devices

Seven file transfer protocol, trivial file transfer protocol, FTP, TFTP
Protocols designed to permit the transfer of all types of files from one device to another

RFC 822, multipurpose Internet mail extensions MIME, simple mail transfer protocol SMTP, post office protocol POP, Internet message access protocol IMAP
Protocols that define the formatting delivery and storage of email messages on TCP/IP networks 


Network news transfer protocol, NNTP
Enables the operation of the use that online community by transferring used netnews messages between hosts

10 hypertext transfer protocol HTTP
Transfers hyper tax documents between hosts; implement the worldwide web

Golfer protocol
An older documents retrieval protocol now are largely replaced by the worldwide

tell protocol
Allows a user on one machine to establish a remote terminal sessions on another

Berkeley art commands
Permit commands in operations on one machine to be performed on another

Internet relay chat, I RC
Allows real time chatting between TCP/IP users.

Administration and troubleshooting utilities and protocols.
A collection of software tools that allows administrators to manage, configure, and troubleshoot TCP/IP internetworks 