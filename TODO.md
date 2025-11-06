### Phase 1: Environment Setup
1. Configure QEMU/KVM on the Ubuntu host.
2. Set up Cockpit for VM management.
3. Create an isolated virtual network for the lab VMs.
4. Deploy the Ubuntu VM for the Wazuh server.
5. Deploy the Windows 11 VM as the monitored endpoint.

### Phase 2: Wazuh Installation
1. Install the Wazuh all-in-one deployment on the Ubuntu VM.
2. Access the Wazuh Dashboard and complete initial configuration.
3. Configure firewall rules for agent communication.
4. Verify core Wazuh services are running.

### Phase 3: Agent Deployment
1. Download the Wazuh Windows agent.
2. Install and configure the agent on the Windows 11 VM.
3. Register the agent with the Wazuh Manager.
4. Verify agent connectivity and data flow.
5. Configure agent modules (FIM, syscollector, vulnerability detection).

### Phase 4: Attack Simulation Setup
1. Install Atomic Red Team on the Windows endpoint.
2. Install additional attack simulation tools:
   - Mimikatz (credential dumping)
   - PowerSploit (PowerShell exploitation)
   - Caldera (adversary emulation)
3. Optionally deploy vulnerable web applications:
   - DVWA (Damn Vulnerable Web Application)
   - WebGoat
4. Document the baseline system state.

### Phase 5: Testing and Detection
1. Execute Atomic Red Team techniques:
   - MITRE ATT&CK tactics (Initial Access, Execution, Persistence, etc.)
   - Privilege escalation attempts
   - Credential dumping
   - Lateral movement simulation
2. Generate web-based attacks:
   - SQL injection
   - XSS attacks
   - Brute force attempts
3. Monitor the Wazuh Dashboard for alerts.
4. Analyze detection coverage and data quality.

### Phase 6: Response and Tuning
1. Create custom detection rules tailored to observed behaviors.
2. Configure active response actions:
   - Automated blocking
   - Process termination
   - Script execution
3. Set up email or webhook alerting.
4. Fine-tune rules to reduce false positives.
5. Document incident response procedures.

### Phase 7: Advanced Features
1. Configure vulnerability detection scanning.
2. Enable compliance monitoring (CIS benchmarks).
3. Set up file integrity monitoring (FIM).
4. Implement log analysis for Windows Event Logs.
5. Create custom dashboards and visualizations.
6. Test integrations with external tools (VirusTotal, OSINT feeds).

## Roadmap

- [ ] Add network diagram(s) for quick visual reference.
- [ ] Publish automation scripts for VM provisioning.
- [ ] Provide sample alert playbooks and runbooks.
- [ ] Document optional integrations (SIEM data exports, SOAR hooks).