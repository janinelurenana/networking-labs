# Networking Labs

## Overview
This repository contains hands-on networking labs built in GNS3, designed to reflect the responsibilities of **SOC analysts, NOC engineers, and junior network engineers**.

The labs emphasize:
- correct network design and segmentation
- controlled traffic flow and security boundaries
- verification through observable evidence
- structured troubleshooting and root-cause analysis

The goal is not just connectivity, but **visibility, control, and validation**.

---

## What This Repo Demonstrates (Role-Aligned)

### For NOC / Junior Network Engineer
- VLAN segmentation and inter-VLAN routing
- Dynamic routing (OSPF) and route verification
- NAT implementation and translation validation
- Layer 2 / Layer 3 integration
- Baseline configuration management
- Connectivity and failure testing

### For SOC / Security-Oriented Roles
- Traffic control using ACLs and firewalls
- Enforcement of least-privilege access between VLANs
- North–South and East–West traffic awareness
- Policy verification through packet flow outcomes
- Documentation of misconfigurations and security-impacting failures

---

## Lab Structure
Each lab follows a documentation-first, evidence-backed structure:

```
/lab-name
├── configs/             # Device startup configurations
├── verification/        # Screenshots proving behavior and policy
├── troubleshooting.md   # Symptoms, root causes, and fixes
├── lessons-learned.md   # Technical and design takeaways
└── README.md            # Lab scope, design, and validation steps
```

This mirrors real operational workflows:
- deploy
- observe
- verify
- troubleshoot
- document

---

## Example Lab
### Small_Enterprise_VLAN_OSPF_NAT_ACL

This lab simulates a small enterprise network with:
- multiple VLANs across access switches
- inter-VLAN routing via routed links
- OSPF for internal route exchange
- NAT for Internet-bound traffic
- ACLs enforcing inter-VLAN access control

**Verification artifacts include:**
- OSPF neighbor formation
- routing table propagation
- NAT translation entries
- enforced ACL blocks between VLANs
- successful and failed connectivity tests

Each behavior is validated with screenshots and logs, not assumptions.

---

## Technologies & Concepts
- VLANs and trunking
- Inter-VLAN routing
- OSPF (single-area)
- NAT (PAT)
- ACLs (security segmentation)
- Firewall integration (FortiGate in later labs)
- GNS3-based simulation
- Linux hosts for testing and validation

---

## Disclaimer
These labs are educational simulations built to reflect real-world networking and security principles.  
They are not production environments.

---

## Author
Built and maintained by Christelle Janine M. Lureñana  
IT student focused on networking and cybersecurity

