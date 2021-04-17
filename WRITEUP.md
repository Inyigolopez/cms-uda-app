# Write-up Template

### Analysis

We are going to compare the option of deploying our application in an Azure WEB APP or the possibility of hiring a virtual machine.

If we had the APP in our own virtual machine, we would have full control of our code while deploying it in an APP we do not. 

In terms of costs, having a basic virtual machine in Azure can cost us 20€/month (adding a hard disk) while with a Web App we can forget about the cost of the infrastructure for an approximate price of 12€/month.

With a VM we guarantee that we have scalability in such a way that if the number of users of our APP grows exponentially we can increase the size of our VM and support the volume of visits, while with a WebAPP it would be more complicated and we would have to redeploy the APP in a new Azure plan.

In terms of availability, an APP guarantees 24x7 availability while the deployment in our own VM requires processes that guarantee that our APP does not fail or in case of failure it will automatically be up again, implemented by ourselves.

### Resolution

Since we can deploy the APP from Git or from Github, we can keep our development environment local and once we have the APP ready for deployment we can deploy it in Azure; that way we can keep control over the code.

On the other hand, since we don't want to reach a lot of people with this APP, we can afford that our APP is not scalable, so it is not worth assuming higher costs to deploy it in our own VM.
In terms of security, it is not an application that requires strong control protocols, so we can deploy it in an Azure WEB APP. 

Additionally, the 24x7 availability of Azure Service WEB APPs makes us choose this option all the more reason to do so. 

### Assess app changes that would change my decision.

In case we needed to deploy an APP that would be consumed globally and had strong security requirements, my decision would have been to deploy it on our own Azure VMs, as this would give me the possibility to scale quickly if needed and to have strong control over our code and architecture to be able to be more flexible in this way.