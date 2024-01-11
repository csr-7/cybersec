##Question: What can you tell us about this capture taken between two routers?

* downloaded the pcap file
* opened with wireshark
* since mentioned routing info bgp protocol stood out
* filtered by bgp protocol and found answers to questions
    * Protocol being used: BGP
    * Identifier of node startign connection: 192.0.0.1 (found under the Border Gateway Protocol - Open Message section of the packet info)
    * IP of the node starting the connection: 172.168.0.2 (can see in source section of capture)
    * IP of the node being connected to: 172.168.0.1 (can see in destination section of capture)
    * How many KEEPALIVE messages made: 26 (found one message and filtered by that type under the Border Gateway Protocol - KEEPALIVE Message section)
    * Network in CIDR that is advertised: 172.168.0.0/24 (find a UPDATE Message and network found in hthe Network Layer Reachability Information under the Border Gateway Protocol - UPDATE Mesage section)

