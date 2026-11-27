# Exploring the CIA Triad

## Objective

Understand the **Confidentiality, Integrity and Availability (CIA)** principles using practical tasks on a Raspberry Pi.

---

# Part 1 – Confidentiality

1. Create a confidential file.

    ```bash
    nano secrets.txt
    ```

1. Write some confidential information.

1. Save the file.

1. Now restrict access:
    ```bash
    chmod 600 secrets.txt
    ```
1. Check permissions:
    ```bash
    ls -l secrets.txt
    ```

**Questions**
- Who can read this file?  Just me .
- How does file permission protect confidentiality? when no one else can see my files, it is protected.

## Part 2 – Integrity

1. Create a hash of the file.
    ```bash
    sha256sum secrets.txt
    ```
    _What does "hash" do?
it gave me lots of numbers followed by my file name secrets.txt
1. Save the output.

1. Modify the file.
    ```bash
    nano secrets.txt
    ```

1. Run the hash again.


** Questions**
- Did the hash change? yes , it did
- Why do security systems use hashing? Hashing is a one-way process. Unlike encryption, which is designed to be reversed using a decryption key, hashing is designed to produce a fixed-length value that cannot feasibly be reversed to recover the original data.

A simple way to remember the difference:
- Hashing: Protects and verifies data.
- Encryption: Protects data by converting it into a form that can be decrypted with the correct key.


# Part 3 – Availability

1. Check system uptime:
    ```bash
    uptime
    ```

1. List running processes:
    ```bash
    top
    ```

**Questions**
- Why is system uptime important?
  System uptime is the amount of time a computer system, network or service is operational and available for users.

Uptime is important because:
1. Availability: Ensures users can access systems and services whenever they need them.
2. Productivity: Allows employees to complete their work without interruptions.
3. Customer satisfaction: Customers can access websites, applications and services without problems.
4. Business continuity: Helps businesses continue operating and avoid disruptions.
5. Financial stability: Reduces the risk of losing money due to system downtime.
6. Reliability: Shows that a system is dependable and can be trusted.
For example, an online banking system needs high uptime so customers can access their accounts and make payments at any time.
2. What happens if a system is unavailable?

   
When a system is unavailable, users cannot access or use its services.

This can lead to:
- Loss of productivity: Employees cannot complete tasks that depend on the system.
- Financial losses: Businesses may lose sales and revenue.
- Customer dissatisfaction: Customers may become frustrated if services are unavailable.
- Data access problems: Important information may become temporarily inaccessible.
- Disruption to operations: Normal business activities may stop.
- Reputational damage: Customers may lose trust in the organisation.
- What happens if a system is unavailable?



## Deliverables
Include:
- Screenshot of file permissions:<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/6a30e4fb-96fc-46ca-9d81-ac5b0336402f" />
- 
- Screenshot of hash results<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/652b6ab4-b77d-4771-9a52-a30381986c55" />
- 
- Answers to questions
- Reflection
    >Explain how this activity demonstrated the CIA triad.
    >i could realize how important the Triad is for cyber security to keep our information safe.
    >
