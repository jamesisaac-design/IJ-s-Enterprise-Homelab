# Enterprise Security & Infrastructure Homelab

A self-hosted homelab simulating enterprise networking, firewall administration, VPN infrastructure, and secure remote access using a Fortinet firewall and Linux server.

## Overview

Production-style homelab focused on networking, security, and infrastructure operations. Built to practice real-world skills in a segmented, secure environment.

## Hardware & Core Components

- **Fortinet FortiGate 60F** (FortiOS 7.0.14) – Primary firewall and security gateway
- **Raspberry Pi 5** – Linux server hosted in DMZ
- Gigabit Ethernet switching
- External SSD storage

## Network Architecture

**Segmented Network Design**
- **DMZ Network**: 10.10.10.0/24
  - Gateway: 10.10.10.1
  - Linux Server: 10.10.10.10
- Isolated services zone with controlled external access
- NAT, Port Forwarding, and Virtual IP configurations

## Firewall Implementation (FortiGate)

- Comprehensive security policies (LAN-to-WAN, DMZ traffic control)
- NAT rules and Port Forwarding
- Virtual IP objects
- Traffic filtering and rule validation
- VPN integration

## WireGuard VPN Deployment

Fully functional self-hosted VPN solution for secure remote access.

**Features:**
- Public/private key authentication
- Full-tunnel configuration
- Automated client provisioning
- Mobile client support with QR codes
- Firewall integration and NAT traversal

**Automation:**
- Custom `add-client.sh` script for key generation, config creation, and QR code output

## Linux Server Administration

- Full management of Raspberry Pi OS server in DMZ
- Service configuration and hardening
- SSH access control
- Shell scripting and automation
- Network diagnostics (`ip`, `ss`, `tcpdump`, etc.)

## Troubleshooting & Validation

Hands-on diagnostics including:
- VPN handshake failures, routing, and NAT issues
- Firewall policy conflicts
- Port forwarding and connectivity problems

Tools used: `wg show`, `tcpdump`, `traceroute`, `ss`, `ip` suite, and FortiGate diagnostics.

## Technologies Used

**Networking & Security**
- Fortinet FortiGate, TCP/IP, NAT, Firewall Policies, Port Forwarding
- WireGuard VPN
- DMZ Architecture & Zero Trust principles

**Operating Systems & Tools**
- Linux (Raspberry Pi OS)
- Bash scripting
- SSH

## Future Enhancements

- VLAN segmentation
- Active Directory / Microsoft Entra ID integration
- SIEM / logging
- IDS/IPS testing
- Infrastructure automation

---

Built to strengthen enterprise networking, security, and systems administration skills.
