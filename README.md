# Computer-Networking

**What is Computer Networks?**

Computer Network is the collection of devices that are connected to each other which share or information data between them.



**What is Internet?**

Internet is the collection of computer networks.



**How is the Computer Network and Internet started?**

In 1960-70, During the cold war era in the United States. The US Department of Defence (DoD) wanted scientists to share the information easily and efficiently. Then, US Department of Defence created a research agency ARPA (Adevanced Research Projects Agency). ARPA created a project called ARPANET.
  **The aim of this agency was to build a communication network that could work even if any part of network destroyed. (Important during the war).**

Before ARPA, computer networks were like a single phone lines, If one line broke then whole conversation stopped.
ARPANET introduced a revolutionary concept called **Packet Switching**. Suppose you are sending a letter, packet switching breaks down the letter into smaller pieces like sentences. These smaller packets of information can travel independently over different routes. If one route gets blocked or delayed, no prolem!. The packets can take another route to reach their destination. This was the new way of communication between computers.
The first ARPANET connection was made between UCLA and Standford institute in 1969. Then technology eveolved and spread across other regions.

**Client-Server Architecture**

Client - Server architecture is the way of communication between the two devices in which a client (user device) sends a request to a server (remote device).

**Protocols**

Protocols are the rules defined by the Internet Society which ensure how data should transfer between the devices.
It ensures that data packets must completely sent to receiver, Inform during the failure and success.

Basic Protocols:-
1 - TCP (Transmission Control Protocol): This ensure that the data will reach to its destination in correct order and without any error. 

How TCP works:-
  - Establish a Connection:- 
    Before data transmitted, a connection must be established between client and server. Connection is being established with 3-way handshake process.

  - Data Transfer:-
    After established connection, data can be transmitted between client and server. Data is broken into smaller parts called segments, the receiver acknowledege each segment received. If any segemnt lost or damaged, the sender retransmit it again.

  - Connection Termination:-
    Once data is transmitted, connection can be terminated using the TCP Four-way handshake process.

2 - UDP ()
