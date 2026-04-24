# Network Segmentation & Security Design

## Overview

This project documents a segmented network architecture designed to enforce least-privilege access and isolate device classes using VLANs and firewall policies.

---

## Objectives

- Isolate network traffic by function
- Protect critical infrastructure
- Reduce attack surface
- Enable controlled inter-VLAN communication

---

## VLAN Design (Abstracted)

| VLAN | Purpose |
|------|--------|
| VLAN 10 | Management |
| VLAN 20 | Clients |
| VLAN 30 | IoT |
| VLAN 40 | Servers |
| VLAN 50 | VPN |

---

## Security Model

- Default deny between VLANs
- Explicit allow rules only
- Restricted management access
- VPN-only administrative entry

---

## Firewall Design

- Rule-based segmentation
- Network group abstraction
- Service-specific allowances

---

## Design Principles

- Least privilege access
- Separation of concerns
- Defense-in-depth
- Predictable traffic flow

---

## Lessons Learned

- Poor segmentation leads to lateral movement risk
- IoT devices must be isolated
- Firewall clarity is more important than complexity
- Naming conventions matter for scalability

---

## Future Improvements

- Rule automation
- Logging and traffic analysis
- Zero-trust enhancements

---

## Sanitization Notice

All addressing and topology details are generalized.