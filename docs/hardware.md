# Hardware Inventory

This document contains the hardware currently used in the homelab infrastructure.

The inventory will be updated as new devices are added or existing hardware is upgraded.

---

## Current Hardware

| Device | Model | Role | RAM | Storage | Status |
|---|---|---|---|---|---|
| Managed Switch | Cisco SF302-08P | Core network switch | N/A | N/A | Active |
| Mini PC | Qotom Q305P | Dedicated firewall/router | 8 GB | TBD | Pending configuration |
| Mini PC | Zotac ZBOX | Virtualization server | 8 GB | 240 GB SSD | Active |
| Laptop | GDP | Management workstation | 32 GB | 2 TB M.2 SSD | Active |

---

## Cisco SF302-08P

**Role:** Core managed switch

Main managed switch responsible for connecting and segmenting the physical homelab infrastructure.

### Functions

- Network connectivity
- VLAN segmentation
- Access and trunk ports
- Infrastructure network management

### Specifications

- **Model:** Cisco SF302-08P
- **Type:** Managed Switch
- **Management:** Web / CLI
- **VLAN Support:** IEEE 802.1Q

**Status:** Active

---

## Qotom Q305P

**Role:** Dedicated firewall/router

The Qotom Q305P is dedicated to providing routing, security, and traffic management for the homelab.

### Planned Functions

- Firewall
- Routing
- NAT
- DHCP
- DNS
- VPN
- Inter-VLAN routing
- Traffic management

### Specifications

- **Model:** Qotom Q305P
- **RAM:** 8 GB
- **CPU:** TBD
- **Storage:** TBD
- **Network Interfaces:** TBD
- **Operating System:**  OPNsense

**Status:** Pending configuration

---

## Zotac ZBOX

**Role:** Virtualization server

The Zotac ZBOX serves as the main compute and virtualization server of the homelab.

### Functions

- Virtual machines
- LXC containers
- Internal services
- Database environments
- Testing environments

### Specifications

- **Model:** Zotac ZBOX
- **RAM:** 8 GB
- **Storage:** 240 GB SSD
- **CPU:** TBD
- **Network Interfaces:** TBD
- **Hypervisor:** Proxmox VE

**Status:** Active

---

## GDP Laptop

**Role:** Management workstation

The GDP laptop is the primary workstation used to administer and manage the homelab infrastructure.

### Functions

- SSH administration
- Proxmox management
- Network administration
- Firewall administration
- Database administration
- Infrastructure documentation
- Git/GitHub management

### Specifications

- **Model:** GDP
- **RAM:** 32 GB
- **Storage:** 2 TB M.2 SSD
- **CPU:** TBD
- **Network Interfaces:** TBD
- **Operating System:** TBD

**Status:** Active

---

## Planned Hardware

The following components are planned for future expansion.

| Component | Purpose | Status |
|---|---|---|
| NAS | Centralized storage and backups | Planned |
| HDD Enclosure | External storage expansion | Planned |
| HDDs | NAS storage | Planned |
| UPS | Power protection | Planned |
| Wireless Access Point | Managed wireless connectivity | Planned |
