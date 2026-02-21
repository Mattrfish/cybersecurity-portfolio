# **Cybersecurity Homelab**
## What is a cybersecurity homelab?

A home lab serves as a miniature replica of professional IT environments, meticulously crafted for learning, experimentation, and skill development. It’s a controlled space where cybersecurity enthusiasts can immerse themselves in real-world scenarios, test diverse tools and techniques, and acquire practical experience — all without jeopardizing live systems or networks." [1] 

**Project Goal:**  To architect, deploy, and secure a multi-tier virtualized environment for the purpose of simulating real-world attack vectors and validating defensive security controls.

## Project Overview
This repository documents the creation of a segmented, isolated sandbox designed to mimic a corporate infrastructure. In the world of cybersecurity, it is vital to understand both how an attacker thinks and how a defender reacts. This lab provides a safe, "sandbox" environment where I can practice these skills without any risk to my personal computer or home network.

By building this from the ground up, I am gaining a deep understanding of networking, system administration, and security monitoring. This lab serves as my personal training ground to stay ahead of evolving digital threats.

## Project Objectives
The primary focus of this project is to bridge the gap between theoretical knowledge and hands-on application. 

**My objectives include:**
* **Hands-on Exploitation:** Learning how vulnerabilities are discovered and used by attackers to gain access to systems.
* **Defensive Hardening:** Implementing security settings and firewalls to stop those same attacks.
* **Monitoring and Logging:** Setting up systems that "watch" the network and alert me when suspicious activity happens.
* **Documentation:** Practicing the professional habit of recording technical steps, which is a critical skill in any security role.

## Architecture
To make this lab effective, I have designed it to be modular. It isn't just one computer; it is a network of virtual machines that talk to each other.

### Network Topology
The lab is split into two main zones:
**1.  The Attacker Zone:** Contains tools used for scanning and exploitation.
**2.  The Target Zone:** Contains the systems I am trying to protect (and practice breaking into).

These zones are strictly separated to ensure that all "malicious" activity stays contained and cannot leak out into my actual home network.

-- This section will be updated with step-by-step documentation of my network routing, subnet masking, and firewall rules as the build progresses. --

## Hardware
Currently, I am running this entire environment on my primary PC using virtualization. This allows me to run multiple operating systems simultaneously without needing a room full of servers.

-- This section will be updated with step-by-step documentation regarding hardware resource allocation (CPU/RAM) and performance optimization for multiple concurrent VMs. -- 

**Future Expansion:** I plan to integrate a Raspberry Pi 3 to handle specific network tasks and eventually build a Kubernetes cluster to explore cloud security. I am also looking into repurposing old hardware to create a dedicated, physical server for 24/7 security monitoring.

## Software
To manage my virtual machines, I am utilizing VMware and VirtualBox. These "hypervisors" allow me to create, delete, and reset my lab environments in seconds. If I break something (which is the point of the lab), I can simply revert to a previous "snapshot" and start again.

## Configuration and Setup
-- This section will be updated with step-by-step documentation of my build process and technical decision-making. --

### Attacking Machine
My primary tool for testing is Kali Linux. It comes pre-installed with a suite of tools for network analysis and penetration testing. I have configured this machine to reside on a private network where it can only communicate with my lab targets.
### Vulnerable Machine
The targets consist of both Windows and Linux systems. Some are "intentionally vulnerable" machines (like Metasploitable) designed for practice, while others are standard installations that I misconfigure on purpose to see if I can detect the resulting security gaps.

## Tech Stack
* **Virtualization:** VMware Workstation / VirtualBox
* **Operating Systems:** Kali Linux, Windows Server, Ubuntu
* **Security Tools:** Nmap, Wireshark, Metasploit, Hydra, Burp-Suite, GoBuster, John-the-ripper
* **Defensive Tools:** SIEM (Security Information and Event Management), Firewalls, Snort (IDS)

## References
[1] Banson, D. (2024). Building Your Cybersecurity Playground: What is a Home Lab? [online] Medium. Available at: https://medium.com/@daveitt/building-your-cybersecurity-playground-what-is-a-home-lab-f6dd2f995ab7 [Accessed 24 Jan. 2026].

‌
