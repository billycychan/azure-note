# Describe the core architectural components of Azure

# **What is Microsoft Azure**

Microsoft Azure is a **cloud computing service** designed by Microsoft, which provides users with a wide range of cloud services for computing, storage, and networking. 

Azure offers over 200 services, including AI and machine learning capabilities, and is accessible through an online portal with an active internet connection. 

Azure's billing is based on resource consumption, allowing users to pay for what they use and scale their resources accordingly. It provides users with the freedom to build, manage, and deploy applications on a global network using their preferred tools and frameworks. 

With Azure, users can run existing applications on virtual machines, explore new software paradigms, and leverage advanced technologies such as AI and mixed reality. The platform simplifies platform management, enables seamless unification of technology, and provides trusted cloud security.

# **Get started with Azure accounts**

**Azure free account?**

- for new users to get started with
- Free access to popular Azure products for 12 months
- A credit to use for the first 30 days
- Access to more than 25 product that are always free

**What is the Azure free student account?**

- Free access to certain software developer tools.
- give $100 credit and free devs tools, without a credit card

**What is the Microsoft Learn sandbox?**

- a temporary subscription that's added to your Azure account.

# **Describe Azure physical infrastructure**

**Physical Infrastructure**

- Azure’s is built around datacenters. They are in racks, with powers, cooling and networking infrastructure
- Datacenters are **grouped into Azure Regions or Azure Availability Zones** that are designed to help you achieve resiliency and reliability for your business-critical workloads.

**Regions**

- A region is a geographical area on the planet that contains at least one, but potentially multiple datacenters that are nearby and networked together with a low-latency network.

**Availability** **Zones**

- Availability zones are **physically separate datacenters** within an Azure region.
- Each availability zone is made up of **one or more datacenters equipped with independent power, cooling, and networking.**
- An availability zone is set up to be an isolation boundary. If one zone goes down, the other continues working.
- a minimum of three separate availability zones are present in all availability zone-enabled regions to ensure resiliency

**Region pairs**

Most Azure regions **are paired with another region** within the same geography (such as US, Europe, or Asia) at least 300 miles away.

Allows replication of resources across a geography that helpd reduce interruption from natrual disaster, civil unrest, power outages, physical network outage that affect entire region.

West US ↔ East US

South-East Asia ↔ with East Asia

West India and Brazil South (only one direction pairing)

Advantages:

- restored as quickly as possible for applications hosted in that region pair incase of outage
- Azure updates can be rolled out to one region at time to minimize downtiem and risks
- For tax and law-enforcement jurisdiction purposes

**Sovereign Regions**

- Sovereign regions are instances of Azure that are **isolated from the main instance of Azure**
- for compliance or legal purposes.
- **US DoD Central, US Gov Virginia, US Gov Iowa** and more: These regions are physical and logical network-isolated instances of Azure **for U.S. government agencies and partners.** These datacenters are operated by **screened U.S. personnel** and include additional compliance certifications.
- **China East, China North**, and more: These regions are available through a unique partnership between **Microsoft** and **21Vianet**, whereby Microsoft doesn't directly maintain the datacenters.

# **Describe Azure management infrastructure**

**Azure resources**  

- A resource is the basic building block of Azure.
- Anything that you create, provision, deploy is a resources.
- VMs, virtual networks, databases, cognitive services …

**Resource groups**

- Groupings of resources.
- A single resource can only be in one resource group at a time
- When you move a resource to a new group, it will no longer be associated with the former group.
- It could not be nested

**Azure Subscriptions**

- subscriptions are a unit of management, billing, and scale
- subscriptions allow you to **logically organize your resource groups** and facilitate billing.
- A subscription provides you with **authenticated and authorized access to Azure products** and services..
- two types of subscription boundaries that you can use:
    - **Billing boundary**: This subscription type determines how an Azure account is billed for using Azure.
    - **Access control boundary:** Azure applies access-management policies at the subscription level, and you can create separate subscriptions to reflect different organizational structures. (different departments, distinct Azure subscription policies)
- Three additional Azure subscription
    - **Environments**
        - to set up separate environments for development and testing, security, or to isolate data for compliance reasons
    - **Organizational structures**
        - o reflect different organizational structures
    - **Billing**
        - for billing purposes.(one subscription for your production workloads and another subscription for your development and testing workloads)

## Azure management groups

- Resources are gathered into resource groups
- Resource groups are gathered into subscriptions
- Azure management groups provide a level of scope above subscriptions
- Enterprise-grade management at a large scale
- Can be nested
- Usecases
    - Create a hierarchy that applies a policy
    - Provide user access to multiple subscription

![104](./104/104.png)