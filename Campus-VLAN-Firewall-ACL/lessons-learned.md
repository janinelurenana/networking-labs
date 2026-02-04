# Lessons Learned

## Technical Lessons

* An **L3 switch can effectively replace a traditional router** for inter-VLAN routing in a campus or small enterprise design, reducing cost and operational complexity.

* Firewall operation reinforced that **routing correctness is a prerequisite for security policy enforcement**; NAT and policies are irrelevant without proper return paths.

* Using a **summarized internal route (10.10.0.0/16)** on the firewall simplified the routing table and made the design easier to scale as VLANs grow.

## Design & Process Lessons

* Separating **east–west traffic control (core ACLs)** from **north–south control (firewall policies)** resulted in clearer responsibility boundaries and easier troubleshooting.

* End-to-end validation **(internal → internet success, guest → internal failure)** was essential to confirm that the design intent matched real network behavior.