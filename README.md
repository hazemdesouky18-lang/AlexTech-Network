# 🌐 Project 7: Build a Functional DNS & Web Server Network

## 🏢 Industry Scenario
**Client:** AlexTech Startup — Internal IT Infrastructure Launch

AlexTech is a brand-new tech startup in Alexandria with 10 employees. The founding team wants to host their own internal company website and use a custom domain name (`www.alextech.eg`) so employees can access it without memorizing an IP address.

> The startup's budget is tight — they cannot afford a cloud provider yet. This project builds and configures their internal DNS and web server infrastructure before the first day of operations.

---

## 🎯 Project Objectives

Set up a complete internal network in Cisco Packet Tracer that includes:
- A **DNS Server** for name resolution
- An **HTTP Web Server** hosting the internal company website
- **3 Client PCs** configured to use DNS
- Demonstrate the full journey of a browser request — from client → DNS → web server → back

---

## 📁 Project Structure

```
AlexTech-Network/
│
├── Phase_1_project_network.pkt   # Cisco Packet Tracer file (Phase 1 & 2)
└── README.md                     # Project documentation
```

---

## ✅ Phase 1 Tasks — Due: Week 9, April 5, 2026

| # | Task | Status |
|---|------|--------|
| 1 | Build AlexTech network: 1 DNS server, 1 HTTP server, 3 client PCs, 1 switch — same subnet | ✅ Done |
| 2 | Configure DNS server with an A record resolving `www.alextech.eg` → HTTP server IP | ✅ Done |
| 3 | Configure all 3 client PCs to use the DNS server as their name server | ✅ Done |
| 4 | Test DNS resolution from each client using `nslookup` — confirm correct IP returned | ✅ Done |

---

## ✅ Phase 2 Tasks — Due: Week 14, May 10, 2026

| # | Task | Status |
|---|------|--------|
| 1 | Open web browser on each client and access `www.alextech.eg` — confirm page loads | ✅ Done |
| 2 | Use Simulation Mode to trace full packet journey (DNS query → response → HTTP GET → response) | ✅ Done |
| 3 | Document every step: protocols, IP addresses, port numbers | ✅ Done |
| 4 | Present complete working system to instructor (AlexTech founders) | ✅ Done |

---

## 🖧 Network Topology

| Device | Role |
|--------|------|
| Server 1 | DNS Server |
| Server 2 | HTTP Web Server |
| PC 1–3 | Client PCs |
| Switch | Connects all devices on same subnet |

**Domain:** `www.alextech.eg`

---

## 🔄 Full Packet Journey (Phase 2)

```
Client PC
   │
   ├─── DNS Query (UDP, Port 53) ──────► DNS Server
   │◄── DNS Response (IP of HTTP Server) ─┘
   │
   ├─── HTTP GET (TCP, Port 80) ───────► HTTP Server
   │◄── HTTP Response (Web Page) ──────┘
   │
   └─── ✅ www.alextech.eg loads in browser
```

---

## 📦 Required Deliverables

- [x] Packet Tracer file (`.pkt`)
- [x] DNS & HTTP configuration screenshots
- [x] Process documentation (protocols, IPs, ports)
- [x] Live demo / presentation

---

## 🛠️ Tools Used

- Cisco Packet Tracer
- DNS (Port 53 / UDP)
- HTTP (Port 80 / TCP)
- `nslookup` command for testing
- Packet Tracer Simulation Mode

---

## 👥 Team

> Desouky Hatem

---

*Project completed — Phase 1 & Phase 2 submitted as part of the Networking course.*
