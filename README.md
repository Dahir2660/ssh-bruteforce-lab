# SSH Brute-Force Attack Simulation Lab

## Overview
This project demonstrates SSH brute-force attack simulation and detection techniques using Hydra and Linux security tools in a controlled lab environment.

## Objectives
- Simulate SSH brute-force attacks
- Analyze authentication logs
- Detect failed login attempts
- Understand password attack techniques
- Practice basic defensive security monitoring

## Tools Used
- Kali Linux
- Hydra
- OpenSSH
- journalctl
- fail2ban
- Wireshark
- Nmap

## Skills Demonstrated
- Linux administration
- Threat detection
- Authentication monitoring
- Brute-force attack analysis
- Log investigation
- Basic incident response

## Lab Activities
### SSH Brute-Force Simulation
Used Hydra to simulate password attacks against a Linux SSH service running in a virtual lab environment.

### Authentication Log Investigation
Analyzed Linux authentication logs to identify:
- Failed login attempts
- Repeated authentication failures
- Suspicious login activity

### Defensive Security Measures
Configured fail2ban to automatically block repeated failed SSH login attempts.

## Sample Commands
```bash
hydra -l kali -P passwords.txt ssh://127.0.0.1

sudo journalctl | grep "Failed password"

sudo systemctl start ssh

nmap -sV 127.0.0.1
```

## Key Takeaways
This lab improved my understanding of SSH security, password attacks, Linux log analysis, and basic SOC monitoring techniques used to detect suspicious authentication activity.
