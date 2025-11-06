# SIEM + XDR w/ Wazuh

A complete SIEM + XDR setup that uses Wazuh to monitor, detect, and respond to simulated security threats in a controlled environment. Adittionally testing and configuring to mitigate and work with dealing with real-world threats.

## Table of Contents
- [About The Project](#about-the-project)
  - [Learning Objectives](#learning-objectives)
- [Architecture](#architecture)
  - [Host Environment](#host-environment)
  - [Virtual Machines](#virtual-machines)
  - [Configuration](#configuration)
- [License](#license)
- [Contact](#contact)

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

## Architecture

### Host Environment
- **Platform**: Ubuntu Server with QEMU/KVM
- **Management**: Cockpit web GUI for VM management
- **Virtualization**: Two virtual machines on an isolated virtual network

### Virtual Machines

**WZ-SRV — Wazuh Server (Ubuntu)**
- Central SIEM/XDR management server
- Runs Wazuh Manager (threat detection engine)
- Hosts Wazuh Indexer (data storage and search)
- Provides Wazuh Dashboard (web-based UI)

**USER-PC — Windows 11 Endpoint**
- Monitored client and attack target
- Runs the Wazuh Agent for telemetry collection
- Includes Atomic Red Team for simulations
- Hosts vulnerable applications for testing

## License

Distributed under the MIT License. See `LICENSE` for more information.
