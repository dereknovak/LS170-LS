## 1. **What is a network?**
- A network, in its simplest form, is formed when two devices are connected, allowing communication and data to be exchanged between them.

## 2. **What is the Internet?**
- The Internet is a network of networks, providing connections between these various networks through switches, routers, and other forms of network connection. Along with this physical infrustructure, the Internet is built on a series of protocols that allow each individual device on the network communicate successfully with other devices.

## 3. **Is the Internet the same thing as a network?**
- The Internet is a network, but a network is not necessarily the Internet. The Internet is a *network of networks*, essentially creating a network relationship between two or more other networks.

## 4. **What is WEB (world wide web)**
- The World Wide Web is a service that is offered within the Internet. While the Internet is a the physical infrustructure and protocols of the network, the Web is how we interact with it.

- A service that is offered via the internet
- The content or services you access using the internet

## 5. **What is the difference between network, Internet, and WEB?**
- A network is a communication connection between two or more devices, which is then expanded to form the Internet, a *network of networks*. The service used to interact with the Internet is know as the World Wide Web.

## 6. **What are LAN and WLAN?**
- A Local Area Network (LAN) is exactly as it sounds: a network formed with an area of close proximity. These are generally connected in a physical manner (copper cables, switches, etc); however, it can be expanded wirelessly to form a Wireless Local Area Network (WLAN). In general, LAN is faster and more reliable, as it relies on a physical connection. This is contrasts by the radio waves used by WLAN, which is less reliable but much more portable.

- local area network (multiple devices connect in a close location)
- wireless version (WLAN)
- LAN would be faster

## 7. **What is a protocol?**
- A *protocol* is a system of rules that two hosts follow to allow for successful data exchange or transmission. Without these agreed-upon rules, information between the hosts would become chaotic and likely misunderstood and unprotected.

- System of rules that dictate how devices communicate
- IP
- Ethernet protocol at each layer
- TCP/UDP
## 8. **What is the role of protocols?**
- Protocol establish the system of rules that two hosts follow to allow for successful data exchange or transmission. Without these agreed-upon rules, information between the hosts would become chaotic and likely misunderstood and unprotected.

## 9. **Why there are many different types of protocols?**
- Because there are so many devices with different applications to the overall network infrustructure, different kinds of protocols are made to allow the devices to communicate in their most suitable way. Otherwise, the task of a protocol would become too complex and data exchange would be incredibly fragile.

## 10. **What does it mean that a protocol is stateless?**
- A protocol is *stateless* when it does not persist any information between exchanges, causing each new transfer of data to act independently of another. While seemingly inefficient, this structure allows for a flexible network to exist to which developers can build with the necessary speed and security that is intended.

## 11. **Explain briefly what are OSI and TCP/IP models? What is the purpose of having models like that?**
- Both the OSI and TCP/IP models represent the general process to which data is exchanged between networks. Broadly speaking, a client will request data from a server. This request will identify and package the necessary port number and IP address, using the MAC address from each intermediate hop to relay the request to the server. Once arrived, the original request will find its way to the server, which will issue a response in a reverse route.
- Having models such as these allows developers to understand how this information is exchanged so that the necessary implementation of the systems and security will work with the existing network.

## 12. **What is PDU? What is its role?**
- A protocol data unit (**PDU**) represents a block of data that is transferred across a network, with each PDU receiving a different name depending on its placement within the OSI or TCP/IP model. As data moves across the network, the The entire PDU for a specific layer of the OSI model--header, data payload, trailer--is encapsulated as the data payload for the layer below it. This allows each layer to operate independently, disregarding any information from other layers and providing a 'service' to the upward layer.

- Encapsultates data we are tying to send, along with its metadata
- Packages it up to send to the next layer
- Use payload for word for information

## 13. **What is Data Payload?**
- A data payload represents a chunk of data that is being sent from one host to another, complimented with a header to provide metadata. Each PDU within the OSI and TCP/IP models are encapsulated into the data payload for the lay below it, allowing each layer to operate independently and deliver each layer's respective data payload to the appropriate host.

## 14. **What is the relationship between PDU and Data Payload?** 
- The PDU from the layer above within the OSI and TCP/IP models are encapsulated into its data payload, allowing each layer of the models to operate independently from one another.

## 15. **Explain How lower-level protocols work in general?**
- Different names for the PDU

## 16. **What is encapsulation in the context of networking?**
- The entire PDU for a specific layer of the OSI model--header, data payload, trailer--is encapsulated as the data payload for the layer below it. For example, the TCP segment of a data exchange is encapsulated within the data payload of the IP packet, which is then encapsulated as the data payload of the ethernet frame. This allows each layer to operate independently, disregarding any information from other layers and providing a 'service' to the upward layer.

## 17. **Why do we need encapsulation?**
- Encapsulating the PDU from the layer above into the data payload of the present PDU allows each layer to abstact away its information while the data package moves from one host to another. These layers can function independently from one another, focusing on their given task. For example, the TCP segment is only concerned with making its way to the appropriate application using the destination port number within its PDU, while the IP packet from the layer below is concerned with simply *getting to* the device by way of an IP address.

- Allows each layer to abstract away its information while the moves
- Layer below does not need to know what's going on above

## 18. **What are the characteristics of a physical network?** 
- The physical network is made up of all the working devices connected together to allow for network communication. These include the devices themselves, the switches and routers to relay information to the appropriate parties, and the cables, fiber optics, and radio waves traversed.

- The physical devices in conjuction

## 19. **How can we as developers deals with the limitations of physical network?**
- Developers can deal with these limitations by implementing checks within the virtual network to ensure all data is transferring successfully. TCP segments, for example, employ an array of different reliability checks (in-order delivery, de-duplication, message acknowledgements and retransmission) that allow lost data along these paths to be resubmitted and reorganized if out of order. To span long distances, developers may also implement repeaters to resend data while along the path, preventing packets from dropping.

## 20. **What is Latency?**
- **Latency** is the measure of time that it takes for data to move from one part of a network to another.

- Actual time to process
- Actual time to put on stack
- Time in que
- Propogation delay

## 21. **What is** **Bandwidth?**
- **Bandwidth** refers to the total data that can be transferred from one device to another within a specific timeframe.

## 22. **What are** **Network 'Hops'?**
- A **hop** is the movement from one device to another. Each IP package keeps track of its hop count, preventing bugs in the path from halting a delivery using the hop limit.

## 23. **What is the relationship between network 'Hops' and latency?**
- In general, the more hops required of a network transmission, the more delayed the latency will be.

## 24. **What is a switch and what is it used for?**
- Used in LAN
## 25. **What is a hub and what is it used for?**
- Used in LAN
## 26. **What is a modem and what it is used for?**
- Used in WLAN
- Also called a gateway (check)
- Gateway into the wider internet that helps you get the infirstructure to the ISP
## 27. **What is a router and what is it used for?**
- Used in the larger internet 
## 28. **What is the difference between a switch, hub, ## modem, and router?**
## 29. **How does the Internet work?**
- The internet is a network of networks, connecting millions of hosts from across the globe. Hosts are represented by either a client (making a request) or a server (responding to a request). With each request, data is packed into a series of PDUs and encapsulated within the data payload of the PDU beneath it and is sent through an array of switches, routers, and other devices until arriving at the server to which the client is requesting data. After decapsulation of the data and processing of the request, the server then sends back a response to the client in a similar but reversed route as the client.
- Broadly speaking, each interaction with a resource prompts this request and response cycle, resulting in tens of billions of cycles occuring across the world per second.

## 30. **What is a MAC address and what is its role in ## network communication?** 
- Part of the Ethernet frames
- Provide 
## 31. **Give an overview of the Link/Data Layer**
## 32. **What is included in an Ethernet frame?**
## 33. **Give an overview of the Internet/Network Layer and it's role.**
## 34. **What is IP?**
- Way of identifying devices on the network
- Structured in a logical way rather than a flat heiarchy

## 35. **What is IP address?** 
- IPv4 - 32 bits in length
- IPv6 
## 36. **What are the components of IP addresses?**
- 32 bits, range from 0-255 
## 37. **What is a packet in computer networking?**
## 38. **Why do we need both MAC addresses and IP addresses?** 
## 39. **What is DNS and how does it work?**
- Pairs up the more readable name to the IP address
## 40. **How do port numbers and IP addresses work together?**
## 41. **What is a checksum and what is it used for? How is ## it used?**
## 42. **Give an overview of the Transport Layer.** 
## 43. **What are the fundamental elements of reliable protocol?**
- Having the data arrive in tact
- Arrive in order
- Mesasge acknowledgement
- Retransmission of lost packets
## 44. **What is pipe-lining protocols? What are the ## benefits of it?**
## 45. **What is a network port?**
## 46. **What is a port number?**
## 47. **What is a network socket?**
## 48. **Is TCP connectionless? Why?**
- Three-way handshake

## 49. **How do sockets on the implementation level relate ## to the idea of protocols being connectionless or ## connection-oriented?** 
## 50. **What are sockets on implementation and on a ## theoretical level?** 
## 51. **What does it mean that the protocol is ## connection-oriented?**
## 52. **What is a three-way handshake? What is it used for?**
- Syn => Syn-Ack => 
## 53. **What are the advantages and disadvantages of a ## Three-way handshake?** 
## 54. **What are multiplexing and demultiplexing?**
## 55. **How does TCP facilitate efficient data transfer?**
## 56. **What is flow control? How does it work and why do ## we need it?**
## 57. **How TCP prevents from receiver's buffer to get ## overloaded with data?**
## 58. **What is congestion avoidance?**
- Strategy used to reduce latency
- If a router is overloaded, it will store data in a buffer
- Only so much room, excess will be dropped
- 
## 59. **What is network congestion?**
- Know the difference between network congestion and congestion avoidance

## 60. **How do transport layer protocols enable communication between processes?**
- The transport layer protocols enable communication by holding information about the source and destination **port numbers** within its header. These identifiers are used to locate a specific application within a device, and are typically appended on the device's IP address in the form of a *socket*.

## 61. **Compare UDP and TCP. What are similarities, what are differences? What are pros and cons of using each one?**
- The Transport Layer Protocol (TCP) and User Datagram Protocol (UDP) are protocols that are used in the Trasport Layer of the OSI model. They exist as a means to trasport either TCP segments or UDP datagrams between two applications. TCP is a connection-oriented protocol and is focused primarily on reliablility, implementing in-order delivery, de-duplication, and message acknowledgements and retransmission to ensure that all data arrives in tact. While reliable, this also slows down the TCP transaction.
- UDP, on the otherhand, is a connectionless protocol. This means that a connection does not need to be established before commencing communication, nor do any of the previously mentioned checks take place. While less reliable, a UDP datagram makes up for it in speed and flexibility, as it does not have to worry about the extra checks. Although UDP does not come stock with any of the reliability perks, many developers will add extra functionality to the protocol to make it more reliable.

## 62. **What does it mean that network reliability is engineered?**
- Networks are inherently unreliable, meaning that data can be sent across a network and there is no guarantee that the information will not be lost. Obviously, this would not bode well for communication, so reliability is engineered into the process to ensure all data is transferred successfully. Many examples of reliability engineering exist in TCP, which adds in-order delivery (packets are sorted in appropriate order), de-duplication (repeated packets are deleted), and message acknowledgements and retransmission (dropped packets are resent).

## 63. **Give an overview of the Application Layer.** 
- The Application layer's job in regards to the OSI model is allow applications to share information at a syntactical level. Certain applications, such as e-mail clients or web browser, require different kinds of communcation, which is where the Application layer protocols come to shine.

## 64. **What is HTML?**
- The Hypertext Markup Language (HTML) is a structured file that can include headings, paragraphs, lists, and most importantly links, which is where *hypertext* is derived.

- structure/organization of the page

## 65. **What is a URL and what components does it have?**
- A URL is a type of URI that includes *both* the name and protocol. While its technically correct to call a string of characters with both present a URI, it's *more correct* to refer to it as a URL, as its a more specific distinction.
- A URL must consist of a scheme and a host. They can also include a port number (no port number uses a default), a path, a query string, and a fragment.

## 66. **What is a Query string? What it is used for?**
- The **query string**, which is made up of one or more *query parameters* are used to send additional data to the server upon request.

- can be used to persist state

## 67. **What URL encoding is and when it might be used for?**
- Special Character's using UTF-8


## 68. **Which characters have to be encoded in the URL? Why?**

## 69. **What is www in the URL?** 
- WWW refers to the World Wide Web, which is a service used to request information throughout the internet. This is mostly a naming convention that is used to identify a web address and serves no technical purpose.

## 70. **What is URI?**
- A URI is a string of characters that identifies a specific resourse and can include either its name, protocol, or both.

## 71. **What is the difference between scheme and protocol in URL?**
- While there is a connection between the scheme and a protocol, they are *not* the same thing; the scheme simply indicates which protocol is being used.

## 72. **What is HTTP?**
- HTTP is a text-based request response protocol that allows the transfer of hypertext documents between two web applications. This is accomplished through requests, which can retrieve, add, or change various documents by means of HTTP methods, and the subsequent response, which provides information about the documents and status code of the request.

- HTTP is in plain text

## 73. **What is the role of HTTP?**
- HTTP is a protocol established at the Application layer of a Networking model. It's a text-based request response protocol that allows the transfer of hypertext documents between two web applications.

## 74. **Explain the client-server model of web interactions, and the role of HTTP as a protocol within that model**
- When an application (client) makes a request to another application (server), an exchange of data is made. This is accomplished through requests, which can retrieve, add, or change various documents by means of HTTP methods, and the subsequent resposne, which provides information about the documents and status code of the request.

## 75. **What are HTTP requests and responses? What are the components of each?**
- Any time that you enter a URL or click on a resource, your web browser (client) is making a request to its respective server. Each request will contain a header that indicates the name of the server, acceptable languages that can be used, the client's ID, the type of connection preferred, and more. Upon each request, a response is provided by the server. Similarly, a header is used to provide information, including the type of data encoding, the name of the server, the location of the resource, the type of data, and more. Each request will also include the type of request method used (GET, POST) and the response will return a status code to indicate the status of the request.

## 76. **Describe the HTTP request/response cycle.**

## 77. **What is a state in the context of the 'web'?**
- A state refers to saved information that allows for dynamic accessibility to the web. However, HTTP is a *stateless* protocol in that it does not save state in any part of its implementation, causing each request and response by applications to act independently from any other. For this reason, developers must engineer methods to create a *stateful* environment through the use of sessions, cookies, and AJAX.

## 78. **What is statelessness?**
- HTTP is a *stateless* protocol in that it does not persist state in any part of its implementation, causing each request and response by applications to act independently from any other. This provides resilience to the HTTP protocol, as no maintenance is required throughout usage; however, lack of state creates a challenging experience for building stateful applications as programmers must find alternative methods of storing information.

## 79. **What is a stateful Web Application?**
- A *stateful* Web Application refers to one that can save information between requests, allowing for a dynamic interaction with the Web Application.

## 80. **How can we mimic a stateful application?**

## 81. **What is the difference between stateful and stateless applications?**
## 82. **What does it mean that HTTP is a 'stateless protocol?** 
## 83. **Why HTTP makes it difficult to build a stateful application?**
## 84. **How the idea that HTTP is a stateless protocol makes the web difficult to secure?** 

## 85. **What is a `GET` request and how does it work?**
- A `GET` request is an HTTP method that retrieves data from a server. Any time a URL is entered, a link is followed, or a resource is clicked, a `GET` request is made that provides access to the data.

## 86. **How is `GET` request initiated?**
## 87. **What is the HTTP response body and what do we use it for?**
- The HTTP response body is the raw data from the resource requested. While this data respresents the encoding of the resource in either HTML, JSON, etc, applications within web browsers interpret the code and display it in a more readable fashion.

## 88. **What are the obligatory components of HTTP requests?**
- An HTTP request must always contain a method (`GET`/`POST`) as well as the path.

## 89. **What are the obligatory components of HTTP response?**
- An HTTP response will always include a status code, but everything else is optional.

## 90. **Which HTTP method would you use to send sensitive information to a server? Why?**
- The `POST` HTTP method should be used when sending sensitive information to a server. This is because, in a `GET` method request, all sensitive data is displayed within the URL query string and is therefore easily accessible to a hijacker. Instead, with `POST` method requests, this data is included within the optional HTTP body.

## 91. **Compare `GET` and `POST` methods.**
## 92. **Describe how would you send a `GET` request to a server and what would happen at each stage.**
## 93. **Describe how would you send `POST` requests to a server and what is happening at each stage.**
## 94. **What is a status code? What are some of the status codes types? What is the purpose of status codes?**
- The **status code** is a three-digit number included in the HTTP response that references the status of the given request. A few common status codes include 200 (successful request), 302 (successful, but redirected), 404 (resource not found), and 500 (server error). These status codes exist to provide status information to the client on their given request.

## 95. **Imagine you are using an HTTP tool and you received a status code `302`. What does this status code mean and what happens if you receive a status code like that?**
- The 302 status code represents a successful request, however a redirect was required. This means that the resource request exists, but at a different location than at the inputted request.

## 96. **How do modern web applications 'remember' state for each client?**
- Web applications can exhibit a *stateful* environment with the implementation of **sessions**, **cookies**, and Asynchronous JavaScript and XML (**AJAX**).

- combination of some
- 
## 97. **What role does AJAX play in displaying dynamic content in web applications?**
- AJAX is used to request data and process its response without reloading the current web page. By eliminating this full page refresh, the client's experience with the web application's content becomes faster and more fluid.

- Polling/Long-polling

## 98. **Describe some of the security threats and what can be done to minimize them?**
- Due to the stateless nature of HTTP, there are a few security threats that have become commonplace and must be addressed. Anyone can intercept a request, which may house sensitive information. HTTPS implements encryption with every request, giving the ability to decrypt to only the client and server. Foreign parties may also try to post data from a unknown source, so developers can add a *same-origin policy* to prevent access to the data without a matching scheme and host. Session hijacking is another threat that can exist, which occurs when a foreign user intercepts a session ID. To combat this, developers can frequently refresh the ID, making the hijacker's useless. Lastly, a threat may post explicit code directly into a comment box that can change the resource in an unintended way. Developers are encouraged to sanitize any inputs such as this to prevent these unexpected behaviors.

## 99. **What is the Same Origin Policy? How it is used to mitigate certain security threats?**
- The **same-origin policy** restricts specific interactions between foreign resources, referring to those that originate from a different scheme or host. While more secure, this restriction can make it challenging for developers who require cross-origin requests. To combat this, Cross-origin resource sharing (**CORS**) was developed to permit these cross-origin interactions by implementing a new set of HTTP headers.

## 100. **What determines whether a request should use `GET` or `POST` as its HTTP method?**
## 101. **What is the relationship between a scheme and a protocol in the context of a URL?**
## 102. **In what ways can we pass information to the application server via the URL?**
## 103. **How insecure HTTP message transfer looks like?**
## 104. **What services does HTTP provide and what are the ## particular problems each of them aims to address?**
## 105. **What is TLS Handshake?**
- The TLS handshake is used in the HTTPS encryption process that establishes both the TLS version and cypher used in data exchange between a client and server.

## 106. **What is symmetric key encryption? What is it used for?**
- Symmetric Key Encryption provides two applications with the same decryption key, allow an exchange of encrypted data between them that only the two can decrypt.
- 
## 107. **What is asymmetric key encryption? What is it ## used for?**
- Asymmetric Key Encryption provides two application with a public decryption key and only one with a private key. The application without the private key can send an encrypted message to the other using the public key, and the other can decrpyt it using their private key. This allows for one way communication, which is typically used in setting up the shared key that both applications will use in the upcoming symmetric key encryption data exchange.
- 
## 108. **Describe SSL/TLS encryption process.**
## 109. **Describe the pros and cons of TLS Handshake**
- The TLS handshake provides a reliable exchange of a 
## 110. **Why do we need digital TLS/SSL certificates?** 
- Certificates issued to a server by a Certificate Authority are used to proved that the IP is who they say they are.

## 111. **What is it CA hierarchy and what is its role in providing secure message transfer?**
## 112. **What is Cipher Suites and what do we need it for?**
- A Cipher Suite includes all of the ciphers that a client has the ability to use. The Cipher Suite is shared with a server upon the TLS handshake, and the server will select an included cipher to use for the initial ansynchronous encryption.

## 113. **How does TLS add a security layer to HTTP?**

## 114. **Compare HTTP and HTTPS.**
- HTTP and HTTP are exactly the same except for one element: added security. With the 'S' representing 'Secure', HTTPS implements the Transport Layer Security (TLS) into each request, encrypting every message exchange between the client and server.

## 115. **Does HTTPS use other protocols?** 
- HTTPS uses the Transport Security Layer (TLS) protocol to establish and maintain a secure connection between two hosts.

## 116. **How do you know a website uses HTTPS?**
- You can see that a website uses HTTPS if the URL's scheme includes `https://`. In many browsers, you can also see a padlock next to the URL that will provide information on the host's security, which if referencing TLS or SSL, HTTPS is being used.

## 117. **Give examples of some protocols that would be used when a user interacts with a banking website. What would be the role of those protocols?** 
- A bank would most likely use HTTPS in conjunction with TLS, as this is an easy and very powerful security system to implement. TLS would encrypt all requests and responses made by the client and bank server, keeping all data confidential. In terms of a transport protocol, TCP would most likely be used over UDP, as reliablity is much more vital than speed when working with personal finances.

## 118. **What is server-side infrastructure? What are its basic components?**
## 119. **What is a server? What is its role?** 
## 120. **What are optimizations that developers can do in order to improve performance and minimize latency?**
- Limit the total number of resources that need to be fetched
- Compress data using a utility such at gzip
- Reuse a TCP connection with implementation of keep-alive
- Optimize the DNS lookup process
- Incorporate a cache to include a short-term memory bank
