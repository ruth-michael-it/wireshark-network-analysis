# Network Traffic Analysis & Packet Inspection Lab (Wireshark)

This repository documents hands-on network troubleshooting, protocol verification, and baseline traffic analysis using Wireshark packet captures. The focus is on diagnosing network anomalies, inspecting core protocols, and analyzing security baselines.

## 🔍 Core Analysis Focus

### 1. The TCP Three-Way Handshake
Verified network connection initialization procedures by isolating clean TCP streams to confirm structural handshake sequences:
* **SYN:** Analyzed initial synchronization request containing client MSS parameters and sequence number allocation.
* **SYN-ACK:** Inspected server acknowledgement parameters confirming window scaling factors.
* **ACK:** Validated completion of connection state before active data payload transfer.

### 2. Network Anomaly Diagnosis
Utilized advanced Wireshark display filters to isolate transmission failures and performance bottlenecks:
* `tcp.analysis.retransmission`: Identified structural packet losses across the local network route.
* `tcp.analysis.duplicate_ack`: Documented early out-of-order segment arrivals triggering fast retransmit protocols.

### 3. Core Infrastructure Protocol Verification
* **DNS (Domain Name System):** Inspected transactional pairings of UDP standard queries and response strings to map name resolution delays.
* **ARP (Address Resolution Protocol):** Tracked structural broadcast requests mapping physical MAC addresses to logical IP layers across local subnets.

## 🛠️ Environment & Tools
* **Traffic Captures:** Wireshark v4.x
* **Environments Inspected:** Home-Lab Virtualized Network Stacks (Windows Server & Linux Instances)
* **Analyzed Protocols:** TCP, UDP, DNS, ARP, ICMP

## 💡 Practical Skills Demonstrated
* Proficient application of complex Wireshark display and capture filters.
* Replay and reconstruction of raw packet payloads to analyze application layer behaviors.
* Systematic isolation of network connectivity faults between endpoints.

