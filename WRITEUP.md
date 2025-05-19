# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For both a VM or App Service solution for the CMS app:*

*Analyze costs, scalability, availability, and workflow*
*Choose the appropriate solution (VM or App Service) for deploying the app*
*Justify your choice*

Criteria           | Azure Web App (App Service)                       | Azure Virtual Machine (VM)
Monthly cost       | From ~$13/month (Basic B1 plan)                   | From ~$25/month (B1s Linux VM, no disk or IP included)
High availability  | Included in Standard plans and above              | Requires additional configuration
Scalability	       | Built-in auto-scaling                             | Manual scaling, requires custom setup
Deployment         | Native support for GitHub Actions, ZIP, FTP, CLI  | CI/CD must be manually set up
Maintenance        | Azure manages OS, runtime, patching               | Fully self-managed (OS, updates, security)

For this project, I had to choose between using a Virtual Machine (VM) or an App Service (Web App) to deploy my CMS application. I chose App Service because it’s a fully managed platform, which means I don’t have to handle the infrastructure myself. It also includes features like automatic scaling, built-in monitoring, and easy deployment options. As someone who is still learning, this made the whole process super simple.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
If I had chosen a Virtual Machine, I would need to set up the server myself (install Python, Flask, Git, etc.), manually configure the web server, and handle updates, patches, and scaling on my own.
This would give me more control, but it would also be more complex and time-consuming — especially for a small project like this.
