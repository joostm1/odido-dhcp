# odido-dhcp
## DHCP sequence Zyxel device and Dutch internet provider Odido - previously T-Mobile.

Here's the DHCP sequence for obtaining the IP address for the internet link (VLAN ID 100):


## [DHCP Discover](https://github.com/joostm1/odido-dhcp/tree/main#dhcp-discover)
## [DHCP Offer](https://github.com/joostm1/odido-dhcp/tree/main#dhcp-offer)
## [DHCP Request](https://github.com/joostm1/odido-dhcp/tree/main#dhcp-request)
## [DHCP ACK](https://github.com/joostm1/odido-dhcp/tree/main#dhcp-ack)

# DHCP Discover
    Frame 362: 594 bytes on wire (4752 bits), 594 bytes captured (4752 bits)
        Encapsulation type: Ethernet (1)
        Arrival Time: Sep 21, 2023 12:18:32.626530000 W. Europe Summer Time
        [Time shift for this packet: 0.000000000 seconds]
        Epoch Time: 1695291512.626530000
        [Time delta from previous captured frame: 0.029200000 seconds]
        [Time delta from previous displayed frame: 0.000000000 seconds]
        [Time since reference or first frame: 106.586809000 seconds]
        Frame Number: 362
        Frame Length: 594 bytes (4752 bits)
        Capture Length: 594 bytes (4752 bits)
        [Frame is marked: False]
        [Frame is ignored: False]
        [Protocols in frame: eth:ethertype:vlan:ethertype:ip:udp:dhcp]
        [Coloring Rule Name: UDP]
        [Coloring Rule String: udp]
    Ethernet II, Src: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
        Destination: Broadcast (ff:ff:ff:ff:ff:ff)
        Source: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4)
        Type: 802.1Q Virtual LAN (0x8100)
    802.1Q Virtual LAN, PRI: 0, DEI: 0, ID: 100
        Internet Protocol Version 4, Src: 0.0.0.0, Dst: 255.255.255.255
        0100 .... = Version: 4
        .... 0101 = Header Length: 20 bytes (5)
        Differentiated Services Field: 0x00 (DSCP: CS0, ECN: Not-ECT)
        Total Length: 576
        Identification: 0x0000 (0)
        000. .... = Flags: 0x0
        ...0 0000 0000 0000 = Fragment Offset: 0
        Time to Live: 64
      Protocol: UDP (17)
        Header Checksum: 0x78ae [validation disabled]
        [Header checksum status: Unverified]
        Source Address: 0.0.0.0
        Destination Address: 255.255.255.255
      User Datagram Protocol, Src Port: 68, Dst Port: 67
        Source Port: 68
        Destination Port: 67
        Length: 556
        Checksum: 0x73e9 [unverified]
        [Checksum Status: Unverified]
        [Stream index: 4]
        [Timestamps]
        UDP payload (548 bytes)
    Dynamic Host Configuration Protocol (Discover)
        Message type: Boot Request (1)
        Hardware type: Ethernet (0x01)
        Hardware address length: 6
        Hops: 0
        Transaction ID: 0xf4012537
        Seconds elapsed: 0
        Bootp flags: 0x0000 (Unicast)
        Client IP address: 0.0.0.0
        Your (client) IP address: 0.0.0.0
        Next server IP address: 0.0.0.0
        Relay agent IP address: 0.0.0.0
        Client MAC address: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4)
        Client hardware address padding: 00000000000000000000
        Server host name not given
        Boot file name not given
        Magic cookie: DHCP
        Option: (53) DHCP Message Type (Discover)
        Option: (60) Vendor class identifier
           Length: 8
           Vendor class identifier: DX5401B0
        Option: (55) Parameter Request List
           Length: 7
           Parameter Request List Item: (1) Subnet Mask
           Parameter Request List Item: (3) Router
           Parameter Request List Item: (6) Domain Name Server
           Parameter Request List Item: (12) Host Name
           Parameter Request List Item: (15) Domain Name
           Parameter Request List Item: (28) Broadcast Address
           Parameter Request List Item: (43) Vendor-Specific Information
        Option: (255) End
           Option End: 255
        Padding: 000000000000000000000000000000000000000000000000000000000000000000000000…
        
        
# DHCP Offer
    Frame 364: 372 bytes on wire (2976 bits), 372 bytes captured (2976 bits)
        Encapsulation type: Ethernet (1)
        Arrival Time: Sep 21, 2023 12:18:32.646764000 W. Europe Summer Time
        [Time shift for this packet: 0.000000000 seconds]
        Epoch Time: 1695291512.646764000
        [Time delta from previous captured frame: 0.002370000 seconds]
        [Time delta from previous displayed frame: 0.020234000 seconds]
        [Time since reference or first frame: 106.607043000 seconds]
        Frame Number: 364
        Frame Length: 372 bytes (2976 bits)
        Capture Length: 372 bytes (2976 bits)
        [Frame is marked: False]
        [Frame is ignored: False]
        [Protocols in frame: eth:ethertype:vlan:ethertype:ip:udp:dhcp]
        [Coloring Rule Name: UDP]
        [Coloring Rule String: udp]
      Ethernet II, Src: Atrie_00:00:02 (00:0e:00:00:00:02), Dst: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4)
        Destination: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4)
           Address: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4)
           .... ..0. .... .... .... .... = LG bit: Globally unique address (factory default)
           .... ...0 .... .... .... .... = IG bit: Individual address (unicast)
        Source: Atrie_00:00:02 (00:0e:00:00:00:02)
        Type: 802.1Q Virtual LAN (0x8100)
      802.1Q Virtual LAN, PRI: 6, DEI: 0, ID: 100
        110. .... .... .... = Priority: Internetwork Control (6)
        ...0 .... .... .... = DEI: Ineligible
        .... 0000 0110 0100 = ID: 100
      Type: IPv4 (0x0800)
        Internet Protocol Version 4, Src: 10.68.0.2, Dst: 10.68.211.232
        0100 .... = Version: 4
        .... 0101 = Header Length: 20 bytes (5)
        Differentiated Services Field: 0xc0 (DSCP: CS6, ECN: Not-ECT)
        Total Length: 354
        Identification: 0xb1c6 (45510)
        000. .... = Flags: 0x0
        ...0 0000 0000 0000 = Fragment Offset: 0
        Time to Live: 128
        Protocol: UDP (17)
        Header Checksum: 0x9e92 [validation disabled]
        [Header checksum status: Unverified]
        Source Address: 10.68.0.2
        Destination Address: 10.68.211.232
      User Datagram Protocol, Src Port: 67, Dst Port: 68
        Source Port: 67
        Destination Port: 68
        Length: 334
        Checksum: 0x702d [unverified]
        [Checksum Status: Unverified]
        [Stream index: 5]
        [Timestamps]
        UDP payload (326 bytes)
    Dynamic Host Configuration Protocol (Offer)
        Message type: Boot Reply (2)
        Hardware type: Ethernet (0x01)
        Hardware address length: 6
        Hops: 0
        Transaction ID: 0xf4012537
        Seconds elapsed: 0
        Bootp flags: 0x0000 (Unicast)
        Client IP address: 0.0.0.0
        Your (client) IP address: 10.68.211.232
        Next server IP address: 0.0.0.0
        Relay agent IP address: 0.0.0.0
        Client MAC address: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4)
        Client hardware address padding: 00000000000000000000
        Server host name not given
        Boot file name not given
        Magic cookie: DHCP
        Option: (53) DHCP Message Type (Offer)
           Length: 1
           DHCP: Offer (2)
        Option: (54) DHCP Server Identifier (10.68.0.2)
           Length: 4
           DHCP Server Identifier: 10.68.0.2
        Option: (51) IP Address Lease Time
           Length: 4
           IP Address Lease Time: 1 hour (3600)
        Option: (1) Subnet Mask (255.255.0.0)
           Length: 4
           Subnet Mask: 255.255.0.0
        Option: (3) Router
           Length: 4
           Router: 10.68.0.1
        Option: (6) Domain Name Server
           Length: 8
           Domain Name Server: 62.58.48.20
           Domain Name Server: 37.143.84.228
        Option: (15) Domain Name
           Length: 20
           Domain Name: ftth.glasoperator.nl
        Option: (43) Vendor-Specific Information
           Length: 24
           Value: 012e687474703a2f2f31302e31322e302e31303a37353437
        Option: (255) End
           Option End: 255
        
           
        0000   d4 1a d1 74 ac d4 00 0e 00 00 00 02 81 00 c0 64   ...t...........d
        0010   08 00 45 c0 01 62 b1 c6 00 00 80 11 9e 92 0a 44   ..E..b.........D
        0020   00 02 0a 44 d3 e8 00 43 00 44 01 4e 70 2d 02 01   ...D...C.D.Np-..
        0030   06 00 f4 01 25 37 00 00 00 00 00 00 00 00 0a 44   ....%7.........D
        0040   d3 e8 00 00 00 00 00 00 00 00 d4 1a d1 74 ac d4   .............t..
        0050   00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00   ................
        0060   00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00   ................
        0070   00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00   ................
        0080   00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00   ................
        0090   00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00   ................
        00a0   00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00   ................
        00b0   00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00   ................
        00c0   00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00   ................
        00d0   00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00   ................
        00e0   00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00   ................
        00f0   00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00   ................
        0100   00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00   ................
        0110   00 00 00 00 00 00 00 00 00 00 63 82 53 63 35 01   ..........c.Sc5.
        0120   02 36 04 0a 44 00 02 33 04 00 00 0e 10 01 04 ff   .6..D..3........
        0130   ff 00 00 03 04 0a 44 00 01 06 08 3e 3a 30 14 25   ......D....>:0.%
        0140   8f 54 e4 0f 14 66 74 74 68 2e 67 6c 61 73 6f 70   .T...ftth.glasop
        0150   65 72 61 74 6f 72 2e 6e 6c 2b 18 01 2e 68 74 74   erator.nl+...htt
        0160   70 3a 2f 2f 31 30 2e 31 32 2e 30 2e 31 30 3a 37   p://10.12.0.10:7
        0170   35 34 37 ff                                       547.
        
        
# DHCP Request
    Frame 365: 594 bytes on wire (4752 bits), 594 bytes captured (4752 bits)
        Encapsulation type: Ethernet (1)
        Arrival Time: Sep 21, 2023 12:18:32.655570000 W. Europe Summer Time
        [Time shift for this packet: 0.000000000 seconds]
        Epoch Time: 1695291512.655570000
        [Time delta from previous captured frame: 0.008806000 seconds]
        [Time delta from previous displayed frame: 0.008806000 seconds]
        [Time since reference or first frame: 106.615849000 seconds]
        Frame Number: 365
        Frame Length: 594 bytes (4752 bits)
        Capture Length: 594 bytes (4752 bits)
        [Frame is marked: False]
        [Frame is ignored: False]
        [Protocols in frame: eth:ethertype:vlan:ethertype:ip:udp:dhcp]
        [Coloring Rule Name: UDP]
        [Coloring Rule String: udp]
      Ethernet II, Src: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
        Destination: Broadcast (ff:ff:ff:ff:ff:ff)
           Address: Broadcast (ff:ff:ff:ff:ff:ff)
           .... ..1. .... .... .... .... = LG bit: Locally administered address (this is NOT the factory default)
           .... ...1 .... .... .... .... = IG bit: Group address (multicast/broadcast)
        Source: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4)
           Address: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4)
           .... ..0. .... .... .... .... = LG bit: Globally unique address (factory default)
           .... ...0 .... .... .... .... = IG bit: Individual address (unicast)
        Type: 802.1Q Virtual LAN (0x8100)
      802.1Q Virtual LAN, PRI: 0, DEI: 0, ID: 100
        000. .... .... .... = Priority: Best Effort (default) (0)
        ...0 .... .... .... = DEI: Ineligible
        .... 0000 0110 0100 = ID: 100
        Type: IPv4 (0x0800)
      Internet Protocol Version 4, Src: 0.0.0.0, Dst: 255.255.255.255
        0100 .... = Version: 4
        .... 0101 = Header Length: 20 bytes (5)
        Differentiated Services Field: 0x00 (DSCP: CS0, ECN: Not-ECT)
        Total Length: 576
        Identification: 0x0000 (0)
        000. .... = Flags: 0x0
        ...0 0000 0000 0000 = Fragment Offset: 0
        Time to Live: 64
        Protocol: UDP (17)
        Header Checksum: 0x78ae [validation disabled]
        [Header checksum status: Unverified]
        Source Address: 0.0.0.0
        Destination Address: 255.255.255.255
      User Datagram Protocol, Src Port: 68, Dst Port: 67
        Source Port: 68
        Destination Port: 67
        Length: 556
        Checksum: 0xf698 [unverified]
        [Checksum Status: Unverified]
        [Stream index: 4]
        [Timestamps]
        UDP payload (548 bytes)
      Dynamic Host Configuration Protocol (Request)
        Message type: Boot Request (1)
        Hardware type: Ethernet (0x01)
        Hardware address length: 6
        Hops: 0
        Transaction ID: 0xf4012537
        Seconds elapsed: 0
        Bootp flags: 0x0000 (Unicast)
        Client IP address: 0.0.0.0
        Your (client) IP address: 0.0.0.0
        Next server IP address: 0.0.0.0
        Relay agent IP address: 0.0.0.0
        Client MAC address: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4)
        Client hardware address padding: 00000000000000000000
        Server host name not given
        Boot file name not given
        Magic cookie: DHCP
        Option: (53) DHCP Message Type (Request)
           Length: 1
           DHCP: Request (3)
        Option: (60) Vendor class identifier
           Length: 8
           Vendor class identifier: DX5401B0
        Option: (50) Requested IP Address (10.68.211.232)
           Length: 4
           Requested IP Address: 10.68.211.232
        Option: (54) DHCP Server Identifier (10.68.0.2)
           Length: 4
           DHCP Server Identifier: 10.68.0.2
        Option: (55) Parameter Request List
           Length: 7
           Parameter Request List Item: (1) Subnet Mask
           Parameter Request List Item: (3) Router
           Parameter Request List Item: (6) Domain Name Server
           Parameter Request List Item: (12) Host Name
           Parameter Request List Item: (15) Domain Name
           Parameter Request List Item: (28) Broadcast Address
           Parameter Request List Item: (43) Vendor-Specific Information
        Option: (255) End
           Option End: 255
        Padding: 000000000000000000000000000000000000000000000000000000000000000000000000…
        
# DHCP Ack
    Frame 369: 372 bytes on wire (2976 bits), 372 bytes captured (2976 bits)
        Encapsulation type: Ethernet (1)
        Arrival Time: Sep 21, 2023 12:18:32.677168000 W. Europe Summer Time
        [Time shift for this packet: 0.000000000 seconds]
        Epoch Time: 1695291512.677168000
        [Time delta from previous captured frame: 0.006601000 seconds]
        [Time delta from previous displayed frame: 0.021598000 seconds]
        [Time since reference or first frame: 106.637447000 seconds]
        Frame Number: 369
        Frame Length: 372 bytes (2976 bits)
        Capture Length: 372 bytes (2976 bits)
        [Frame is marked: False]
        [Frame is ignored: False]
        [Protocols in frame: eth:ethertype:vlan:ethertype:ip:udp:dhcp]
        [Coloring Rule Name: UDP]
        [Coloring Rule String: udp]
      Ethernet II, Src: Atrie_00:00:02 (00:0e:00:00:00:02), Dst: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4)
        Destination: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4)
           Address: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4)
           .... ..0. .... .... .... .... = LG bit: Globally unique address (factory default)
           .... ...0 .... .... .... .... = IG bit: Individual address (unicast)
        Source: Atrie_00:00:02 (00:0e:00:00:00:02)
           Address: Atrie_00:00:02 (00:0e:00:00:00:02)
           .... ..0. .... .... .... .... = LG bit: Globally unique address (factory default)
           .... ...0 .... .... .... .... = IG bit: Individual address (unicast)
        Type: 802.1Q Virtual LAN (0x8100)
      802.1Q Virtual LAN, PRI: 6, DEI: 0, ID: 100
        110. .... .... .... = Priority: Internetwork Control (6)
        ...0 .... .... .... = DEI: Ineligible
        .... 0000 0110 0100 = ID: 100
        Type: IPv4 (0x0800)
      Internet Protocol Version 4, Src: 10.68.0.2, Dst: 10.68.211.232
        0100 .... = Version: 4
        .... 0101 = Header Length: 20 bytes (5)
        Differentiated Services Field: 0xc0 (DSCP: CS6, ECN: Not-ECT)
           1100 00.. = Differentiated Services Codepoint: Class Selector 6 (48)
           .... ..00 = Explicit Congestion Notification: Not ECN-Capable Transport (0)
        Total Length: 354
        Identification: 0xb5c6 (46534)
        000. .... = Flags: 0x0
           0... .... = Reserved bit: Not set
           .0.. .... = Don't fragment: Not set
           ..0. .... = More fragments: Not set
        ...0 0000 0000 0000 = Fragment Offset: 0
        Time to Live: 128
        Protocol: UDP (17)
        Header Checksum: 0x9a92 [validation disabled]
        [Header checksum status: Unverified]
        Source Address: 10.68.0.2
        Destination Address: 10.68.211.232
      User Datagram Protocol, Src Port: 67, Dst Port: 68
        Source Port: 67
        Destination Port: 68
        Length: 334
        Checksum: 0x6d2d [unverified]
        [Checksum Status: Unverified]
        [Stream index: 5]
        [Timestamps]
           [Time since first frame: 0.030404000 seconds]
           [Time since previous frame: 0.030404000 seconds]
        UDP payload (326 bytes)
    Dynamic Host Configuration Protocol (ACK)
        Message type: Boot Reply (2)
        Hardware type: Ethernet (0x01)
        Hardware address length: 6
        Hops: 0
        Transaction ID: 0xf4012537
        Seconds elapsed: 0
        Bootp flags: 0x0000 (Unicast)
           0... .... .... .... = Broadcast flag: Unicast
           .000 0000 0000 0000 = Reserved flags: 0x0000
        Client IP address: 0.0.0.0
        Your (client) IP address: 10.68.211.232
        Next server IP address: 0.0.0.0
        Relay agent IP address: 0.0.0.0
        Client MAC address: ZyxelCommuni_74:ac:d4 (d4:1a:d1:74:ac:d4)
        Client hardware address padding: 00000000000000000000
        Server host name not given
        Boot file name not given
        Magic cookie: DHCP
        Option: (53) DHCP Message Type (ACK)
           Length: 1
           DHCP: ACK (5)
        Option: (54) DHCP Server Identifier (10.68.0.2)
           Length: 4
           DHCP Server Identifier: 10.68.0.2
        Option: (51) IP Address Lease Time
           Length: 4
           IP Address Lease Time: 1 hour (3600)
        Option: (1) Subnet Mask (255.255.0.0)
           Length: 4
           Subnet Mask: 255.255.0.0
        Option: (3) Router
           Length: 4
           Router: 10.68.0.1
        Option: (6) Domain Name Server
           Length: 8
           Domain Name Server: 62.58.48.20
           Domain Name Server: 37.143.84.228
        Option: (15) Domain Name
           Length: 20
           Domain Name: ftth.glasoperator.nl
        Option: (43) Vendor-Specific Information
           Length: 24
           Value: 012e687474703a2f2f31302e31322e302e31303a37353437
        Option: (255) End
           Option End: 255
