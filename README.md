# homelab-infrastructure

Personal homelab project focused on networking, virtualization, Linux, databases, storage, containers, and infrastructure management.

This repository documents the design, implementation, and evolution of my personal IT infrastructure homelab.

The project aims to build a dedicated environment for designing and managing networks, deploying servers, working with virtualization, managing databases, implementing centralized storage, and experimenting with different infrastructure technologies.

Rather than deploying isolated services, the goal is to progressively build a complete infrastructure while documenting configurations, design decisions, issues encountered, and implemented solutions.

> **Project Status:** In Progress

---

## Objectives

The homelab is designed for hands-on practice and experimentation across different infrastructure areas:

- Linux system administration
- Network design and administration
- Switching
- VLAN segmentation
- Firewalls and security policies
- Server virtualization
- Database administration
- Containers
- Centralized storage
- Backup and recovery
- Infrastructure monitoring
- Automation
- Secure remote access
- System and network troubleshooting

---

## Current Infrastructure

The homelab currently consists of the following devices:

| Device | Role | Status |
|---|---|---|
| Cisco SF302-08P | Main managed switch | Available |
| Qotom Mini PC | Dedicated firewall/router | Pending configuration |
| Zotac ZBOX | Main server | Active |
| GDP Laptop | Management workstation | Active |

Complete device specifications are available at:

[Hardware Inventory](docs/hardware.md)

---

## Architecture

The infrastructure is designed with a separation of responsibilities between networking, computing, storage, and management.

- **Qotom Mini PC:** Main firewall and router running OPNsense.
- **Cisco SF302-08P:** Main managed switch for network connectivity and segmentation.
- **Zotac ZBOX:** Main server running Proxmox VE for virtual machines, containers, and services.
- **GDP Laptop:** Workstation used for infrastructure administration.

The architecture will evolve as VLANs, centralized storage, monitoring, and additional services are implemented.

[Architecture Documentation](docs/architecture.md)

---

## Networking

The network infrastructure is based on a Cisco managed switch and a dedicated device for firewall and routing functions.

The design will provide hands-on experience with:

- VLANs
- Access ports
- Trunk ports
- IEEE 802.1Q
- Spanning Tree Protocol
- Routing
- Inter-VLAN routing
- DHCP
- DNS
- NAT
- VPN
- Network segmentation
- Firewall policies
- Traffic monitoring

---

## Firewall and Routing

The Qotom Mini PC is intended to operate as the dedicated firewall and router for the infrastructure.

Its planned functions include:

- Firewall
- NAT
- DHCP
- DNS
- Routing
- Inter-VLAN routing
- VPN
- Traffic management
- Inter-network access policies
- Infrastructure segmentation

The firewall platform and its configuration will be documented once the implementation is complete.

---

## Switching

The Cisco SF302-08P serves as the main managed switch for the homelab.

Its implementation will provide hands-on experience with:

- VLANs
- Access ports
- Trunk ports
- IEEE 802.1Q
- Spanning Tree Protocol
- Network segmentation
- Switch administration
- Interface monitoring
- Port security

Configurations will be progressively documented as the network design evolves.

---

## Virtualization

The Zotac ZBOX serves as the main homelab server.

The virtualization platform in use is:

**Proxmox VE**

The server hosts virtual machines and containers, providing isolated environments for testing and running services.

Planned and current workloads include:

- Linux servers
- Databases
- LXC containers
- Docker services
- Internal services
- Monitoring tools
- Testing environments
- Automation

---

## Linux

Linux is an important part of the homelab environment.

The environment is used to practice and document tasks such as:

- User and group administration
- Permissions
- Service management with systemd
- Networking
- SSH
- Package management
- LVM
- Filesystems
- Logs
- Script-based automation
- Scheduled tasks
- Troubleshooting

---

## Databases

The homelab is used to deploy and administer different database management systems.

The goal is to provide environments for practicing:

- Installation
- Configuration
- Administration
- Users and privileges
- Storage management
- Backup and recovery
- Monitoring
- Troubleshooting
- Optimization

The initial focus is primarily on **Oracle Database**, with additional database systems planned for future implementations.

---

## Containers

The homelab includes services deployed using container technologies.

Technologies include:

- Docker
- Docker Compose
- LXC
- Self-hosted services

Each implemented service will be documented individually within the repository.

---

## Services

Services deployed within the homelab will be progressively documented.

Some of the planned services include:

| Service | Platform | Purpose | Status |
|---|---|---|---|
| Homelable | Proxmox / LXC | Homelab visualization and documentation | Planned |
| Oracle Database | Virtual Machine | Database administration lab | Planned |
| Docker | VM / LXC | Containerized services | Planned |
| Monitoring | VM / LXC | Infrastructure monitoring | Planned |

This list will be updated as new services are implemented.

---

## Storage

One of the next stages of the project is to implement a NAS for centralized homelab storage.

The NAS will be used for:

- Centralized storage
- Backups
- Shared files
- Virtual machine backups
- ISO images
- Service data
- SMB
- NFS

The storage solution is currently in the planning stage.

---

## Security

Security will be progressively incorporated into the infrastructure design.

Planned implementations include:

- VLAN segmentation
- Firewall rules
- IoT device isolation
- Management network
- VPN
- SSH access
- Principle of least privilege
- User and permission management
- Security updates
- Event monitoring

---

## Monitoring

A monitoring platform will be implemented to provide visibility into the status and performance of servers, services, and network infrastructure.

Monitoring will include:

- CPU
- RAM
- Storage
- Network interfaces
- Service availability
- Virtual machines
- Containers
- Databases
- Network traffic

---

## Backup Strategy

The homelab design will include a backup strategy.

The following areas will be progressively documented:

- Virtual machine backups
- Configuration backups
- Database backups
- Firewall configuration backups
- Switch configuration backups
- Retention policies
- Restore procedures

The goal is to ensure that virtual machines, configurations, and services do not depend exclusively on the local storage of individual devices.

---

## Roadmap

### Networking

- [x] Design IP addressing scheme
- [ ] Design VLAN architecture
- [ ] Configure Cisco SF302-08P
- [ ] Configure dedicated firewall/router
- [ ] Implement firewall rules
- [ ] Implement Inter-VLAN routing
- [ ] Implement VPN
- [ ] Document network topology

### Servers and Virtualization

- [ ] Complete Zotac server configuration
- [ ] Document Proxmox VE
- [x] Create virtual machines
- [x] Create LXC containers
- [x] Implement internal services
- [ ] Implement Homelable

### Storage

- [ ] Design NAS solution
- [ ] Implement centralized storage
- [ ] Configure SMB/NFS
- [ ] Integrate NAS with Proxmox
- [ ] Implement backup strategy

### Monitoring

- [x] Implement server monitoring
- [ ] Implement network monitoring
- [ ] Create dashboards
- [ ] Configure alerts

---

## Project Status

**In Progress**

The homelab is continuously evolving. The infrastructure and its documentation will be updated as new services, configurations, and improvements are implemented.

---

## Expected Result

The final goal is to build a segmented, manageable, and well-documented home infrastructure that serves both as a platform for personal services and as a hands-on environment for working with infrastructure technologies, networking, systems administration, databases, storage, security, and automation.
