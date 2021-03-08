# Hetzner VM Routing

The goal of this repository is to simplify the process for hosting Virtual Machines (VMs) on Hetzner dedicated servers.


# Architecture Overview

We will assume the following design throughout the process for simplicity sake as it applies to most users.
```mermaid
graph TD

A[WAN]  -->B(Dedicated Server)

B --> |Network Bridge|C{Virtual Machines}

C -->|One| D[CentOS]

C -->|Two| E[Debian]

C -->|Three| F[FreeBSD]

C -->|Four| G[Windows]}
C --> D
```
