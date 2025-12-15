# Planning Phase  

## 1. Problem Statement  
Project: SERVERTRON exists to provide a secure, reproducible, single-node platform for hosting both Internet-facing and home services, using DevOps and platform engineering practices, along with thorough documentation and Infrastructure as Code.  

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
- The residents who share the gateway router to the Internet  
- End users, including website visitors, Minecraft players, and Plex viewers  
- Future reviewers, including recruiters, interviewers, and other visitors to plaforms used to document the project (e.g. GitHub)  
- Threat actors using the external Internet  

## 5. Service Inventory  
The following services will be installed as part of the scope of this project: 

| Service | Purpose | Exposure | Data | Criticality |
|---------|---------|----------|------|-------------|
| Web | Personal and business websites | Internet | Medium | High |
| Minecraft | Game server | Internet | Medium | Medium |
| Plex | Media server | LAN | High | Low |
| Monitoring | Visibility | LAN | Medium | Medium |

## 6. Trust & Threat Model  
The web server and Minecraft server will be exposed to the Internet. But administrative capabilities and communication with any databases will be limited to the local host. Plex service will be limited to the local network due to a low upload speed to the Internet on the premises.    
The threats if the server were to compromised are relatively low as, at least initially, the server will only host my own websites, a Minecraft server, and media content. With the potential for the addition of ecommerce capabilities to websites, and the desire to follow good DevOps practices throughout the project, good security practices are vital.  

## 7. Architecture  
The architecture of SERVERTRON-1 will be as follows:  
![Architecture diagram](../images/SERVERTRON-1-architecture.png)


## 8. Infrastructure as Code Boundaries


## 9. Risks and Trade-Offs


## 10. Success criteria  
- The system should be as replicable as possible from Git alone  
- Services survive reboot without intervention  
- Each major design decision should be documented  
- A third party must be able to understand the repository  
