# linux-hardening-lab

## Overview

**Wormz Cyber Lab** is a hands-on cybersecurity project organized by the **Wormz Cybersecurity Club**.
The goal of this project is to help members practice real-world cybersecurity skills such as network configuration, system hardening, traffic analysis, attack simulation, and detection techniques.

Participants will work in teams to build and analyze a small virtual lab environment in order to understand how cyber attacks work and how systems can be secured and monitored.

---

## Objectives

The main objectives of this project are:

* Understand **network architecture**
* Install and configure **virtual machines**
* Perform **network traffic analysis**
* Apply **security hardening techniques**
* Simulate **basic cyber attacks**
* Detect suspicious activity using **system logs**

---

## Project Organization

The project is organized into **five teams**.
Each team has its own directory in the repository and must complete all tasks inside its folder.

```
wormz-cyber-lab
│
├── team-1
├── team-2
├── team-3
├── team-4
└── team-5
```

---

## Team Directory Structure

Each team must organize their work using the following structure:

```
team-x
│
├── architecture
├── setup
├── network
├── traffic-analysis
├── security
├── attack
├── detection
└── report
```

---

## Expected Content

### Architecture

* Network diagram of the lab environment.

### Setup

* Installation and configuration of the virtual machines.

### Network

* IP configuration
* Connectivity tests (ping, network verification).

### Traffic Analysis

* Packet captures using **Wireshark** or **tcpdump**.
* Analysis of captured network traffic.

### Security

Security configuration such as:

* SSH hardening
* Firewall configuration
* Fail2Ban installation and configuration.

### Attack

Simulation of basic attacks such as:

* Nmap scans
* Brute-force attempts
* Network probing.

### Detection

* Analysis of system and authentication logs.
* Identification of suspicious or malicious activity.

### Report

Final report summarizing:

* Work completed
* Tools used
* Results obtained
* Lessons learned.

---

## Working Method

Each team must follow these steps:

1. Clone the repository.
2. Work only inside their team directory.
3. Commit their work regularly.
4. Push their updates to the repository.

Example:

```
git clone https://github.com/wormz-club/wormz-cyber-lab
```

Add files and commit:

```
git add .
git commit -m "Team 2 - Network configuration"
git push
```

---

## Useful Commands

### Network Scanning (Nmap)

Scan a network:

```
nmap 192.168.1.0/24
```

Scan services and versions:

```
nmap -sV 192.168.1.10
```

---

### Packet Capture

Capture packets using tcpdump:

```
sudo tcpdump -i eth0
```

Save captured packets:

```
sudo tcpdump -i eth0 -w capture.pcap
```

---

### SSH

Connect to a remote machine:

```
ssh user@192.168.1.10
```

Generate SSH keys:

```
ssh-keygen
```

---

### Firewall (UFW)

Enable firewall:

```
sudo ufw enable
```

Allow SSH:

```
sudo ufw allow ssh
```

Check firewall status:

```
sudo ufw status
```

---

### Fail2Ban

Check Fail2Ban status:

```
sudo fail2ban-client status
```

Restart Fail2Ban:

```
sudo systemctl restart fail2ban
```

---

### Log Analysis

View authentication logs:

```
sudo cat /var/log/auth.log
```

Search failed login attempts:

```
grep "Failed password" /var/log/auth.log
```

---

## Evaluation Criteria

Teams will be evaluated based on:

* Quality of the **technical work**
* Organization and completeness of the **GitHub repository**
* Quality of the **final report**
* **Project presentation**

---

## Wormz Cybersecurity Club

This project is part of the activities of the **Wormz Cybersecurity Club**, where members collaborate to learn cybersecurity through practical labs and real-world scenarios.

**Learn • Practice • Secure**
