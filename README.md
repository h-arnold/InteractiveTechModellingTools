# Interactive Teaching Tools

- [Interactive Teaching Tools](#interactive-teaching-tools)
  - [Introduction](#introduction)
- [WJEC A-Level Computer Science](#wjec-a-level-computer-science)
  - [Fixed vs Variable Length Records Simulator](#fixed-vs-variable-length-records-simulator)
    - [Visualising Storage Structure](#visualising-storage-structure)
    - [The Access Speed Race](#the-access-speed-race)
- [WJEC GCSE Computer Science](#wjec-gcse-computer-science)
  - [1.1 Systems Architecture](#11-systems-architecture)
    - [FDE Cycle Simulator (WIP 🏗️)](#fde-cycle-simulator-wip-️)
  - [1.3 Networks and Communications](#13-networks-and-communications)
    - [DoS Attack Simulator](#dos-attack-simulator)
    - [Data Interception and Theft Simulators](#data-interception-and-theft-simulators)
    - [Password Cracking Simulator](#password-cracking-simulator)
- [Level 2 Extended Certificate in IT User Skills (ITQ)](#level-2-extended-certificate-in-it-user-skills-itq)
  - [Video Upload Pages Mockups](#video-upload-pages-mockups)

## Introduction

This repository contains links to all of the interactive modelling tools I've created to help students explore and interact with various concepts.

Almost all of these tools were vibe-coded using Google Gemini and so the code quality will probably be iffy. [I do write nice code when I write it myself, promise!](https://github.com/h-arnold/AssessmentBot)

It's now possible to create a similar resource yourself in 10-15 minutes - the sort of time it used to take me to create a worksheet. See the guide below for details on how you can do this youself:

[How to Create Your Own Interactive Classroom Resources with AI](HowToMakeYourOwnResources.md)

#Certainly. I have reinstated the links to both the live websites and their respective GitHub repositories for your convenience.

---

# WJEC A-Level Computer Science

## Fixed vs Variable Length Records Simulator

[Website](https://h-arnold.github.io/FixedVsVariableLengthRecordsSimulator/) | [Repo](https://h-arnold.github.io/ALevelOrganisationAndStructureOfDataSimulators/)
This tool visualises how data is stored on a disk and compares access speeds, helping students grasp the trade-off between storage efficiency and access performance.

### Visualising Storage Structure

This activity allows students to input data and toggle between "Fixed" and "Variable" storage modes.

* **Fixed Length:** Demonstrates how the system reserves uniform space (e.g., 15 bytes), filling unused space with padding. This visualises internal fragmentation/wasted space.
* **Variable Length:** Demonstrates dynamic allocation where records take up only the space they need, often using terminators or length headers, eliminating padding but introducing overhead.

### The Access Speed Race

A comparative simulation where students race a "Memory Controller" to find a specific record (e.g., Record #450).

* **Fixed Length (Calculated):** Shows how the computer calculates the exact address instantly (Direct Access / ) using the formula: .
* **Variable Length (Serial):** Shows the disk read head physically "walking" through the data (Serial Access), scanning for terminators or reading length headers to find the next record, highlighting the latency difference.

---

# WJEC GCSE Computer Science

## 1.1 Systems Architecture

### FDE Cycle Simulator (WIP 🏗️)

[Website](https://h-arnold.github.io/FDESimulator/) | [Repo](https://github.com/h-arnold/FDESimulator/deployments/github-pages)
An interactive model of the CPU designed to scaffold the understanding of the Fetch-Decode-Execute cycle.

* **Cycle Visualisation:** Students can interact with the cycle using 'Step' (to pause at each stage) or 'Run' (continuous flow).
* **Component Interaction:** The simulation visually highlights data movement across the **System Buses** (Address, Data, Control) and updates the contents of specific registers (**PC, MAR, MDR, CIR, ACC**) and the **ALU** in real-time, reinforcing the specific role of each component during the cycle.

## 1.3 Networks and Communications

### DoS Attack Simulator

[Website](https://h-arnold.github.io/DoSAttackSimulator/) | [Repo](https://github.com/h-arnold/DoSAttackSimulator)

A "Red Team / Blue Team" sandbox environment where students can act as both the attacker and the network administrator to understand the impact of Denial of Service attacks and how to mitigate them.

Attack Vectors: Students can configure an "Attacker" to launch specific types of floods (UDP, TCP SYN, ICMP) and scale the attack from a single device (DoS) to a botnet (DDoS) to overwhelm the server.

Defensive Measures: The simulation features a "Firewall & Mitigation" panel, allowing students to experiment with Blocking Protocols, enabling Rate Limiting, or deploying infrastructure upgrades like Load Balancing and Reverse Proxies to absorb the traffic.

Impact Visualisation: The tool visually demonstrates the consequences of an attack via a "User Happiness" metric (showing legitimate users being denied service) and Server Resource monitors (CPU/RAM and Bandwidth usage).

### Data Interception and Theft Simulators

[Website](https://h-arnold.github.io/DataInterceptionAndTheftSimulators/) | [Repo](https://github.com/h-arnold/DataInterceptionAndTheftSimulators)
A comprehensive suite of 5 simulations demonstrating network vulnerabilities.

* **Session Hijacking:** Students play the role of an attacker to observe how an unencrypted session cookie can be stolen and injected into a browser to impersonate a victim.
* **Packet Sniffer:** A "Wireshark-style" interface where students can capture network traffic, filter packets, and inspect payloads to find unencrypted credentials.
* **Man-in-the-Middle (MitM):** An interactive scenario where students intercept packets between two parties, modifying the messages before forwarding them, demonstrating active interception.
* **IP Spoofing & Evil Twin:** Demonstrates how a Rogue Access Point (Evil Twin) combined with spoofing a source IP address can trick simple firewalls and users.
* **DNS Cache Poisoning:** Shows how a DNS resolver can be tricked into caching a forged IP address, redirecting users from a legitimate site to a malicious one.

### Password Cracking Simulator

[Website](https://h-arnold.github.io/PasswordCrackingDemo/) | [Repo](https://github.com/h-arnold/PasswordCrackingDemo)
Three distinct demonstrations to highlight the importance of password entropy and secure authentication.

* **Brute Force Attack:** Systematically attempts every possible character combination to crack a password, visually demonstrating the time cost associated with simple vs. complex passwords.
* **Dictionary Attack:** Uses a pre-compiled list of common words to attempt a crack, showing how this method is often faster than brute force for weak passwords.
* **Credential Stuffing:** Simulates the automated injection of leaked username/password pairs across multiple sites to demonstrate the dangers of password reuse.

---

# Level 2 Extended Certificate in IT User Skills (ITQ)

## Video Upload Pages Mockups

[Website](https://h-arnold.github.io/VideoUploadPageMockups/SiteMockup/index.html) | [Repo](https://github.com/h-arnold/VideoUploadPageMockups)
These mockups simulate the upload interfaces of popular social media platforms. They are designed to teach students about file formats, codecs, and compression trade-offs by enforcing specific "client-side" constraints. Students will learn about the codecs and formats and are then challenged with converting a video file and 'uploading' it to find out whether they've met the requirements.