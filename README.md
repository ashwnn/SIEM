# SIEM + XDR w/ Wazuh

A complete SIEM + XDR setup that uses Wazuh to monitor, detect, and respond to simulated security threats in a controlled environment. Adittionally testing and configuring to mitigate and work with dealing with real-world threats.

## Table of Contents
- [About The Project](#about-the-project)
  - [Learning Objectives](#learning-objectives)
- [Architecture](#architecture)
- [License](#license)
- [Contact](#contact)

### About The Project
This project is kind of just an overview and a skeleton for anyone who wants to learn Wazuh and it's components as well as working with SIEM + XDR monitoring solutions. Although not the most popular solution Wazuh is the quite comprehensive and covers the majority of aspects of a SIEM. This project is meant to give someone an in-depth understanding of how we can setup, maintain and evolve a SIEM system in smaller spaces such as a local buisness or organization.

Although managing smaller devices with anti-virus the goal of a SIEM is to help aggregate and track alerts across a large number of devices, automatically running customized prevention rules and enforcing specified policies. For this project I used two virtual machines in my Homelab to create the Wazuh Server & the endpoint. After which I will run simulated attacks on the endpoint.

### Learning Objectives

**SIEM Fundamentals**
- Log collection and normalization
- Event correlation and analysis
- Alert creation and management
- Dashboard creation and reporting

**XDR Capabilities**
- Endpoint detection and response (EDR)
- Threat hunting techniques
- Automated response mechanisms
- Cross-layer visibility

**Threat Detection**
- Understanding MITRE ATT&CK framework
- Recognizing attack patterns
- Identifying indicators of compromise (IOCs)
- Behavioral analysis

**Incident Response**
- Alert triage and prioritization
- Investigation workflows
- Containment strategies
- Documentation and reporting

### Architecture

**Network**
Virtualized Network with NAT.

**Virtual Machines**

**WZ-SRV — Wazuh Server (Ubuntu)**

- Central SIEM/XDR management server
- Runs Wazuh Manager (threat detection engine)
- Hosts Wazuh Indexer (data storage and search)
- Provides Wazuh Dashboard (web-based UI)

**STU-PID — Windows 11 Endpoint**
- Monitored client and attack target
- Runs the Wazuh Agent for telemetry collection
- Includes Atomic Red Team for simulations
- Hosts vulnerable applications for testing

## License

Distributed under the MIT License. See `LICENSE` for more information.
