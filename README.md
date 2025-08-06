#PNETLab OSPF Lab: Two-Router Topology

This lab demonstrates a basic **OSPF (Open Shortest Path First)** configuration using two routers in **PNETLab**. It’s designed to help learners understand OSPF neighbor relationships, DR/BDR election, and basic IP routing.

## 🖥Topology Overview

- **Router R1**
  - Loopback: `1.1.1.1/32`
  - Link to R2: `10.0.0.1/30`
  - Role: **Backup Designated Router (BDR)**

- **Router R2**
  - Loopback: `2.2.2.2/32`
  - Link to R1: `10.0.0.2/30`
  - Role: **Designated Router (DR)**

## Configuration Highlights

- OSPF is enabled on all interfaces.
- Loopback interfaces are advertised in OSPF.
- DR/BDR election occurs on the shared `10.0.0.0/30` network.
- Basic routing is verified using `ping` and `show ip route`.

## Files Included

- `lab.pnet` – PNETLab topology file
- `R1.cfg` – Configuration for Router R1
- `R2.cfg` – Configuration for Router R2

## Getting Started

1. Import the `.pnet` file into your PNETLab environment.
2. Start both routers.
3. Verify OSPF adjacency using:
