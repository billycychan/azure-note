# Describe cloud computing

- Define cloud computing.
- Describe the shared responsibility model.
- Define cloud models, including public, private, and hybrid.
- Identify appropriate use cases for each cloud model.
- Describe the consumption-based model.
- Compare cloud pricing models.

## What is cloud computing

- Cloud computing is the delivery of computing services over the internet
    - virtual machines, storage, databases, and networking
    

## Describe the shared responsibility model

![https://learn.microsoft.com/en-us/training/wwl-azure/describe-cloud-compute/media/shared-responsibility-b3829bfe.svg](https://learn.microsoft.com/en-us/training/wwl-azure/describe-cloud-compute/media/shared-responsibility-b3829bfe.svg)

Customers arae always responsibile for 

- The information and data stored in the cloud
- Devices that are allowed to connect your cloud
- The accounts and identities of the people, services, and devices within your organization

The cloud provider is always responsible for:

- The physical datacenter
- The physical network
- The physical hosts

The responsibilities of the service model will determine by 

- Operating systems
- Network controls
- Applications
- Identity and infrastructure

## Define Cloud Models

**Private Cloud**
A private cloud is a **single-entity cloud** that provides **greater control for companies** and their IT departments. However, it comes with **higher costs** and **fewer benefits** compared to public clouds. Private clouds can be hosted on-site or offsite by a third-party provider dedicated to the company.

**Public Cloud**
A public cloud is built, controlled, and maintained by a third-party cloud provider. Anyone can access and use resources in a public cloud, making it a key difference from private clouds.

**Hybrid Cloud**
A hybrid cloud **combines public and private clouds** in an interconnected environment. This allows for flexible deployment of services between the two environments, providing an extra layer of security and scalability.

**Comparative Table**

|  | Public Cloud | Private Cloud | Hybrid Cloud |
| --- | --- | --- | --- |
| Capital Expenditures | No | Yes | Flexible  |
| Control over Resources and Security | Limited | Complete | Flexible |
| Scalability | Easy | Challenging | Easy |
| Cost | Pay-per-use | Higher upfront costs | Varies |
|  |  |  |  |

**Multi-Cloud**
A multi-cloud scenario involves using multiple public cloud providers, either for different features or to migrate from one provider to another. This environment requires managing resources and security across two (or more) cloud providers.

**Azure Solutions**

- **Azure Arc**: A set of technologies that helps **manage cloud environments**, including private clouds, hybrid configurations, and multi-cloud scenarios.
- **Azure VMware Solution**: Allows organizations to run VMware workloads in Azure with seamless integration and scalability, making it easier to migrate from a private cloud environment to a public or hybrid cloud.

## Describe the consumption-based model

**Capital expenditure (CapEx)** 

A **one-time payment** made to acquire a tangible asset, such as equipment, property, or software.

 **Operational expenditure (OpEx).**

OpEx is spending money **on services or products over time.**

This consumption-based model has many benefits, including:

- No **upfront costs.**
- No need to **purchase and manage costly infrastructure** that users might not use to its fullest potential.
- The ability to **pay for more resources when they're needed.**
- The ability to **stop paying for resources that are no longer needed.**

Traditional datacenter, can sometimes under/over estimate the resouces.

## Compare cloud pricing model

pay-as-you-go pricing model

- Plan and manage your operating costs.
- Run your infrastructure more efficiently.
- Scale as your business needs change.

 cloud computing is a way to rent compute power and storage from someone else’s datacenter

## Summary

1. General cloud concept, what is cloud computing.
2. Shared responsibility model, customer vs cloud provider
3. Different cloud models (public, private, hybrid, multi-cloud)
4. How cloud shifts IT spend from a capital