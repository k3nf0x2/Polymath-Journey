# Polymath-Journey
## SETUP-2 homelab (VirtualBox/Host-only 192.168.20.0/24)

## Overview
This repo documents my homelab for sysadmin, blue-team, and portfolio projects. Everything is reproducible and uses only free tools.

## Network
- Subnet: 192.168.20.0/24 (Host-only)
- Gateway/Firewall: VyOS (Portal, 192.168.20.1)

## Hosts
| Host | Role | OS | IP | RAM/CPU |
|---|---|---|---|---|
| Portal | Virtual router/firewall | VyOS | 192.168.20.1 | 1 GB / 1 |
| Web | Web server | Alma Linux | 192.168.20.2 | 2 GB / 2 |
| File | Web + DNS + Monitoring | Alma Linux | 192.168.20.3 | 2 GB / 2 |
| DC1 | ADDS + DNS + DHCP | Windows Server 2022 | 192.168.20.4 | 2 GB / 2 |
| monitor-K | Analyst WS | Windows 10 | 192.168.20.5 | 3 GB / 2 |
| monitor-U | Analyst WS | Ubuntu 25.04 | 192.168.20.6 | 3 GB / 2 |
| monitor-W | Analyst WS | Windows 10 | 192.168.20.7 | 3 GB / 2 |

## Goals
- Become job-ready in 2 months (Linux/Windows admin)
- English to C1 in 4 months, JLPT N1 long-term
- Cybersecurity polymath in 2 years (purple-team focus)

## Repo structure
- docs/ — designs, decisions, READMEs per service
- diagrams/ — ASCII/Mermaid diagrams
- configs/ — sanitized configs (no secrets)
- runbooks/ — “how to operate” SOPs
- scripts/ — Bash/PowerShell utilities
- logs/ — daily logs, TIL, experiments
- templates/ — logging templates (how-to, what-is, TIL, postmortem)
- screenshots/ — proof of work

## Safety and secrets
- Never commit passwords, keys, tokens, or internal certs. Use placeholders like <REDACTED>.

## Reproduce
- Virtualization: VirtualBox
- Networks: Host-only + NAT as needed
- OS ISOs: Official vendor sites (free/eval)

## License
MIT
