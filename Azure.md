# 1] Microsoft IAM 

## IAM
- To access a specific resource in Azure  
- Uses Authentication frameworks such as password or MFA(Multi Factor Authentication)  
- Authorization - What kind of resource we can access and what access do we have  
- Auditing - Who accessed which reource  

### 1] User Management
Microsoft Entra ID Admin center allows admin to manage different user accounts and managing their profiles.

### 2] Group Management
Access control for group of specifies user, admin can assign permission for group, i.e multiple users at once.

### 3] Device Managemnt
Managing devices that can access organizational network.

### 4] Application Management
Managing application, making sure they are compliant with organizational policies, ensures the employees has access to only certain Application

### 5] Single sign on
Access to application at once

### 6] Self Service password reset

### 7] Multi Factor Authentication

### 8] Priveleged Identity management
Access management for Highly priveleged role


# 2] Microsoft Entra Product Family

Multi cloud identity and network access solution for microsoft 

1. Microsoft Entra ID  
2. Microsoft Entra ID Governance  
3. Microsoft Entra Workload Identity - Application nd services securely access azure resources.  
4. Microsoft Entra Internet Access - Web gateway solution that provides access for SAAS application and Microsoft 365 application  

## Microsoft Entra ID
1. Also known as Azure AD  
2. Identity provider  
3. Identity: Object in Microsoft Entra ID that gets authenticated.  
4. Tenant: All the information about the identities ae stored in the tenant(company-name.com)  
5. Account: Idenitity that has data associated with it.  
6. User: Verified account associated with the person  

### What we can do with Microsoft Entar ID
- User management  
- Authentication, SSO and MFA, Biometric  
- Authorization and RBAC  
- Security, complicance and Audits  


# 2] Azure Compute

### 1] VM
- IAAS compute

### 2] AKS
- AKS

### 3] Azure App Services
- PAAS for webapps  
- Supports nodejs, Python, .NET, Java, PHP  
- Autoscaling, CICD integration, custom domains, SSL  


# 3] Azure Network

### 1] Vnet, Subnets, Routes tables, NSG, ASG

#### Vnet
A Virtual Network in Azure is the fundamental networking building block that allows Azure resources to communicate  
securely with each other, the internet, and on-premises networks.  
Every VNet is assigned a private IP address range using CIDR notation.

#### Subnet
A subnet is a logical subdivision of a VNet used to organize and secure resources.  
Azure automatically creates system routes but custom routes can override them.

#### Route table
Route tables determine where network traffic should be forwarded.

#### NSG
Firewall rules at subnet or NIC level  
NSG is a layer 4 firewall used to control inbound and outbound traffic to Azure resources.

#### ASG
ASG logically groups virtual machines so that security rules can be applied based on application roles rather than IP addresses.  
ASGs are mainly used with NSG rules to implement application tier segmentation.

#### Azure LB
Azure Load Balancer is a layer 4 load balancer that distributes network traffic across multiple backend resources.

#### Azure App Gateway
Application Gateway is a layer 7 load balancer designed for web applications.

#### Azure Frontdoor
Azure Front Door is a global load balancing service operating at layer 7.

Features
- Global traffic distribution  
- SSL offloading  
- Content caching  
- Web application firewall  
- DDoS protection  

#### Azure VPM Gateway
Azure VPN Gateway enables secure communication between on-premises networks and Azure VNets using encrypted tunnels.

#### ExpressRoute
ExpressRoute provides private dedicated connectivity between on-premises infrastructure and Azure.

#### Private Endpoint
Secure access to PaaS services  

Private Endpoint provides private access to Azure PaaS services using private IP addresses within a VNet.

AKS -> Private Endpoint -> Storage Account


# 4] Azure Storage Services

Storage Account

### 1] Azure Blob storage
object storage[images, video, backups, Logs]

### 2] Azure Disk storage
Persistent for VM [premium ssd, std hdd, std ssd]

### 3] Azure File storage
Azure File Storage provides fully managed file shares accessible using SMB or NFS protocols.

### 4] Azure Queue storage
Queue Storage is a messaging service used for asynchronous communication between components.

### 5] Azure Table stotrage
Table Storage is a NoSQL key value store designed for large amounts of structured data.

### 6] Azure Data Lake Storage
data analytics [Spark, Hadoop, Databricks]

IAAS[VM, VMSS]  
PAAS[AKS, ACR]  
SAAS[Microsoft 365, copilot]


# 5] Azure Container Ecosystem

### 1] ACR

### 2] AKS integration
ACR, Azure Monitor, Azure Policy, Key Vault


# 6] Azure Monitpring and Logging

### 1] Azure Monitor
Collects metrics, logs and alerts

### 2] Log Analytics
Query logs using KQL

### 3] Application Insights
APM


# 7] Azure Security Services

### 1] Azure Key Vault
Secure secret Management - password, certificate and keys

### 2] Microsoft Defender for Cloud
Vulnerability scanning and threat detection


# 8] Infrastructure as a Code in Azure

### 1] ARM Templates
ARM templates are JSON files used to deploy Azure infrastructure declaratively  
ARM templates are native Azure IaC solution.

### 2] Bicep
Bicep is a domain specific language built on top of ARM templates.  
Bicep compiles into ARM templates before deployment.

### 3] teraform
Terraform is an open source Infrastructure as Code tool.


# 9] Azure Architecture Concepts

### Regions
Physical datacenter locations

### Availability zones
Different datacenters within regions

### Availability sets
Availability sets ensure virtual machines are distributed across multiple fault domains and update domains.

#### Fault Domains
Protect against hardware failures.

#### Update Domains
Ensure not all VMs are rebooted simultaneously during maintenance.
