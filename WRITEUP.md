# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

### What I chose
I chose the App Service to deploy the CMS application.

### Analyze cost, scalability, avaliability and workflow:

- Cost: Azure App service is less expensive than Virtual Machines. A free tier is available.

- Scalability: Horizontal or vertical scaling are the two scaling techniques that App Service provides. Vertical scaling automatically increases or decreases resources allocated (CPUs, RAMs, etc.) to our App Service while horizontal scaling increases or decreases the number of VMs instances our App Service is running.

- Availability: App Services are highly available at a global scale, thanks to its SLA.

- Workflow: The App service support automated deployments from GitHub. Therefore, developers can create well-structured CI/CD pipelines for deploying their applications hosted in their Github repo.

### Overall Reasoning for my choice
- An App Service pretty much has everything that a developer like me deploy different types of applications (web, mobile, server, etc). It's secure, scalable, cheaperand easier to maintain compared to a virtual machine. A virtual machine requires a developer to control the underlying OS or installing softwares, which seems like an overkill for the CMS application.
The App service Support multiple languages including Python, which is what the CMS application was written in. Since all I want is to quickly build and deploy the CMS application to Azure, I don't think I will need a virtual machine where I will need to be responsible from maintenance to security. These are the reasons why I chose the App Service for deployment.


### Assess app changes that would change your decision. 

- App Services are limited by their hardware. If the CMS app grows to a larger scale, which involves large increase in the number of users, Virtual Machines are more preferred.

- For auto scaling and traffic management features, Virtual Machines will be more handy.

- App Services also supports limited number of programming languages. So, for other programming languages not supported by AS, I would go for a VM.
