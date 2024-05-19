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

IP (Internet Protocol) address is the unique address for a device that is used to identify a device on the internet. 

e.g. You have a router provided by your Internet Service Provider (ISP) like we have a Jio Fiber wifi. Jio has provided a router which has a global IP address. All devices connected to this router will have the same IP Address that IP address is the local IP Address given using the DHCP protocol by the router.
If any of the devices make a request to google that means that router is making a request to google because router has the global IP address. Google sends response to router then router decides which device to send that response and that is done by NAT (Network Access Translation).

Now router knows that device 1 made the google request but which application in device 1 made that request. IP address decides which device to send the data but how to decide which application to send the data to that device. That is done by the **PORT** numbers.


**OSI Model**

OSI (Open System Interconnections) model is the conceptual model to understand how data travels between different devices on internet. When a device sends the data to other device then data follows the OSI model concept to reach its destination device.

![OSI Model image](https://github.com/puneet4840/Computer-Networking/assets/65063977/db3d471b-44ef-4c62-9b25-2afef19ac866)


7 Layers of OSI Model:-

1 - Application layer:- This layer helps to establish connections with server using the protocols. When a user interects to any software this layer ensure the data generated by the user is good for transmission.

e.g. When you use your web browser to access a website, the application layer handles the communication between the browser and the web server.


2 - Presentation Layer:- This layer convert the data from human-readable format to machine-readable format. It handles data encryption, compression, formatting.

e.g. When you access a secure website (HTTPS), the presentation layer encrypts your data to ensure privacy and security during transmission.


3 - Session Layer:- This layer establish, manages, terminates the communication session between the two devices.

e.g. When you have a video call, the session layer establishes and maintains the session between your device and the remote device until the call ends.


4 - Transport Layer:- This layer divides the large amount of data into smaller packets then send it to netwrok layer.

e.g. When you stream a video, the transport layer ensures that the video data packets arrive in the correct order and are reassembled properly.


5 - Network Layer:- This layer add the source and destination IP address to each data packet.

e.g. When you access a website, your router determines the best path for the data packets to travel across the internet to reach the web server.


6 - Data-Link Layer:- This layer check the error in each layer. This layer packages the data into manageable chunks and adds error-checking information. It's responsible for ensuring the data gets delivered to the correct device on the same network segment.

e.g. When data is transferred from your computer to a switch in your office network, the data link layer handles the addressing and ensures error-free delivery.

7 - Physical Layer:- It is responsile for physical transmission of data over wired cable or wireless signal.

e.g. When you plug an Ethernet cable into your computer and connect it to a router, you're working with the physical layer.
