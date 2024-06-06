  # Sanat
---
[![Typing SVG](https://readme-typing-svg.demolab.com?font=VT323&size=40&duration=2000&multiline=true&repeat=false&random=false&width=510&height=150&lines=Software+Engineer;Distributed+Systems+%7C+Blockchain;Cyber+Security)](https://git.io/typing-svg)

btw I’m currently learning 🌱 rusttt🦀 !!!

---
# Highlights
---
## Distributed Systems
Distributed Systems and Computing is the field of study that powers various applications such as Blockchains, Cloud Services and P2P applications. It is a paradigm concerned with ensuring consistency, fault tolerance, and efficient communication among distributed components in a network of computing devices. Given below is the summary of the fundamental concepts underpinning this field.  

<img src="https://github.com/s4nat/s4nat/assets/65476084/7182d41a-e841-4daa-8b7b-685fba7f8e10" alt="Distributed systems concepts" width="500" height="400">

Below are some of my personal projects in the area of Distributed Systems.

### [DNS on Chord](https://github.com/s4nat/dns-chord)
📑[Original Chord Paper](https://example.com/path/to/your/file.pdf)

📑[DNS on Chord Report](https://github.com/s4nat/s4nat/files/15230838/50_041_Distributed_Systems_Project.pdf)

DNS on Chord is a fault tolerant P2P Distributed Hash Table which aims to replace the legacy hierarchical structure of the current DNS network. When a user of DNS on Chord attempts to retrieve DNS records for a particular hostname from the legacy DNS network, it ports over the record to the distributed P2P network where a network participant contributes to hosting the record.
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

### Bully Algorithm
The Bully Algorithm is a classic election algorithm used in distributed systems to elect a leader among a group of nodes even in the event of node crashes. In distributed systems, having a single leader is often crucial for coordinating actions and ensuring consistent decision-making. Election algorithms like the Bully Algorithm facilitate the selection of a leader node that can oversee and coordinate the activities of other nodes in the system.

### Distributed Mutual Exclusion


### [IVY File System](https://github.com/s4nat/ivy)
Ivy is a multi-user read/write peer-to-peer file system. Ivy has no centralized or dedicated components, and it provides useful integrity properties without requiring users to fully trust either the underlying peer-to-peer storage system or the other users of the file system. This repo is a Go-based implementation of fault-tolerant Ivy Architecture with a backup central manager for consistent (meta)data handling during primary CM failures.

---
## Security
### Buffer Overflow Exploits
### Unix Privilege Separation 
### DNS Kaminsky Attack
### TCP SYN Flooding
### 

## Software Engineering
### MonstyrXAI 
### [ByteBass](https://github.com/s4nat/bytebass)

📑[ByteBass Presentation](https://github.com/s4nat/s4nat/files/15236518/ByteBass.pdf)

📑[ByteBass Report](https://github.com/s4nat/s4nat/files/15236529/PLC.Report.pdf)

ByteBass is an application written entirely in C which takes bass guitar audio in wav file format and parses it to determine the musical notes being played. The parsed notes are then fed into a Finite State Machine which determine's whether the notes being played follow a musical certain scale or not.

### [ByteWallet](https://github.com/s4nat/digitalWallet)


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
