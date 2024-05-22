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

1 - _Application layer_:- This layer helps to establish connections with server using the protocols. When a user interects to any software this layer ensure the data generated by the user is good for transmission.

e.g. When you use your web browser to access a website, the application layer handles the communication between the browser and the web server.


2 - _Presentation Layer_:- This layer convert the data from human-readable format to machine-readable format. It handles data encryption, compression, formatting.

e.g. When you access a secure website (HTTPS), the presentation layer encrypts your data to ensure privacy and security during transmission.


3 - _Session Layer_:- This layer establish, manages, terminates the communication session between the two devices.

e.g. When you have a video call, the session layer establishes and maintains the session between your device and the remote device until the call ends.


4 - _Transport Layer_:- This layer divides the large amount of data into smaller packets then send it to netwrok layer.

e.g. When you stream a video, the transport layer ensures that the video data packets arrive in the correct order and are reassembled properly.


5 - _Network Layer_:- This layer add the source and destination IP address to each data packet.

e.g. When you access a website, your router determines the best path for the data packets to travel across the internet to reach the web server.


6 - _Data-Link Layer_:- This layer check the error in each packet. This layer packages the data into manageable chunks and adds error-checking information. It's responsible for ensuring the data gets delivered to the correct device on the same network segment.

e.g. When data is transferred from your computer to a switch in your office network, the data link layer handles the addressing and ensures error-free delivery.

7 - _Physical Layer_:- It is responsile for physical transmission of data over wired cable or wireless signal. It finds the best path to send the data packet.

e.g. When you plug an Ethernet cable into your computer and connect it to a router, you're working with the physical layer.


### TCP/IP Model

TCP/IP model is simplified and practical model for understanding how data is transmitted from one device to other device over the internet. It was designed by Department of Defence (DoD) in 1960.

**What does TCP/IP do?**

The main work of this model is to transfer the data from one device to another device. The main condition of this process is to make data reliable and accurate so that receiver will receive the same information which is send by the sender.

**How does TCP/IP work?**

Whenever we want to send something over internet using TCP/IP model, the TCP/IP mdeol divides the data into packets at sender's end and the same pckets have to be recombined at the receiver's end from the same data.

5 Layers of TCP/IP model:-

1 - _Application Layer_:- Application Layer is which the user interacts. It provides network services directly to end-user applications.

2 - _Transport Layer_:- Transport layer divides the data into packets and ensures data gets delivered accuratly and in correct order between the devices.

3 - _Network Layer_:- Network layer add the source and destination ip address to each data packet and responsible for routing data packets from one device to another.

4 - _Data-Link Layer_:- This layer check the error in each packet. This layer packages the data into manageable chunks and adds error-checking information.

5 - _Physical Layer_:- It is responsile for physical transmission of data over wired cable or wireless signal. It finds the best path to send the data packet.


### PORT

A PORT is a virtual number which is assigned to an application or service running on a device which defines on which application to send the data. A device can run many applications or services at a time, e.g. You are searching something on a browser, checking email (using Outlook), listening to music (using music streaming application) at the same time. So here port comes in the picture, PORT will decide which application to send the data.

IP Address- It uniquely idendified the device on network.

PORT- Directing the data to the particular appliction or service on the device which is uniquely identified on a network.

**Ephemeral PORT**

Ephemeral port is the temporary number assigned to that service or application which is already running on the same port.

e.g. You are visiting a website in chrome, here your port 80 is already busy because the website you are visitin is using the PORT 80. If you open one more tab and visit to another websitethen ephemeral port comes here in picture. Your browser will assign a temporary port number to the other tabs you will open after the first tab. An that ephemeral port will last untill your session ends or you close the tab.


### HTTP

HTTP (Hypertext Transfer Protocol) is a set of rule which define how the data (web pages, images, videos) transmitted to the server and receive from the server over the internet.

It works on a Client-Server model where a client (your machine) sends the HTTP request to the server and A server sends the HTTP response to the client. Here works the HTTP protocol.

HTTP uses TCP protocol to send or receive the data.

It is a Stateless protocol it means when a user sends a HTTP request to the server then the server does not store any information about the user machine by default.

**HTTP Methods**

HTTP methods tells the server what to do when a client makes a http request to the server, like Get the data, Post the data, Put the data, Delete the data.

**HTTP Error/Status Codes**

Error or Status code represents the result of the http request. When you want to know the status of your sent request to the server it is known by these codes.

1XX - Informational (e.g., 100: Continue).

2XX - Success (e.g., 200: OK, 201: Created).

3XX - Redirection (e.g., 301: Moved Permanently, 302: Found).

4XX - Client Errors (e.g., 404: Not Found, 403: Forbidden).

5XX - Server Errors (e.g., 500: Internal Server Error, 503: Service Unavailable).

### Cookies

Cookie is a small piece of data stored on a user's computer in the form of file by a web browser while visiting a website.

e.g. When you visit a website for the first time that website will set (save) a cookie in your device, after that when you visit that same website again in the request header the cookie will be sent to the server by your browser then server will know ohh this request is coming from Puneet then the server will check in its database and find a last visit session for it.

Server will know like who is contacting

Real Life Examples:-

1 - Imagine you are shopping online on amazon, As you browse different items and add them to your cart, a cookie is created is created to rember the items in your cart. If you leave the site and come back later, the website can retrieve the cookie and your will still have the items you selected earlier.

2 - When you login websites like Instagram or Gmail, acookie is created to remember your login session. When you open the same website again you don't need to login again directly redirecte to the homepage.


### SMTP

SMTP (Simple Mail Transfer Protocol) is the set rules that is used to send email from one person to another person. It tells how the email data travels from sender's device to receiver's device.

How it works?

Behind the scene your email client doesn't send the email directly. Instead, it connects to a special server called SMTP server.

There are two ways:-

1 - When a person send a mail from Gmail to Gmail:-

You write an email using an email client like Gmail. Your email client (Gmail) connects to its SMTP server and sends the mail data to its server. Now SMTP server processes the data and determine the receiver's detail. If the detail is correct then SMTP server transfer the mail to receiver's device. Finally receiver receive the mail and SMTP server send success or failure acknowledgement to sender. There is a dedicated SMTP server of each of the client like Gmail. 

2 - When a person send a mail from Gmail to Outlook.

Your write an email using an email client like Gmail. Your email client (Gmail) to its SMTP server and sends the mail data to its server. Now Gmail SMTP server connects to the receiver's SMTP server, verify the receiver's detail and sends mail data to receiver's SMTP server. Here in this case Gmail SMTP server will connect to the Outlook SMTP server. Now receiver's SMTP server attempts to deliver the email to recipeint's mail box. If there is an issue receiver's SMTP server bounce back the mail to sender, noifying them the failed delivery.

e.g., Imagine you are sending a birthday email to your friend who uses Yahoo mail:-

- Your client connects to your email provider's SMTP server (like Gmail).

- The SMTP server verifies your login information.

- The SMTP server finds Yahoo Mail's SMTP server address.

- Your email is sent to Yahoo Mail's SMTP server.

- Yahoo mail's server check if the recipeint's emsil address exists and deliver it to their inbox.

- If the recipient's mailbox is full, Yahoo Mail's server sends a bounce-back message to your Gmail account.

SMTP uses port 25 for the communication. It uses TCP protocol to send or receive the data.

