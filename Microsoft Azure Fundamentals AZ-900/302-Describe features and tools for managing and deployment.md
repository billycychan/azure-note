# Describe features and tools for managing and deploying Azure resources

## Describe tools for interacting with Azure

- **Azure Portal**
    - build, manage, monitor, web interface
    - custom dashboards
    - accessibility options
- **Azure CloudShell**
    - browser based shell that allows you to create, configure, manage Azure resources using a shell
    - authenticated to your Azure credentials
    - Both supports Azure PowerShell and CLI
- **Azure Power Shell**
    - developers, DevOps, and IT professionals can run commands called command-lets (cmdlets).
    - The **routine setup, teardown, and maintenance** of a single resource or multiple connected resources.
    - The **deployment of an entire infrastructure**, which might contain **dozens or hundreds of resources, from imperative code.**
- **Azure Command Line Interface (CLI)**
    - Bash commands

## Describe the purpose of Azure Arc

on-premises resources in a hybrid configuration

the cloud resources in a multi-cloud configuration

**Secure, develop, and operate infrastructure, apps, and Azure services anywhere.**

Azure Arc 

- extends Azure compliance and monitoring to hybrid and multi-cloud environments, providing a centralized platform for managing non-Azure resources as if they were running in Azure.
- It allows users to manage **virtual machines, Kubernetes clusters, and databases** across multiple clouds and on-premises environments using familiar Azure services and management capabilities.
- By projecting existing non-Azure resources into ARM, Azure Arc simplifies governance and management, enabling a consistent multi-cloud and on-premises management experience.

## Describe Azure Resource Manager and Azure ARM templates

- Azure Resource Manager
    - Manage your infrastructure **through declarative templates** rather than scripts. A Resource Manager **template is a JSON file that defines what you want to deploy to Azure.**
    - Deploy, manage, and monitor all the resources for your solution as a group, rather than handling these resources individually
    - Re-deploy your solution **throughout the development life-cycle** and have confidence your resources are deployed in a consistent state
    - Define the dependencies between resources, so they're deployed in the correct order.
    - Apply access control to all services because RBAC is natively integrated into the management platform.
    - Apply tags to resources to logically organize all the resources in your subscription
    - Clarify your organization's billing by viewing costs for a group of resources that share the same tag.

**Infrastructure as code**

- manage your infrastructure as lines of code
- **ARM templates and Bicep** are two examples of using infrastructure as code with the **Azure Resource Manager** to maintain your environment.

### ARM templates

- By using ARM templates, you can describe the resources you want to use in a declarative JSON format
- The template then orchestrates the creation of those resources **in parallel**. That is, if you need 50 instances of the same resource, all 50 instances are created **at the same time.**

### Bicep

Bicep is a language that uses declarative syntax to deploy Azure resources. A Bicep file defines the infrastructure and configuration.

While similar to an ARM template, which is written in JSON, Bicep files tend to use a simpler, more concise style.