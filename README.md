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

1 - TCP (Transmission Control Protocol): This ensure that the complete data will reach to its destination in correct order and without any error. 

How TCP works:-
  - Establish a Connection:- 
    Before data transmitted, a connection must be established between client and server. Connection is being established with 3-way handshake process.

  - Data Transfer:-
    After established connection, data can be transmitted between client and server. Data is broken into smaller parts called segments, the receiver acknowledege each segment received. If any segemnt lost or damaged, the sender retransmit it again.

  - Connection Termination:-
    Once data is transmitted, connection can be terminated using the TCP Four-way handshake process.

2 - UDP (User Datagram Protocal): This protocol is a connection-less protocol which sends the data to receiver but does not guarentee the complete transmission of data packets to receiver. It is used for application where speed and efficiency are priotized over reliability such as Video Calling, Online Gaming Live Streaming, Voice Over IP (VoIP). Suppose you are on a video call with someone then sometime video stuck or freezes, it means your data packets get lost did not reach to you that's why you got the freeze in the video calling.

How UDP Works:-
    - Imagine a real time video streaming application using UDP.
    - The video stream is broken down into UDP packets, each packet is containing the portion of video data. These packets are sent over the network to the receiving device, which decodes and displays the video in real time.
    - If few packets are lost or arrive out of order, the video may experience glitched, frezze but the application continues to play without waiting for retransmission.


3 - HTTP/HTTPS

4 - SMTP

5 - FTP

6 - DNS

7 - DHCP


**IP Address**
