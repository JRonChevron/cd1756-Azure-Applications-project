# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

| Criteria | Azure Web App (App Service) | Azure Virtual Machine (VM)| 
|----------|-----------------------------|---------------------------|
|Monthly cost	| $0 (Free F1 Tier Plan)	| From ~$16/month (Basic / General Purpose Plan)	|
|Scalability	| Virtual machine scale sets - Integrated	| Virtual machine scale sets - Manual |
|High availability	| Azure Traffic Manager and Azure Front Door	| Azure Traffic Manager, Azure Front Door, and cross-region Azure Load Balancer |
|Deployment	| Integrated support for GitHub Actions, CLI, etc.	| CI/CD must be manually set up|
|Maintenance	| Azure manages OS, runtime, patching	| Fully self-managed (OS, updates, security)|

For this project, I had to choose between using a Virtual Machine (VM) or an App Service (Web App) to deploy my CMS application. I chose App Service because it’s a fully managed platform, which means I don’t have to handle the infrastructure myself. Also, we need to consider that costs are lowwer, and it also includes features like automatic scaling, built-in monitoring, and easy deployment options. As someone who is still learning, this made the whole process super simple.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
If I had chosen a Virtual Machine, I would need to set up the server myself (install Python, Flask, Git, etc.), manually configure the web server, and handle updates, patches, and scaling on my own.
This would give me more control, but it would also be more complex and time-consuming — especially for a small project like this.
