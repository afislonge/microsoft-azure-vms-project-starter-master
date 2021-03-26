# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

VM : IaaS option giving the developer complete control over deployment and the technology stack of the operating system. Provides tiers getting into substantially more memory and CPU cores.

Some of the benefits of VMs are:

VMs allow you full access and control of the VM.
Lower up-front cost compared to purchasing and maintaining hardware.
Support of both Linux and Windows VMs.
Multiple types to choose from, such as compute or memory-optimized VMs, along with varying amounts of CPU, RAM and storage.
VMs allow for the installation of custom images and are an excellent choice for migrating from an on-premises server to the cloud.
Multiple VMs can be grouped to provide high availability, scalability, and redundancy. There are two options when it comes to scaling—Virtual Machine Scale Sets and Load Balancers. These will be covered in a different course.
Some of the limitations of VMs are:

They are more expensive
They can be more time consuming for the developer than other compute options

App Service : PaaS option allowing the developer to focus on app development while receiving less control over the deployment pipeline. Tiers provide less memory and CPU cores.
Some of the benefits of using an App Service are:

Support of multiple languages, such as .NET, .NET Core, Java, Ruby, Node.js, PHP, or Python
High availability, auto-scaling and support of both Linux and Windows environments.
Continuous deployment model using GitHub, Azure DevOps, or any Git repo.
Vertical or Horizontal scaling. Vertical scaling increases or decreases resources allocated to our App Service, such as the amount of vCPUs or RAM, by changing the App Service pricing tier. Horizontal scaling increases or decreases the number of Virtual Machine instances our App Service is running.
You can set the amount of hardware allocated to host your application, and cost varies based on the plan you choose. There are three different tiers - Dev/Test, Production, and Isolated. We’ll be using the free option within Dev/Test for the exercises in this course.
Some of the limitations of an App Service are:

You have limited access to the host server, so you are unable to control the underlying OS or install software on the server.
You’re always paying for the service plan, even if your services or application isn’t running.
There are hardware limitations, such as a maximum of 14GB of memory and 4 vCPU cores per instance
While they support multiple languages, as noted in the benefits above, they are limited to just using those languages (as of when this course was built).


The project deployed to App Service


App Service
Adv
Support multiple langauges
High availability and auto-scalling
Vetical and horizontal scalling
Support linux and window
Support continuos deployent
Platfomr as as service(Pass)
Cost based service plan

Disadv
limited acccess to host sevrer (cant control os or install software)
cost - pay for service plan even your app is snot running
hardware limitation
limited set of programming languages



Vm 
Adv
Full access to Vms
No hardware purchase necessary
Support linux and windows
Flexible Type and sizes available
Support custoe images
Hihg availability and scalling

Disadv
genrally expensive compare to App service
Labour intensive

App services
Dont need control of the OS or custom software
The application is lightweight
The application does not need high performance compute power

Some key points that stood out to me were:

Deploying a series of lightweight APIs
Less concern about scaling up processing power
Cost-consciousness
I would choose an App Service in this situation. Lightweight APIs tend to be well-suited to App Services over VMs, and won't approach the size limit for App Services very easily. Additionally, App Services cost less than VMs do. Lastly, since the ability to scale quickly is less of a concern, we don't need to factor that into the analysis.

 it can scale vertically to meet different demand levels, and the compute resources needed are well within App Service limits.


Choice can change if
A vast increase in the number of users
The need for dedicated servers for security reasons

control we need over the underlying OS, security requirements

However, there's some consideration that Virtual Machines may be necessary in the near future if many more features are added, or demand changes in a way that requires vertical scaling.


### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 



An Azure PaaS option allowing developers to focus more on their apps than the underlying infrastructure. It is an HTTP-based service for hosting web applications, REST APIs, and mobile back ends. It supports multiple languages and continuous deployment. While they are good for scaling, there is also a limit of up to 14 GB or 4 CPU cores on the highest tier.