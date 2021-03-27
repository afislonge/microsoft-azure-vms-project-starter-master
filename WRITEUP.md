# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

### Virtual Machine (VM)
IaaS option giving the developer complete control over deployment and the technology stack of the operating system. Provides tiers getting into substantially more memory and CPU cores.
- They are more expensive
- Multiple VMs can be grouped to provide high availability
- Multiple VMs can be grouped to provide high scalability

### App Service
PaaS option allowing the developer to focus on app development while receiving less control over the deployment pipeline. Tiers provide less memory and CPU cores.
- Cost less than VMs
- Vertical or Horizontal scaling capability, without having to redeploy.
- Achieve high availability with SLA-backed uptime of 99.95%.

### Deployment Option

**The project deployed to App Service**

### Justification

I choose an App Service in this situation because of the following
- Lightweight APIs tend to be well-suited to App Services over VMs, and won't approach the size limit for App Services very easily. Additionally, 
- App Services cost less than VMs do. 
- It can scale quickly with less concern, and don't need to factor that into the analysis.
- It can scale vertically to meet different demand levels
- The compute resources needed are well within App Service limits.
 
### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

App Service was used for the deployment, the following would have to chnage for me to change my decision

- A vast increase in the number of users
- The need for dedicated servers for security reasons
- More features added to the project
- Demand changes in a way that requires vertical scaling