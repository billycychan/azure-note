# Describe cost management in Azure

## Describe factors that can affect costs in Azure

Azure from CapEx to OpEx

- Resource type
    - blob, a performance tier, an access tier, redundancy settings, and a region
- Consumption
    - pay-as-you-go
    - reserve capacity (certain amount of Azure resources commitment, 1/3 years)
- Maintenance
    - Using resource group to keep resources organized
    - maintain your cloud environment to control costs
- Geography
    - With this global deployment comes global pricing differences.
    - cost of power, labor, taxes and fees vary depending on the location
    - inter region/ inter-continental data transfer, between Availability Zone
- Subscription type
    - usage allowances, which affect costs.
- Azure MarketPlace
    - lets you purchase **Azure-based solutions and services** from third-party vendors
    - you may pay for not only the Azure services that you’re using, but also **the services or expertise of the third-party vendor**

## Compare the Pricing and Total Cost of Ownership calculators

- Pricing Calculator
    - is designed to give you an estimated cost for provisioning resources in Azure
- Total Cost Ownership Caluculator
    - is designed to help you **compare the costs for running an on-premises infrastructure** compared to an **Azure Cloud infrastructure**

## Describe the Microsoft Cost Management Tool

If you accidentally provision new resources, you may not be aware of them until it’s time for your invoice. Cost Management is a service that helps avoid those situations.

- **Cost Alert**
    - **Budget Alert**
        - notify you when spending, based on usage or cost, reaches or exceeds the amount defined in the alert condition of the budget.
        - **Azure portal** or the **Azure Consumption API.**
    - **Credit Alerts**
        - Credit alerts are generated automatically at 90% and at 100% of your Azure credit balance
    - **Department spending quota alerts**
        - Department spending quota alerts notify you when department spending **reaches a fixed threshold of the quota**. Spending quotas are configured in the EA portal

- **Budget**
    - You can set budgets based on a subscription, resource group, service type, or other criteria with alert.

## Describe the purpose of tag

Tags provide extra information, or metadata, about your resources.

- Resource management
- Cost management and optimization
- Operations management
- Security tags
- Governance and regulatory compliance
- Workload optimization and automation

You can add, modify, or delete resource tags through **Windows PowerShell, the Azure CLI, Azure Resource Manager templates, the REST API, or the Azure portal.**

Example tagging structure

| Name | Value |
| --- | --- |
| AppName | The name of the application that the resource is part of. |
| CostCenter | The internal cost center code. |
| Owner | The name of the business owner who's responsible for the resource. |
| Environment | An environment name, such as "Prod," "Dev," or "Test." |
| Impact | How important the resource is to business operations, such as "Mission-critical," "High-impact," or "Low-impact." |