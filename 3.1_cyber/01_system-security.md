# Exploring Your System's Security

## Task 1 --- List System Users

Run:

    cat /etc/passwd

### Screenshot

(Add screenshot here)<img width="1276" height="904" alt="image" src="https://github.com/user-attachments/assets/c48922b7-07ad-4439-8013-ed4b539a7f10" />


### Questions

1.  How many users exist on the system? lots
2.  Which accounts appear to be system accounts? systemd-timesync:x:991:991:systemed
3.  Why do operating systems create system accounts?
Operating systems create system accounts to manage and run essential services and background processes securely. These accounts have specific permissions and limited access, which helps prevent unauthorised users or programs from making changes to important system files.
### Reflection

Explain why understanding system users is important for cybersecurity.

Understanding system users is important for cybersecurity because it helps us identify who has access to a computer and what permissions they have. It allows us to detect suspicious activity, prevent unauthorised access, and reduce security risks. It also helps ensure that users and programs only have the permissions they need to perform their tasks.
------------------------------------------------------------------------

## Task 2 --- Inspect Running Processes

Run:

    ps aux

### Screenshot

(Add screenshot here)<img width="1714" height="888" alt="image" src="https://github.com/user-attachments/assets/62711f60-636c-4e1b-8d88-9e7ba37abfe2" />


### Questions

1.  Which processes are running as `root`? 378   0.0  0.0 435318112   3792   ??  Ss    8:54a.m.   0:00.01 autofsd
root               358   0.0  0.0 435355632   7408   ??  Ss    8:54a.m.   0:00.56 /usr/libexec/diskarbitrationd
root               355   0.0  0.2 435380416  63952   ??  Ss    8:54a.m.   0:59.47 /System/Library/Frameworks/

3.  Why can processes running as root be dangerous?
  Processes running as root are dangerous because root has full control over the operating system. If a process makes a mistake or is compromised, it could damage important system files, change security settings, or access sensitive information.


4.  What could happen if a malicious program ran with root privileges?

A malicious program running with root privileges could take complete control of the computer. It could steal personal information, delete files, install malware, disable security features, or create unauthorised user accounts.
### Reflection

What did you learn about system processes and security?

i learnt that root can be dangerous because they can have full control over the operating system, and malicious program ran with root priveleges could take com,plete control of the computer.

------------------------------------------------------------------------

## Task 3 --- Identify Open Network Ports

Run:

    ss -tuln

### Screenshot

(Add screenshot here)<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/9aa54f84-a8dc-4d02-93a7-abe6d08a910a" />


### Questions

1.  Which ports are open? 4096, 128
2.  Which services appear to be listening? 127.0.0.1:631, 0.0.0.0:22
3.  Why might open ports represent a security risk?
   Open ports can represent a security risk because they allow external devices to communicate with services running on a computer. If a port is open and the service is vulnerable or poorly secured, attackers could exploit it to gain unauthorised access.

### Reflection

Explain the relationship between open ports and potential attack
surfaces.
Open ports create potential entry points for cyberattacks. Attackers can scan for open ports to identify running services and weaknesses. They may exploit these vulnerabilities to steal data, install malware, or gain control of a system. Closing unused ports and securing necessary ones helps reduce security risks.
