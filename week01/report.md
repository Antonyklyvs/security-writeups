# Week 01 — Nmap Recon & Lab Setup

## Executive Summary
One-line: what you did and the main outcome.

## Scope
- Attacker: Kali (host)
- Target: Metasploitable2 (lab-only)
- Note: Lab-only, all targets are VMs under my control.

## Tools
- nmap (vX.Y.Z), VirtualBox, Wireshark

## Commands & Raw Output (sanitized)
### Host discovery
`nmap -sn 192.168.56.0/24`
<sanitized output or link to artifact>

### Version detection
`nmap -sC -sV -oA week01/week1_scan 192.168.56.101`
<sanitized output excerpt>

## Findings
- 22/tcp ssh — OpenSSH X.Y
- 80/tcp http — Apache/2.4.XX
- 3306/tcp mysql — version...
- Prioritized next steps: directory enumeration, webapp testing.

## ATT&CK Mapping
- Initial Access: T1078 (Valid Accounts) — example mapping
- Discovery: T1046 (Network Service Scanning)

## Remediation & Recommendations
- Close unnecessary services
- Apply strict firewall rules
- Harden SSH (disable password auth, use keys)

## Artifacts
- `assets/screenshot1.png`
- `outputs/week1_scan.nmap` (sanitized)

## Lessons Learned
Short bullet list.

