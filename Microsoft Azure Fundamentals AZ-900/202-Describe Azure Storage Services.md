# Describe Azure Storage Services

## Describe Azure Storage Accounts

- A storage account provided a unique namespace for your Azure Storage data that’s accessible from anywhere in the world over HTTP or HTTPS.
- Data is secure, highly available, durable and massively scalable.

| Storage service | Endpoint |
| --- | --- |
| Blob Storage | https://<storage-account-name>.blob.core.windows.net |
| Data Lake Storage Gen2 | https://<storage-account-name>.dfs.core.windows.net |
| Azure Files | https://<storage-account-name>.file.core.windows.net |
| Queue Storage | https://<storage-account-name>.queue.core.windows.net |
| Table Storage | https://<storage-account-name>.table.core.windows.net |

## Describe Azure storage redundancy

- tradeoffs between lower costs and higher availability
    - How your data is replicated in the primary region
    - Whether your data is replicated to a second region that is geographically distant to the primary region, to protect against regional disasters.
    - Whether your application requires read access to the replicated data in the secondary region if the primary region becomes unavailable.

### **Locally redundant storage**

Locally redundant storage (LRS) replicates your data **three times within a single data center** in the **primary region**. LRS provides at least 11 nines of durability (99.999999999%) of objects over a given year.

- Lowest cost, least durability

### **Zone-redundant storage**

- zone-redundant storage (ZRS) replicates your **Azure Storage data synchronously** across **three Azure availability zones** in the primary region
- Microsoft recommends

### **Redundancy in a secondary region**

- Geo-redundant storage
    - It copies your data synchronously **three times within a single datacenter** in the primary region using LRS.
    - Then copied the data asyncronously to the secondary region (Region-pair)
- Geo-zone-redundant storage
    - is copied across **three Azure availability zones** in the primary region (similar to ZRS)
    - also replicated to a secondary geographic region, using LRS, for protection from regional disasters

## Describe Azure storage services

**Azure Blobs:** A massively scalable object store for text and binary data.

**Azure Files:**  Managed file shares for cloud or on-premises deployments.

**Aure Queues:** A messaging store for reliable messaging between application components.

**Azure Disks:** Block-level storage volumes for Azure VMs.

**Azure Tables:** NoSQL table option for structured, non-relational data.

Benefits:

- Durable and highly available
- Secure, access control, encrypted
- Scalable, massively scalable to meet the data storage and performance needs of today’s application
- Managed by Azure hardware maintenance
- Accessible from anywhere

### Azure Blobs

text/binary data, unstructured,  thousands of simultaneous uploads, massive amounts of video data, constantly growing log files

Blob storage is ideal for:

- Serving **images** or documents directly to a browser.
- Storing files for distributed access.
- Streaming video and audio.
- Storing data for backup and restore, disaster recovery, and archiving.
- Storing data for analysis by an on-premises or Azure-hosted service.

 HTTP or HTTPS.

The Azure Storage REST API, Azure PowerShell, Azure CLI, or an Azure Storage client library

- **Hot access tier**
- **Cool access tier**,  infrequently accessed and stored for at least 30 days
- **cold access tier,** s infrequently accessed and stored for at least 90 days.
- **archive access tier,** is rarely accessed and stored for at least 180 day

### Azure Files

- SMB/ NFS on the cloud

Benefits

- Shared access
- Fully managed
- Scripting and tooling
- Resiliency
- Familiar programmability

### Azure Queues

- Azure Queue storage is a service for storing large numbers of messages
- A queue can contain as many messages as your storage account has room for (potentially millions).
- 64KB size

## Azure Disks

block-level storage volumes managed by Azure for use with Azure VMs.

## Azure Tables

Azure Table storage stores large amounts of structured data. Azure tables are a NoSQL datastore that accepts authenticated calls from inside and outside the Azure cloud. 

## Identify Azure data migration options

- **Azure Migrate**
    - an on-premises environment to the cloud.
    - unified migration platform
    - range of tools
    - assessment and migration
- **Azure Migrate: Discovery and assessment**. Discover and assess on-premises servers running on VMware, Hyper-V, and physical servers in preparation for migration to Azure.
- **Azure Migrate: Server Migration**. Migrate VMware VMs, Hyper-V VMs, physical servers, other virtualized servers, and public cloud VMs to Azure.
- **Data Migration Assistant**. Data Migration Assistant is a stand-alone tool to assess SQL Servers. It helps pinpoint potential problems blocking migration. It identifies unsupported features, new features that can benefit you after migration, and the right path for database migration.
- **Azure Database Migration Service**. Migrate on-premises databases to Azure VMs running SQL Server, Azure SQL Database, or SQL Managed Instances.
- **Azure App Service migration assistant**. Azure App Service migration assistant is a standalone tool to assess on-premises websites for migration to Azure App Service. Use Migration Assistant to migrate .NET and PHP web apps to Azure.
- **Azure Databox**
    - a physical migration service that helps transfer large amounts of data in a quick, inexpensive, and reliable way.
    - The Data Box is transported to and from your datacenter via a regional carrier. A rugged case protects and secures the Data Box from damage during transit.
    - Usecases
        - One time migration
        - Moving a media library from offline tapes into Azure to create an online media library
        - Migrating your VM farm, SQL server, and applications to Azure.
        - Moving historical data to Azure for in-depth analysis and reporting using HDInsight
        - Initial bulk transfer - when an initial bulk transfer is done using Data Box (seed) followed by incremental transfers over the network.
        - Periodic uploads - when large amount of data is generated periodically and needs to be moved to Azure

## Identify Azure file movement options

## **AzCopy**

- CLI utility to copy blobs  / files to or from your storage account
- upload files, download files, copy files between storage accounts, and even synchronize files

## Azure Storage Explorer

- GUI to manage files and blobs in your Azure Storage Account

## Azure File Sync

- centralize your file shares in Azure Files and keep the flexibility, performance, and compatibility of a **Windows file server.**