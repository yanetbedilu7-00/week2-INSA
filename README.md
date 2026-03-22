NETWORKING
📘 1. What is Networking?
Networking is the connection of two or more computers/devices to share data, resources, and communication.
🔹 Examples
Sharing files between computers
Internet access
Email and messaging
📘 2. Types of Networks
Type
Meaning
Example
LAN
Local Area Network
School, home
WAN
Wide Area Network
Internet
MAN
Metropolitan Area Network
City network
📘 3. Network Devices
Router → connects networks (internet access)
Switch → connects devices in LAN
Modem → connects to ISP
Access Point → provides Wi-Fi
📘 4. IP Address (Internet Protocol)
An IP address is a unique number given to each device on a network.
🔹 Format
IPv4 = x.x.x.x
Example: 192.168.1.1
Each part (octet) = 0–255
📘 5. Structure of IPv4
Total = 32 bits
Divided into 4 octets
Example:
192 . 168 . 1 . 10
​
📘 6. IP Address Classes
Class
Range
Default Mask
Structure
A
1–126
255.0.0.0
N.H.H.H
B
128–191
255.255.0.0
N.N.H.H
C
192–223
255.255.255.0
N.N.N.H
D
224–239
—
Multicast
E
240–254
—
Experimental
📘 7. Network vs Host
Class
Network Part
Host Part
A
1 octet
3 octets
B
2 octets
2 octets
C
3 octets
1 octet
🔹 Example
IP: 192.168.1.10
Network = 192.168.1
Host = 10
📘 8. Special / Reserved IP Addresses ⭐​
These are VERY IMPORTANT for exams
Address
Meaning
0.0.0.0
Unspecified / default
127.x.x.x
Loopback (your computer)
127.0.0.1
Localhost
255.255.255.255
Broadcast
224–239
Multicast (Class D)
240–254
Experimental
📘 9. Important Rules
✅ Each octet = 0–255
❗ But not all values are usable
Host = 0 → network address
Host = 255 → broadcast
127 → loopback (cannot use)
📘 10. Class D (Multicast)
Range: 224–239
No network/host split
Used to send data to many devices at once
Example: video streaming
📘 11. Key Points to Remember
128 → Class B starts
192 → Class C starts
224 → Class D starts
127 → reserved (loopback)
🧠 Practice Exercises
✏️ 1. Identify the class
a) 10.1.1.1
b) 128.5.6.7
c) 192.168.0.1
d) 225.1.1.1
✏️ 2. Network & Host
a) 172.16.5.10
b) 192.168.1.25
✏️ 3. Special or Not?
a) 127.0.0.1
b) 255.255.255.255
c) 0.0.0.0
✏️ 4. True/False
a) Class D has hosts
b) 223 is Class C
c) 128 is Class A
✅ Answers
1.
a) Class A
b) Class B
c) Class C
d) Class D
2.
a) Network = 172.16, Host = 5.10
b) Network = 192.168.1, Host = 25
3.
a) Loopback
b) Broadcast
c) Unspecified
4.
a) False
b) True
c) False
🔥 Final Summary (Quick Memory)
A: 1–126
B: 128–191
C: 192–223
D: 224–239
E: 240–254
127: loopback
0: default
255: broadcast
ipv4 4 billion
ipv6 3.4 un decillion
OSI  layers
1. Application Layer (Layer 7) — “You tell the browser what you want”
You type the URL in your browser.
Browser creates an HTTP request asking for the webpage.
Think of it like writing a letter: “Dear server, please send me this page.”
2. Presentation Layer (Layer 6) — “Prepare your letter”
The browser formats the request so the server can understand it.
If it were HTTPS, it would also encrypt it.
Think of it as putting your letter in the right envelope.
3. Session Layer (Layer 5) — “Keep the conversation open”
The browser and server establish a connection.
Makes sure your request can be sent and replied to properly.
Think of it like making a phone call instead of just sending a letter and hoping the server answers.
4. Transport Layer (Layer 4) — “Ensure it arrives safely”
Breaks your HTTP request into smaller TCP pieces.
Adds port numbers so the server knows which app to send it to (port 80 for HTTP).
Ensures all pieces arrive complete and in order.
Like sending a multi-page letter in an envelope, and the post office guarantees it won’t lose any pages.
5. Network Layer (Layer 3) — “Find the route”
Adds IP addresses (your device → server).
Decides the best path through the Internet.
Like a GPS for your letter, finding the quickest route to the server.
6. Data Link Layer (Layer 2) — “Deliver locally”
Prepares data for your local network (home Wi-Fi, office LAN).
Adds MAC addresses (like street addresses inside the city).
Ensures it reaches your router, then the ISP.
7. Physical Layer (Layer 1) — “Send the bits”
Converts everything into electric signals, light pulses, or Wi-Fi signals.
Travels through cables, fiber, or airwaves to reach the next device.
Like your postal truck physically carrying the letter.
🔁 How It Returns to You
Server receives the request → prepares HTTP response (web page)
Data travels back through all 7 layers in reverse: Physical → Data Link → Network → Transport → Session → Presentation → Application
Browser reassembles everything → displays the page on your screen
🖼 Easy Analogy (The “Letter + GPS” Version)
OSI Layer
What it does
Analogy
7 Application
Creates HTTP request
Writing a letter
6 Presentation
Formats/encrypts
Putting letter in envelope
5 Session
Keeps connection alive
Making a phone call
4 Transport
Ensures delivery
Sending multi-page letter safely
3 Network
Routes packets
GPS for letter
2 Data Link
Local delivery
Street addresses within city
1 Physical
Transmits signals
Postal truck or airplane
✅ Key idea: Every layer has a specific job, but they all work together to get your web page from the server to your browser.
IP address → “Which network / city should this packet go to?”
MAC address → “Which exact device / house inside that network should get it?”
