  # Sanat
---
[![Typing SVG](https://readme-typing-svg.demolab.com?font=VT323&size=40&duration=2000&multiline=true&repeat=false&random=false&width=510&height=150&lines=Software+Engineer;Distributed+Systems+%7C+Blockchain;Cyber+Security)](https://git.io/typing-svg)


---
# Highlights
---
## Distributed Systems
Distributed Systems and Computing is the field of study that powers various applications such as Blockchains, Cloud Services and P2P applications. It is a paradigm concerned with ensuring consistency, fault tolerance, and efficient communication among distributed components in a network of computing devices. Given below is the summary of the fundamental concepts underpinning this field.  

<img src="https://github.com/s4nat/s4nat/assets/65476084/7182d41a-e841-4daa-8b7b-685fba7f8e10" alt="Distributed systems concepts" width="500" height="400">

Below are some of my personal projects in the area of Distributed Systems which showcase my deep and practical understanding of the above concepts.

### [DNS on Chord](https://github.com/s4nat/dns-chord)
📑[Original Chord Paper](https://example.com/path/to/your/file.pdf)

📑[DNS on Chord Report](https://github.com/s4nat/s4nat/files/15230838/50_041_Distributed_Systems_Project.pdf)

DNS on Chord is a fault tolerant P2P Distributed Hash Table which aims to replace the legacy hierarchical structure of the current DNS network. When a user of DNS on Chord attempts to retrieve DNS records for a particular hostname from the legacy DNS network, it copies the record to the distributed P2P network where a network participant contributes to hosting the record. Eventually, the network will host majority of DNS records with a focus on the following features.
Some useful features of this protocol:
- Tolerates planned node departures
- Tolerates unplanned node deaths (due to replication of the records)
- Seamless node joins and redistribution of DNS records
- Fingertable which makes the lookup times for a record O(logN)


### [Lamport's Clock](https://github.com/s4nat/lamport-clocks)

In distributed systems and computing, Lamport's clock is a fundamental concept used to establish a partial ordering of events that occur across multiple nodes without relying on a centralized clock. Lamport's clock assigns timestamps to events in a distributed system to maintain their causal ordering. If event A influences event B, Lamport's clock ensures that the timestamp of A is earlier than that of B. However, if events are concurrent, their timestamps may not follow a specific order.

Lamport's clock is useful for:

- Total ordering of events across distributed nodes
- Concurrency Control - detect causality violations

### [Bully Algorithm](https://github.com/s4nat/Bully-Algo)
The Bully Algorithm is a classic election algorithm used in distributed systems to elect a leader among a group of nodes even in the event of node crashes. In distributed systems, having a single leader is often crucial for coordinating actions and ensuring consistent decision-making. Election algorithms like the Bully Algorithm facilitate the selection of a leader node that can oversee and coordinate the activities of other nodes in the system.

### [Distributed Mutual Exclusion](https://github.com/s4nat/dme)
Distributed systems sometimes access a part of the memory/ some resource that can only be accessed by one process at a time. Examples of such sensitive information includes distributed ledgers, shared documents, bank accounts, etc. Complex protocols have been developed for the seamless handling of these data accesses in order to prevent data corruption and avoid deadlock.

The repository linked above contains implementation of 3 such protocols:
- Lamport's Shared Priority Queue without Ricart and Agrawala’s optimization
- Lamport's Shared Priority Queue with Ricart and Agrawala’s optimization
- Voting Protocol with deadlock avoidance


### [IVY File System](https://github.com/s4nat/ivy)
📑[Original IVY Paper](https://systems.cs.columbia.edu/ds2-class/papers/li-ivy.pdf)

Ivy is a multi-user read/write peer-to-peer file system. Ivy has no centralized or dedicated components, and it provides useful integrity properties without requiring users to fully trust either the underlying peer-to-peer storage system or the other users of the file system. This repo is a Go-based implementation of fault-tolerant Ivy Architecture with a backup central manager for consistent (meta)data handling during primary CM failures.

---
## Security
### Buffer Overflow Exploits
📑[Lab Report](https://github.com/user-attachments/files/17743019/Lab.1.System.Security.pdf)

This lab explores memory vulnerabilities and their exploits. Key concepts and methods such as buffer overflows, code injections in stack, return-to-libC attacks and their corresponding defences have been grokked and implemented.

### Unix Privilege Separation
📑[Lab Report](https://github.com/user-attachments/files/17743043/Lab.2.System.Security.-.Privilege.Separation.pdf)

This lab explores privilege separation and Remote Procedure Calls (RPCs) in Linux environments. The implementation demonstrates the practical application of breaking down monolithic applications into microservices, with a focus on security through separation of responsibilities. We have utilized Linux system calls (setresuid, setresgid) for privilege management and configured granular access controls (chown, chmod) between separated services. The project showcases proficiency in secure system design, implementing controlled access points through RPCs, and managing precise permission controls in a Linux environment. This hands-on implementation emphasizes the importance of security-first architecture in modern system design.

### DNS Kaminsky Attack
📑[Lab Questions](https://seedsecuritylabs.org/Labs_20.04/Files/DNS_Remote/DNS_Remote.pdf)

📑[Lab Report](https://github.com/user-attachments/files/17743180/DNS.Kaminsky.Attack.Lab.pdf)

Unlike traditional DNS cache poisoning, which targets specific domain names, this attack manipulates the authoritative records for entire domains. The attacker floods a DNS resolver with multiple spoofed responses while simultaneously making requests for random, non-existent subdomains. By exploiting the limited entropy of DNS transaction IDs (16 bits) and source ports, the attacker has a higher probability of successfully injecting malicious DNS records into the resolver's cache. If successful, the attack can redirect legitimate traffic to malicious servers, potentially affecting all users relying on the compromised DNS resolver. This vulnerability led to the rapid deployment of source port randomization and DNSSEC as critical security measures.

### TCP SYN Flooding
📑[Lab Questions](https://seedsecuritylabs.org/Labs_20.04/Files/TCP_Attacks/TCP_Attacks.pdf)

📑[Lab Report](https://github.com/user-attachments/files/17743171/TCP.Attacks.Lab.pdf)

A TCP SYN Flood is a denial-of-service (DoS) attack that exploits TCP's three-way handshake mechanism. The attacker sends a flood of TCP SYN packets to the target server, often using spoofed IP addresses. For each SYN packet received, the server responds with a SYN-ACK and reserves resources (like memory buffers) while waiting for the final ACK to complete the handshake. However, since the source addresses are typically spoofed, these ACK packets never arrive. This leads to accumulation of half-open connections, exhausting the server's resources and preventing legitimate users from establishing connections. The server becomes overwhelmed as its connection queue fills up, leading to degraded performance or complete service unavailability.

### 

## Software Engineering
### [MonstyrXAI](https://github.com/s4nat/monstyrxai)
A comprehensive AI solution to automate the slow and tedious processes of a data entry job in a deals aggregation company.

### [ByteBass](https://github.com/s4nat/bytebass)
📑[ByteBass Presentation](https://github.com/s4nat/s4nat/files/15236518/ByteBass.pdf)

📑[ByteBass Report](https://github.com/s4nat/s4nat/files/15236529/PLC.Report.pdf)

ByteBass is an application written entirely in C which takes bass guitar audio in wav file format and parses it to determine the musical notes being played. The parsed notes are then fed into a Finite State Machine which determine's whether the notes being played follow a musical certain scale or not.

### [ByteWallet](https://github.com/s4nat/digitalWallet)
ByteWallet is a comprehensive digital wallet solution that combines the simplicity of Next.js for frontend development, robust authentication mechanisms for security, Node.js Express for backend functionality, and Stripe for easy and secure top-ups. 

<!--
**s4nat/s4nat** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
