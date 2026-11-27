# Observing Network Traffic on Rapsberry Pi

## Task 1 --- Install tcpdump

Run:

    sudo apt install tcpdump

### Screenshot

(Add screenshot)<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/b95a7688-5b8b-47ef-a345-c3a5546388d3" />


------------------------------------------------------------------------

## Task 2 --- Capture Network Traffic

Run:

    sudo tcpdump

Let the capture run for about 20 seconds.

### Screenshot

(Add screenshot)<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/79a16c9a-9749-4720-b4f6-07d4bde651ed" />


### Questions

1.  What types of traffic do you observe? I observed different types of network traffic, including TCP, UDP and DNS packets. These packets show communication between my computer and other devices on the network."


Por exemplo, podes encontrar algo semelhante a:
2.  Can you identify IP addresses? yes, there are 2 types
3.  Do you see DNS queries?
Yes, I can see DNS queries in the captured network traffic. They are used to translate domain names, such as google.com, into IP addresses so that my computer can connect to the correct server."

### Reflection

Explain what network monitoring can reveal about system activity.
Network monitoring can reveal important information about how a computer system and network are being used. It allows administrators to observe network traffic, identify suspicious activity and detect potential security threats.
Network traffic: Shows the types of data being sent and received, such as TCP, UDP and DNS traffic.
Connected devices: Identifies which devices are connected to the network.
Communication activity: Shows which computers or servers are communicating with each other.
Suspicious activity: Helps identify unusual connections, unauthorised access attempts or potential cyberattacks.
System performance: Helps detect slow connections, high bandwidth usage and network problems.
DNS requests: Shows which domain names devices are trying to access.

Using sudo tcpdump, an administrator can monitor network packets and identify which devices are communicating, what protocols they are using and whether there is unusual network activity.


------------------------------------------------------------------------

## Task 3 --- Security Discussion

### Questions

1.  Could sensitive information appear in network traffic? yes , it can appear, when devices communicate over a network, information is connected without encryption attackers who intercept the network traffic may be able to read it.
2.  Why is HTTPS important for protecting communications?
   HTTPS (Hypertext Transfer Protocol Secure) protects communication between a user's browser and a website by using encryption through TLS (Transport Layer Security).

### Reflection

Describe what you learned about network visibility and security.
i could realise that the encryption is very important to keep the sensitive information safe from the attackers.
