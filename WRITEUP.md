# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

1. Costs:
VM: VMs typically involve higher costs due to the need for infrastructure provisioning, including virtual machine instances, storage, and network resources. Costs can vary based on the VM size, storage type, and data transfer.

App Service: App Service usually offers a more cost-effective solution as it abstracts away the underlying infrastructure management. You pay for the compute resources and any additional features like custom domains, SSL certificates, and scaling.

2. Scalability:
VM: Scaling VMs requires manual intervention or the implementation of auto-scaling solutions. It involves provisioning additional VM instances, load balancers, and managing traffic distribution.

App Service: App Service provides built-in auto-scaling features that can dynamically adjust resources based on demand. It simplifies scalability management and ensures optimal performance without manual intervention.

3. Availability:
VM: Achieving high availability with VMs requires implementing redundancy, fault tolerance, and load balancing configurations. This often involves setting up availability sets, virtual machine scale sets, and configuring geo-replication for data redundancy.

App Service: App Service offers high availability out-of-the-box with its global data center presence and built-in load balancing. It automatically handles infrastructure redundancy, failover, and traffic routing, ensuring high availability without additional configuration.

4. Workflow:
VM: Deploying and managing VMs typically involves more manual configuration and maintenance tasks, including OS updates, security patches, and application deployments. DevOps practices like Infrastructure as Code (IaC) with tools like Azure Resource Manager templates or Terraform can streamline deployment workflows.

App Service: App Service simplifies deployment and management with features like continuous integration and deployment (CI/CD), integration with version control systems like GitHub, and support for popular development frameworks like .NET, Java, Node.js, and PHP. It enables faster development cycles and easier deployment workflows.


=> For deploying a CMS app, Azure App Service is likely the better choice over a VM. It offers cost-effectiveness, built-in scalability, high availability, and streamlines deployment workflows. With App Service, you avoid the manual setup and maintenance associated with VMs, making it a more efficient and developer-friendly option.

### Assess app changes that would change your decision.

The decision to choose Azure App Service over a VM for deploying the CMS application could change if the application requires extensive customization, resource-intensive workloads, regulatory compliance, advanced networking configurations, or specialized management and monitoring needs that are not adequately supported by App Service. In such cases, opting for a VM deployment might be more appropriate.