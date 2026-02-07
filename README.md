# GNS3 Networking & Security Labs

A collection of hands-on network topologies focused on enterprise design, traffic segmentation, and security validation. These labs simulate real-world workflows for **NOC/SOC operations**, emphasizing observable evidence over simple "it works" connectivity.

## Project Focus

Instead of just basic connectivity, these labs prioritize:

* **Granular Segmentation:** Implementing VLANs and VRFs to define security boundaries.
* **Traffic Control:** Enforcing least-privilege access via ACLs and Firewalls (North-South/East-West).
* **Evidence-Based Validation:** Proving policy enforcement through packet captures and log analysis.
* **Structured Troubleshooting:** Documenting root causes and systematic fixes for complex outages.

---

## Lab Architecture

Every lab follows a standardized structure to mirror professional documentation workflows:

```
/lab-name
├── configs/            # Clean startup configurations for all nodes
├── verification/       # Evidence: screenshots of routing tables, NAT, and ACL hits
├── troubleshooting.md  # Detailed logs of symptoms, RCA, and resolution
├── lessons-learned.md  # Architectural takeaways and design optimization
└── README.md           # Topology diagram, addressing plan, and scope
```

---

## Featured Lab: Campus-VLAN-Firewall-ACL

This lab simulates a multi-tier enterprise environment using a FortiGate firewall and Layer 3 Core switches.

**Key Features:**

* **OSPF Routing:** Dynamic route propagation between the core and perimeter.
* **Inter-VLAN Security:** Hardware-level ACLs on the core and stateful inspection on the FortiGate.
* **NAT/PAT:** Managing egress traffic for internal and guest segments.
* **Verification:** Includes `show access-lists` hit counts and end-to-end connectivity logs.

---

## Technologies & Tools

* **Infrastructure:** GNS3, Cisco IOS (VLANs, Trunking, EtherChannel).
* **Routing/Security:** OSPF, NAT/PAT, ACLs, FortiGate (FortiOS).
* **Endpoints:** Linux (Ubuntu/Alpine) for traffic generation and testing.
* **Validation:** Wireshark, ICMP/TCP testing, and CLI-based verification.

---

## Author

**Christelle Janine M. Lureñana,** Network & Cybersecurity Student

---
