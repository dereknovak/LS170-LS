## 1. **What is a network?**
- two or more host or devices

## 2. **What is the Internet?**

- connection between multiple networks connected thru switches/hubs/routers
- physical infistructure and the protocols

## 3. **Is the Internet the same thing as a network?**

## 4. **What is WEB (world wide web)**
- A service that is offered via the internet
- The content or services you access using the internet

## 5. **What is the difference between network, Internet, ## and WEB?**
## 6. **What are LAN and WLAN?**
- local area network (multiple devices connect in a close location)
- wireless version (WLAN)
- LAN would be faster
## 7. **What is a protocol?**
- System of rules that dictate how devices communicate
- IP
- Ethernet protocol at each layer
- TCP/UDP
## 8. **What is the role of protocols?** 
## 9. **Why there are many different types of protocols?**
## 10. **What does it mean that a protocol is stateless?**

- AJAX, Sessions, Cookies, Query String Parameters
## 11. **Explain briefly what are OSI and TCP/IP models? ## What is the purpose of having models like that?**

- Different models of network communication
## 12. **What is PDU? What is its role?**
- Encapsultates data we are tying to send, along with its metadata
- Packages it up to send to the next layer
- Use payload for word for information
## 13. **What is Data Payload?** 
## 14. **What is the relationship between PDU and Data ## Payload?** 
## 15. **Explain How lower-level protocols work in general?**
- Different names for the PDU

## 16. **What is encapsulation in the context of networking?**
- PDU for the current layer becomes the data payload for the lower layer
## 17. **Why do we need encapsulation?** 
- Allows each layer to abstract away its information while the moves
- Layer below does not need to know what's going on above
## 18. **What are the characteristics of a physical network?** 
- The physical devices in conjuction
## 19. **How can we as developers deals with the ## limitations of physical network?**
## 20. **What is Latency?**
- Measure of delay
## 21. **What is** **Bandwidth?**
- Measure of capacity
- Specify that it's a set period of time
- how much you can send in (x) amount of time
## 22. **What are** **Network 'Hops'?**
- Each time a transmission changes
- The number of hops can effect the latency of a network
## 23. **What is the relationship between network 'Hops' ## and latency?** 
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
## 29. **How does the Internet works?**
- Data on servers that can be accessed by clients
- Servers processes request and sends back a response to the client

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
## 61. **Compare UDP and TCP. What are similarities, what are differences? What are pros and cons of using each one?** 
## 62. **What does it mean that network reliability is ## engineered?**
## 63. **Give an overview of the Application Layer.** 
## 64. **What is HTML?**
## 65. **What is a URL and what components does it have?**
## 66. **What is a Query string? What it is used for?**
## 67. **What URL encoding is and when it might be used for?**
## 68. **Which characters have to be encoded in the URL? ## Why?**
## 69. **What is www in the URL?** 
## 70. **What is URI?**
## 71. **What is the difference between scheme and protocol ## in URL?**
## 72. **What is HTTP?**
## 73. **What is the role of HTTP?**
## 74. **Explain the client-server model of web ## interactions, and the role of HTTP as a protocol within ## that model**
## 75. **What are HTTP requests and responses? What are the ## components of each?**
## 76. **Describe the HTTP request/response cycle.**
## 77. **What is a state in the context of the 'web'?**
## 78. **What is statelessness?**
## 79. **What is a stateful Web Application?**
## 80. **How can we mimic a stateful application?**
## 81. **What is the difference between stateful and ## stateless applications?**
## 82. **What does it mean that HTTP is a 'stateless ## protocol?** 
## 83. **Why HTTP makes it difficult to build a stateful ## application?**
## 84. **How the idea that HTTP is a stateless protocol ## makes the web difficult to secure?** 
## 85. **What is a `GET` request and how does it work?** 
## 86. **How is `GET` request initiated?**
## 87. **What is the HTTP response body and what do we use ## it for?**
## 88. **What are the obligatory components of HTTP ## requests?** 
## 89. **What are the obligatory components of HTTP ## response?**
## 90. **Which HTTP method would you use to send sensitive ## information to a server? Why?**
## 91. **Compare `GET` and `POST` methods.**
## 92. **Describe how would you send a `GET` request to a ## server and what would happen at each stage.**
## 93. **Describe how would you send `POST` requests to a ## server and what is happening at each stage.**
## 94. **What is a status code? What are some of the status ## codes types? What is the purpose of status codes?** 
## 95. **Imagine you are using an HTTP tool and you ## received a status code `302`. What does this status code ## mean and what happens if you receive a status code like ## that?** 
## 96. **How do modern web applications 'remember' state ## for each client?**
## 97. **What role does AJAX play in displaying dynamic ## content in web applications?**
## 98. **Describe some of the security threats and what can ## be done to minimize them?**
## 99. **What is the Same Origin Policy? How it is used to ## mitigate certain security threats?**  
## 100. **What determines whether a request should use ## `GET` or `POST` as its HTTP method?**
## 101. **What is the relationship between a scheme and a ## protocol in the context of a URL?**
## 102. **In what ways can we pass information to the ## application server via the URL?**
## 103. **How insecure HTTP message transfer looks like?**
## 104. **What services does HTTP provide and what are the ## particular problems each of them aims to address?**
## 105. **What is TLS Handshake?**
## 106. **What is symmetric key encryption? What is it used ## for?**
## 107. **What is asymmetric key encryption? What is it ## used for?**
## 108. **Describe SSL/TLS encryption process.**
## 109. **Describe the pros and cons of TLS Handshake**
## 110. **Why do we need digital TLS/SSL certificates?** 
## 111. **What is it CA hierarchy and what is its role in ## providing secure message transfer?**
## 112. **What is Cipher Suites and what do we need it for?**
## 113. **How does TLS add a security layer to HTTP?**
## 114. **Compare HTTP and HTTPS.**
## 115. **Does HTTPS use other protocols?** 
## 116. **How do you know a website uses HTTPS?**
## 117. **Give examples of some protocols that would be ## used when a user interacts with a banking website. What ## would be the role of those protocols?** 
## 118. **What is server-side infrastructure? What are its ## basic components?**
## 119. **What is a server? What is its role?** 
## 120. **What are optimizations that developers can do in ## order to improve performance and minimize latency?**