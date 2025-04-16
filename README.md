# Networking Fundamentals

This repository contains project for Networking Fundamentals. It covers the OSI model, subnetting calculations, and TCP/IP protocol analysis.

## Contents

### 1. OSI Model Explanation
A breakdown of all 7 layers of the OSI model, with real-world examples of how each layer operates. 

**What is the OSI model?** 

The OSI (Open Systems Interconnection) model is a 7-layered conceptual framework used to understand how data is transmitted over a network and standardize the functions of communication systems. Below is a brief overview of each layer with real-world example
The 7 layers of the OSI model:

### Physical Layer- Layer 1

- **Function:** This defines the physical connection of transmitting data between devices (hardware). It defines the electrical, mechanical, and procedural aspects of communication. e.g., cables, switches, and electrical signals.

- **Real-world example:** You connect your laptop to switches or routers using Cables (Ethernet cables, fiber optics). It is the physical wires and cables that connect your computer to the router or a network switch.

### Data Link Layer - Layer 2

- **Function:** This ensures the error-free transfer of data frames between two devices on the same network, that is, the node-to-node communication and error correction from the physical layer.

- **Real-world example:** When you connect to Wi-Fi, the protocol for data transmission (like Ethernet or Wi-Fi) ensures that data is sent correctly. For example, your laptop’s Ethernet adapter establishes a connection with the router. Ethernet frames or MAC addresses used in a local network to identify devices (e.g., how a switch uses MAC addresses to forward data).

### Network Layer - Layer 3

- **Function:** This routes and forward data packets between devices across different networks using logical addresses (IP addresses).

- **Real-world example:** When you visit a website, your computer uses the IP address to determine how to route the data (like a GPS deciding how to travel across different roads to reach the destination) e.g. IP addresses (e.g., 192.168.1.1) used to route data across the internet.

### Transport Layer - Layer 4

- **Function:** This provides reliable data transfer between devices using protocols like TCP (Transmission Control Protocol) and UDP (User Datagram Protocol) by managing error recovery, data flow control, and retransmission of lost data.

- **Real-world example:** When you load a webpage, TCP ensures that all packets of data are received correctly and in order. Or a video streaming service using TCP to ensure smooth playback and that data arrives correctly and in the right order.

### Session Layer – Layer 5

- **Function:** This establishes, manages, and terminates sessions or connections between applications, ensuring they stay open or are closed properly in an organized manner. It keeps track of which data belongs to which session.

- **Real-world example:** A user logging into a website and maintaining a session through a web browser ensuring the service knows you are still authenticated.

### Presentation Layer - Layer 6

- **Function:** This converts data into a format that the application can understand by the receiving device. It handles data encryption, compression, and translation.

- **Real-world example:** A web browser rendering HTML code into a visual webpage and encrypting a password or compressing files for faster transmission or If you’re watching a video, this layer makes sure the data is in the correct format for your device to display the video. It might also encrypt the data for security.

### Application Layer - Layer 7

- **Function:** This is the closest to the end-user. It enables software applications to interact with the network functions like email, file transfer, and web browsing.

- **Real-world example:** A user sending an email using a mail client. Web browsers (HTTP), email clients (SMTP), or file transfer protocols (FTP).

---

## 2. Subnetting Calculator Results

**Given IP Range:** 192.168.1.0/24

**Requirement:** Divide into 4 subnets

---

**The network address:** (IP address): 192.168.1.0

**The subnet mask:** 255.255.255.0 or /24

Specify the number of subnets you want to create (e.g., 4 subnets).
After entering these details, the subnetting calculator will automatically generate the following information:

**New subnet mask:** 255.255.255.192 or /26

**Number of subnets:** 4 subnets

**Subnet addresses:** The IP addresses that define each of the subnets.

**Subnet range:** The range of IP addresses available for each subnet.

Network address and Broadcast address for each subnet.


**Subnet	Network Address**

1.	192.168.1.0
2.	192.168.1.64
3.	192.168.1.128
4.	192.168.1.192

**First IP**

1. 192.168.1.1  
2. 192.168.1.65
3. 192.168.1.129	
4. 192.168.1.193

**Last IP**

1. 192.168.1.62	
2. 192.168.1.126
3. 192.168.1.190
4. 192.168.1.254 

**Broadcast Address**

1. 192.168.1.63
2. 192.168.1.127
3. 192.168.1.191
4. 192.168.1.255

**Usable IP Range**

1. 192.168.1.1 - 192.168.1.62
2. 192.168.1.65 - 192.168.1.126
3. 192.168.1.129 - 192.168.1.190
4. 192.168.1.193 - 192.168.1.254

Each subnet has its own network address (starting address), a broadcast address, and a range of usable IP addresses.

---

- **Subnetting Calculator Result:**
  ![Subnetting Calculator Result](https://github.com/OrireB/networking-fundamentals/blob/main/Subnetting%20Calculator%20Result.png?raw=true)

---

### 3. TCP/IP Protocol Analysis

**What is the TCP/IP protocol suite?** 

The TCP/IP model is the foundation for networking on the internet. It has 4 layers:

- **Application Layer (HTTP/HTTPS):**

This is where communication takes place between applications. If the server wants to get a web page from the server it sends an HTTP request. (e.g., web browsers, email clients).

- **Transport Layer (TCP):** 

This manages end-to-end communication between application (e.g., TCP, UDP).

- **Internet Layer (IP):**  

This is responsible for routing packets across networks (e.g., IP).

- **Network Access Layer (Ethernet/Wi-Fi):**  

This handles data link protocols and physical transmission (e.g., Ethernet).

**How does TCP/IP work when loading a web page?** 
**1. Application Layer:** When you enter a URL (e.g., www.example.com) in your browser, web server processes the request and sends the web page content back to your device.
 - The request is formatted according to HTTP protocol.
 - A session is established between your device and the web server.
 - 
**2. Transport Layer:** The browser sends HTTP requests to the server using TCP to establish a connection with the server (through a process called a &quot;three-way handshake&quot;).
 - The request is broken into smaller segments and assigned sequence numbers (TCP).
 - The segments are transmitted to the web server, which reassembles them in the correct order.
 - If a packet is lost or corrupted, TCP will request it to be resent.

**3. Internet Layer:** The request is encapsulated in an IP (Internet Protocol) packet and sent to the server, using routers to find the best route.
 - Each router along the path examines the IP address and forwards the request to the next hop.

**4. Network Layer:** The request is transmitted over the physical network (e.g., Ethernet or Wi-Fi) to
reach the server.
 - The data is finally transmitted over the physical medium (e.g., fiber optic cables, Wi-Fi signals) to
the destination device.

**Return Journey**
 - Server Response: The server processes the request and sends back the requested webpage (HTTP response.)
  - The content is reassembled and displayed on your device.
  - The response is reassembled and checked for errors (if using TCP).
  - Your browser receives the HTTP response and displays the webpage ) following the same path as the request.

---

**Process Flow:**
1. You type `https://example.com` into the browser.
2. DNS resolves the domain to an IP address.
3. A TCP connection (3-way handshake) is established.
4. HTTP request is sent, IP packets routed via routers.
5. Server responds with HTML/CSS/JS files.
6. Browser renders the page.

---

