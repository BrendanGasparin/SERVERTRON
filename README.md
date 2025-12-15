# Project: SERVERTRON  
SERVERTRON aims to be a replicable, documented DevOps environment that can host many applications and services on a single physical machine.  

I am creating mine on a 64GB RAM mini-PC called SERVERTRON-1.  

Here are the project [docs/](docs/overview.md).  

## The DevOps Cycle  
The 8 phases of the iterative DevOps cycle are:  
1. [Planning](phases/planning/README.md): Goals, constraints, risk register, threat model, service inventory.  
2. Coding: Ansible, Docker Compose, scripts, and configuration as code.  
3. Building: Proxmox install notes, VM/LXC layout, and template definitions.  
4. Testing: Test plans, smoke tests, backup restore tests, checklists.  
5. Deployment: Web server configs, TLS setup, DNS records, deploy runbooks.  
6. Operation: Runbooks, backups, maintenance, and security hardening.  
7. Monitoring: Prometheus, Grafana, logging, and alerting configuration.  
8. Integration: Postportems, changelog, roadmap, and lessons learned.  

Then the cycle repeats with feedback from the previous loop informing new plans.  

## Goals  
The goals of Project: SERVERTRON are to create a Proxmox installation running Linux containers and virtual machines and to document and make the process as replicable as possible.  

This will include the following containers or VMs:  
- Web server with WordPress sites accessible over the Internet.  
- Plex media server on the local network.  
- Minecraft server playable over the Internet, administered using RCON over a local network.  
- ARK: Survival Evolved server playable over the Internet.  
