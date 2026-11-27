# Basic Firewall Configuration

## Task 1 --- Install the Firewall

Run:

    sudo apt install ufw

### Screenshot
<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/ac77e741-5074-4380-8171-388ea651c543" />

(Add screenshot)<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/7c07d86a-db47-43ea-9209-8d75f06367dd" />


------------------------------------------------------------------------

## Task 2 --- Enable the Firewall

Run:

    sudo ufw enable

### Screenshot

(Add screenshot)<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/f93b907c-d97a-4a0d-88f8-546d4cb38905" />


### Questions

1.  What message appears after enabling the firewall?Firewall is active and enable on system startup
2.  Why are firewalls important?
3.  A firewall is a security system that monitors and controls incoming and outgoing network traffic. It helps protect computers and networks from unauthorised access and cyberattacks.

Firewalls are important for several reasons:
1. Prevent unauthorised access: Blocks people or devices that are not allowed to access a network.
2. Protect against cyberattacks: Helps defend systems against malicious network traffic and certain types of attacks.
3. Monitor network traffic: Checks incoming and outgoing data to identify suspicious activity.
4. Protect sensitive information: Helps prevent unauthorised users from accessing confidential data.
5. Control network access: Allows organisations to decide which websites, applications and services can communicate through their networks.
6. Improve network security: Acts as a barrier between trusted internal networks and untrusted external networks, such as the internet.

------------------------------------------------------------------------

## Task 3 --- Allow SSH Access

Run:

    sudo ufw allow ssh
    sudo ufw status

### Screenshot

(Add screenshot)<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/cd68ac17-331f-48a0-bb7e-82c31a523d2f" />


### Questions

1.  What rule was added? allow anywhere 
2.  Why must SSH be allowed?
   SSH (Secure Shell) is a network protocol that allows users and system administrators to securely access and manage computers remotely over a network.

SSH must be allowed when remote administration is required because:
1. Remote access: Allows administrators to access computers and servers from another location.
2. Secure communication: Encrypts data sent between the user's computer and the remote server.
3. System management: Allows administrators to configure systems, install software and perform maintenance remotely.
4. Troubleshooting: Helps IT staff diagnose and fix problems without physically accessing the computer.
5. File transfers: Supports secure file transfers between computers using tools such as SCP and SFTP.

### Reflection

Explain how firewalls help protect systems from unauthorised access.
firewall protect us by monitoring and controlling incoming and outcoming network traffic based on a set of security rules.
