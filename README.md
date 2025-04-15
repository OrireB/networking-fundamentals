# Networking Fundamentals

This repository contains project for Networking Fundamentals. It covers the OSI model, subnetting calculations, and TCP/IP protocol analysis.

## 📚 Contents

### 1. OSI Model Explanation
A breakdown of all 7 layers of the OSI model, with real-world examples of how each layer operates. 

**What is the OSI model?** 

The OSI (Open Systems Interconnection) model is a 7-layered conceptual framework used to understand how data is transmitted over a network and standardize the functions of communication systems. Below is a brief overview of each layer with real-world example
The 7 layers of the OSI model:

### 1. Physical Layer- Layer 1

**Function:** This defines the physical connection of transmitting data between devices (hardware). It defines the electrical, mechanical, and procedural aspects of communication. e.g., cables, switches, and electrical signals.

**Real-world example:** You connect your laptop to switches or routers using Cables (Ethernet cables, fiber optics). It is the physical wires and cables that connect your computer to the router or a network switch.

### 2. Data Link Layer - Layer 2

**Function:** This ensures the error-free transfer of data frames between two devices on the same network, that is, the node-to-node communication and error correction from the physical layer.

**Real-world example:** When you connect to Wi-Fi, the protocol for data transmission (like Ethernet or Wi-Fi) ensures that data is sent correctly. For example, your laptop’s Ethernet adapter establishes a connection with the router. Ethernet frames or MAC addresses used in a local network to identify devices (e.g., how a switch uses MAC addresses to forward data).

### 3. Network Layer - Layer 3

**Function:** This routes and forward data packets between devices across different networks using logical addresses (IP addresses).

**Real-world example:** When you visit a website, your computer uses the IP address to determine how to route the data (like a GPS deciding how to travel across different roads to reach the destination) e.g. IP addresses (e.g., 192.168.1.1) used to route data across the internet.

### 4. Transport Layer - Layer 4

**Function:** This provides reliable data transfer between devices using protocols like TCP (Transmission Control Protocol) and UDP (User Datagram Protocol) by managing error recovery, data flow control, and retransmission of lost data.

**Real-world example:** When you load a webpage, TCP ensures that all packets of data are received correctly and in order. Or a video streaming service using TCP to ensure smooth playback and that data arrives correctly and in the right order.

### 5. Session Layer – Layer 5

**Function:** This establishes, manages, and terminates sessions or connections between applications, ensuring they stay open or are closed properly in an organized manner. It keeps track of which data belongs to which session.

**Real-world example:** A user logging into a website and maintaining a session through a web browser ensuring the service knows you are still authenticated.

### 6. Presentation Layer - Layer 6

**Function:** This converts data into a format that the application can understand by the receiving device. It handles data encryption, compression, and translation.

**Real-world example:** A web browser rendering HTML code into a visual webpage and encrypting a password or compressing files for faster transmission or If you’re watching a video, this layer makes sure the data is in the correct format for your device to display the video. It might also encrypt the data for security.

### 7. Application Layer - Layer 7

**Function:** This is the closest to the end-user. It enables software applications to interact with the network functions like email, file transfer, and web browsing.

**Real-world example:** A user sending an email using a mail client. Web browsers (HTTP), email clients (SMTP), or file transfer protocols (FTP).


### 2. Subnetting Calculator Results
Includes subnetting for `192.168.10.0/24` into 4 subnets and attached screenshot from a subnet calculator.  
[View File](./subnetting_calculations.md)  
[See Screenshot](./screenshots/subnet_calculator_result.png)

### 3. TCP/IP Protocol Analysis
Describes how the TCP/IP protocol suite works using the example of loading a webpage.  
[View File](./tcp_ip_analysis.md)

---

## 🔧 Tools Used

- Subnetting calculator: [SubnetOnline](https://www.subnetonline.com/pages/subnet-calculators/ip-subnet-calculator.php)
- Markdown for documentation
- GitHub for version control and hosting

---

## 📥 How to Run
No executable code – simply read the markdown files for documentation.

























# Networking Fundamentals

This repository contains the following:

## OSI Model
- Explanation of the OSI model layers with real-world examples.

## Subnetting
- Calculations and results of subnetting for the given IP range.

## TCP/IP Analysis
- Short analysis of how the TCP/IP protocol suite operates across layers in a real-world scenario.
