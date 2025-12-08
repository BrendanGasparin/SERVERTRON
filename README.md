# Project: SERVERTRON
SERVERTRON aims to be a replicable, documented DevOps environment that can host many applications and services on a single physical machine.  

I am creating mine on a 64GB RAM mini-PC.  

Here are the project [docs/](docs/overview.md).  

The 8 phases of the interative DevOps cycle are:  

1. [phases/1.PLAN](phases\1.PLAN\README.md): Goals, constraints, risk register, threat model, service inventory.  
2. CODE: Ansible, Docker Compose, scripts, and configuration as code.  
3. BUILD: Proxmox install notes, VM/LXC layout, and template definitions.  
4. TEST: Test plans, smoke tests, backup restore tests, checklists.  
5. DEPLOY: Web server configs, TLS setup, DNS records, deploy runbooks.  
6. OPERATE: Runbooks, backups, maintenance, and security hardening.  
7. MONITOR: Prometheus, Grafana, logging, and alerting configuration.  
8. INTEGRATION: Postportems, changelog, roadmap, and lessons learned.  

Then the cycle repeats with feedback from the previous loop informing new plans.  

PLAN -> CODE -> BUILD -> TEST -> DEPLOY -> OPERATE -> MONITOR  
  ^                                                       ^  
  |                                                       |  
  ---------------- INTEGRATION / FEEDBACK -----------------  
