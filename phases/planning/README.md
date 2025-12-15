# Planning Phase  

## 1. Problem Statement  
Project: SERVERTRON exists to provide a secure, reproducible, single-node platform for hosting both Internet-facing and home services, using DevOps and platform engineering practices.  

## 2. Goals and Non-Goals  
SERVERTRON should:  
- Demonstrate DevOps practices such as Infrastructure as Code and the DevOps cycle.
- Apply GitOps (even if it is only on one node).
- Run secure-by-default networking.
- Provide full documentation and runbooks.

The following are not goals of Project: SERVERTRON:  
- High availability  
- Multi-node Kubernetes  

## 3. Constraints  
Project: SERVERTRON is affected by the following constraints:  
- A single physical machine  
- Finite RAM and storage  
- Residential Internet connection with copper wiring from the node to the premises  
- Must survive reboots and power loss  
- Mostly open-source tooling  

## 4. Stakeholders
The following stakeholders may have concerns with Project: SERVERTRON:  
- The owner and operator  
- End users, including website visitors, Minecraft players, and Plex viewers  
- Future reviewers, including recruiters, interviewers, and visitors to this Github account  
- Threat actors using the external Internet  

## 5. Service Inventory  
The following services will be installed as part of the scope of this project: 

| Service | Purpose | Exposure | Data | Criticality |
|---------|---------|----------|------|-------------|
| Web | Personal website | Internet | Medium | High |
| Minecraft | Game server | Internet | Medium | Medium |
| Plex | Media server | LAN | High | Low |
| Monitoring | Visibility | LAN | Medium | Medium |
