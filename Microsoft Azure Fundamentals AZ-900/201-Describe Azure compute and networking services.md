
# Describe Azure compute and networking services

## Describe Azure virtual machines

VMs provide **infrastructure as a service (IaaS)** in the form of a virtualized server and can be used in many ways

- OS control
- custom software
- custom hosting configuration
- An **image is a template used to create a VM and may already include an** OS and other software, like development tools or web hosting environments.

### **Virtual machine scale sets (scalability, capacity)**

- To create and manage a group of identical, load-balanced VMs.
- To centrally **manage, configure, and update a large number of VMs in minutes**. The number of VM instances can automatically increase or decrease in response to demand,

### **Virtual machine availability sets （resiliency）**

- a tool to build a more resilient and highly available environment by **staggering updates and providing varied power and network connectivity**
- grouping VMs in two ways:
    - update domain
        - allows you to apply updates while knowing that **only one update domain grouping** will be offline at a time
    - fault domain
        - groups your VMs by common power source and network switch
        - by default an availability set will split your VMs across up to three fault domains

VM Usecases:

- During tests and developments
- when running applications in the cloud
- extending your datacenter to the clud
- during disaster recovery

## Describe Azure virtual desktop

- A desktop and app virtualization service that runs in Azure
- Enable IT Pros and MSPs to create windows 10 & 11 virtual desktops in Azure
- Create a full desktop virtualization environment without having to run additional gateway servers

## Describe Azure container

Azure container are a light-weight, virtualized environment that does not require operating system management, and can respond to change in demand. 

- **Azure Container Instance (ACI)**
    - Runs Docker containers on-demand in a managed, serverless Azure environment
    - A solution for any scenario that can operate in isolated containers, without orchestration
- **Azure Container Apps**
    - Container Apps have extra benefits such as the ability to incorporate load balancing and scaling.
- **Azure Kubernetes Service**
    - a container orchestration service.
    - An orchestration service manages the lifecycle of containers. When you're deploying a fleet of containers, AKS can **make fleet management simpler and more efficient.**

## Describe Azure Functions

- Azure Functions is **an event-driven, serverless compute** option that doesn’t require maintaining virtual machines or containers.
- Azure has already help users to manage the servers
    - No infrastructure management, OS,
    - scalability, continue working under any workload
    - only what you use

## Describe Application Hosting options

**Azure App Service** 

- build and host webapps, background job, mobile back-ends, and RESTful apis in the programming language of your choice without managing infrastructure
- auto scaling and high availability1
- It supports multiple languages, including .NET, .NET Core, Java, Ruby, Node.js, PHP, or Python. It also supports both Windows and Linux environments.
- Web Apps, [ASP.NET](http://asp.net/), [ASP.NET](http://asp.net/) Core, Java, Ruby, Node.js, PHP, or Python.
- API Apps, Full swagger support, REST-based web API, like hosting website
- WebJobs, run program or script, could be scheduled or run by a trigger
- Mobile apps, cloud-based SQL databased, authentication, push notification, custom back-end Node.js, SDK Supports

## Describe Azure virtual networking

Azure virtual networks and virtual subnets **enable Azure resources,** such as VMs, web apps, and databases, **to communicate with each other, with users on the internet**, and with your on-premises client computers.

- Isolation and segmentation, to create multiple isolated virtual networks
- Internet communication, assigning a public IP address to an Azure resource
- Communicate between Azure resources
- Communicate with on-premises resources
- Route network traffic, route tabled defining rules how packages are routed between subnets
- Filter network traffic, (Network security groups, Network virtual appliances , Firewall)
- Connect virtual networks via virtual network peering

## Describe Azure virtual private networks

- VPN  uses an encrypted tunnel within another network
- Azure VPN Gateway, type of VPN
    - Policy based
        - specify statically the IP address of packets that should be encrypted through each tunnel.
    - Route based
        - IPSec tunnels are modeled as a **network interface** or virtual tunnel interface.

## Describe Azure ExpressRoute

- Azure ExpressRoute lets you extend your on-premises networks into the Microsoft cloud over a **private connection,** with the help of a connectivity provider. (ExpressRoute Circuit)
- ExpressRoute connections **don't route through the public internet**, providing users with more reliability, faster speeds, consistent latency, and higher security.

## Describe Azure DNS

- Azure DNS is a hosting service for **DNS domains that provides name resolution** by using Microsoft Azure infrastructure.
- Azure DNS also **supports alias record sets**. You can use an alias record set to refer to an Azure resource, such as an Azure public IP address, an Azure Traffic Manager profile, or an Azure Content Delivery Network (CDN) endpoint.