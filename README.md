# SDN ARP Handling using POX and Mininet

## 📌 Problem Statement
Implement ARP request and reply handling using an SDN controller.

## 🎯 Objective
- Intercept ARP packets
- Generate ARP responses
- Enable host discovery
- Apply match–action flow rules

---

## 🧠 Concept
In traditional networks, ARP uses broadcast, which is inefficient and insecure.

In this project:
- The controller handles ARP centrally
- Maintains IP-to-MAC mapping
- Controls communication using flow rules

---

## 🏗️ Topology

Star topology with one switch and three hosts.

![Topology](topology/topology.pdf)

---

## ⚙️ Setup

```bash
sudo mn -c
cd ~/pox
./pox.py log.level --DEBUG openflow.of_01 arp_controller
