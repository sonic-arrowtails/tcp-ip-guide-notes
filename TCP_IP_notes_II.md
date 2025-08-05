Ch9 SLIP and PPP

SLIP and PPP provide layer 2 connectivity for TCP/IP implementations that run directly over a physical layer link without a layer 2 technology. While SLIP is simpler, PPP is favoured due to its many features and capabilities.


PPP and SLIP cost about the same.

Both are designed for connections between just two devices; thus, the name point to point protocol
Since there are only two devices, the protocols do not have to manage complexities like media access control, collisions, and unique addressing schemes in the way that technologies like ethernet must.

PPP can be used for protocols other than IP, which is why some people don't consider SLIP and BPP to be part of the true TCP/IP protocol suite 

Serial Line Internet Protocol
SLIP has never been defined as a formal standard. It was created in formally in the early 1980s and it became a de facto standard before it was ever described in an RFC. When it was published in 1988 as RFC 1055, "a Nonstandard for Transmission of IP Datagrams over Serial Lines: SLIP"

SLIP provides a layer 2 framing service for IP datagrams but no other features or capabilities.

SLIP sends the datagram one byte at a time, then ends it with a SLIP END character, byte value 192 (0xCO). In better inplementations, END is also used to precede the datagram to separate it from any line noise that came before it.

SLIP ESC Escape char has value 219 (0xDB)

To send the value of character 192, replace it with ESC 220 (219 220) (DB DC)

To send the value of charcater 219, send 219 221


SLIP is most deficient in the following areas:


Standardised datagram size specification: Maximum supported datagram size is not standardised and depends on each implementation. The usual default is 1006 by which becomes the maximum transmission unit for the length. If a different size is used it has to be programmed into the IP layer. 

Error detection and correction mechanism: I was all detective only after an entire day around has been sent and passed back up the stack at the recipient error. Correction can only come in the form of resending any daragrams that were corrupted. 

Control messaging: there is none.

Type identification: since SLIP includes no headers of its own, it's not possible to identify that it's being used. it may or may not use IP however without type identification there's no way to mix day grounds from two or more layer three protocols on the same link. 

Address delivery method: addressing is not needed because it is a point to point connection however device devices do need some way of learning each other's IP addresses for a routing at layer 3FLIP provide provides no method for this 

support for compression: none however some modes usually supports compression at layer one for serial connections that use them.
A new variant of SLIP called compressed SLIP or CSLIP was created in the late 1980s but it was not as widely deployed as regular SLIP

Security features: none. no authentication or encryption.


Point-to-Point Protocol
even as SLIP was being documented, work is underway on a new protocol that would provide full featured IP transmission over direct links between pairs of devices well most often associated with dialogue mode use, PPP can run across any similar type of physical layering, for example, it is often used to provide layer to functionality on integrated services digital network (ISDN).

It is really more a protocol sweet since its operation is based on procedures defined as many individual protocols.

The first form of IETF document related to PPP was RFC 1134 in 1989. this was not the standard itself with a proposal for it would eventually be defined as the first main PPP standard, RFC 1171 in 1990. It was revised several times and several other documents were added to it to define the various protocol that composed the entire PPP suite.

Rather than try to develop PPP from scratch, the IETF decided to base it on the ISO high-level data link control (HDLC) protocol, which was initially developed by IBM. HDLC is a derivative of the synchronous data link control (SDLC) protocol.

PPP is a connection oriented protocol that enables layer two links over a variety of different physical layer connections. It is supported on both synchronous and a synchronous lines and can operate in half duplex or full duplex mode.

some benefits include the following:
A more comprehensive framing mechanism; specification of the encapsulated protocol to allow multiple day or three protocols to be MultiLex on a single link; error detection for each transmitted frame through the use of a cyclic redundancy check code in each frame header;a robust mechanism for negotiating a link parameters, including the maximum freight size permitted; a method for testing links before datagram transmission takes place and for monitoring link quality;
support for authentication of the connection using multiple authentication protocols; support for additional optional features including compression encryption and link aggregation allowing two devices to use multiple physical links as if they were a single higher performance link


PPP successes lead even to the development of derivative protocols like PPP over ethernet PPPOE and PPP over ATMPPPOA these derivatives actually layer PPP over existing data link layer tech technologies


