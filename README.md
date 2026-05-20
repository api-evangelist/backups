# Backups (backups)
An index and topic collection covering backup, disaster recovery, and data protection APIs. Backup APIs enable applications and platforms to schedule, orchestrate, and verify the copying of data from production systems to durable storage targets, manage retention and immutability policies, and recover workloads after incidents ranging from accidental deletion to ransomware. This collection spans enterprise backup platforms like Veeam, Commvault, Rubrik, and Cohesity, SaaS data backup providers like Rewind, OwnBackup, Spanning, and Backupify, endpoint and cloud backup services like Acronis, Druva, and Carbonite, cloud-native backup services from AWS, Azure, and Google Cloud, open-source tools like Restic, BorgBackup, and Duplicati, and storage targets used as backup destinations such as Backblaze B2 and Wasabi.

**URL:** [https://apievangelist.com](https://apievangelist.com)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Backup, Disaster Recovery, Data Protection, Snapshot, Archive

## Timestamps

- **Created:** 2026-05-19
- **Modified:** 2026-05-19

## Common Properties

- [Portal](https://apievangelist.com)
- [GitHubOrganization](https://github.com/api-evangelist)
- [JSONSchema - Backup Job Schema](https://raw.githubusercontent.com/api-evangelist/backups/refs/heads/main/json-schema/backups-backup-job-schema.json)
- [JSONSchema - Recovery Point Schema](https://raw.githubusercontent.com/api-evangelist/backups/refs/heads/main/json-schema/backups-recovery-point-schema.json)
- [JSON-LD](https://raw.githubusercontent.com/api-evangelist/backups/refs/heads/main/json-ld/backups-context.jsonld)
- [Vocabulary](https://raw.githubusercontent.com/api-evangelist/backups/refs/heads/main/vocabulary/backups-vocabulary.yaml)

## Features

| Name | Description |
|------|-------------|
| Backup Job Orchestration | Backup APIs schedule, trigger, and monitor backup jobs across servers, virtual machines, databases, SaaS tenants, and endpoints, with policy-driven recurrence and dependency management. |
| Recovery Point Management | APIs enumerate and inspect recovery points (snapshots, restore points, incremental chains) so that operators and automation can pick the right point in time for granular or full recovery. |
| Retention and Lifecycle Policies | Backup platforms expose retention rules, GFS (grandfather-father-son) schedules, and lifecycle transitions that move data between hot, cold, and archive tiers like S3 Glacier or Azure Archive. |
| Immutability and Ransomware Protection | Modern backup APIs configure object lock, WORM storage, air-gapped copies, and anomaly detection to defend recovery data against ransomware and insider tampering. |
| SaaS Data Backup | SaaS-focused providers like Rewind, OwnBackup, Spanning, and Backupify back up Salesforce, Microsoft 365, Google Workspace, GitHub, Shopify, and other tenant data through vendor APIs. |
| Disaster Recovery Orchestration | DR APIs from AWS, Azure, VMware, and Veeam coordinate failover, failback, runbook execution, and recovery validation across primary and secondary sites or cloud regions. |
| Cross-Cloud and Hybrid Targets | Backup APIs write to a mix of on-prem appliances, object storage (Backblaze B2, Wasabi, S3, Azure Blob), and cloud-native services, enabling 3-2-1 strategies across providers. |

## Use Cases

| Name | Description |
|------|-------------|
| Ransomware Recovery | Organizations use backup APIs to identify the most recent clean recovery point after a ransomware event and orchestrate restore of affected VMs, files, and databases at scale. |
| SaaS Tenant Protection | SMBs and enterprises run SaaS backup APIs to protect Microsoft 365 mailboxes, SharePoint sites, Google Workspace drives, and Salesforce records against accidental deletion and malicious actors. |
| Cross-Region Disaster Recovery | Operators use APIs like AWS Backup, Azure Site Recovery, and Veeam to replicate workloads across regions and execute scheduled DR drills with measurable RPO and RTO. |
| Long-Term Archival and Compliance | Regulated industries push immutable backup copies to archive tiers (S3 Glacier, Azure Archive, B2) via backup APIs to satisfy retention mandates under HIPAA, SOX, GDPR, and FINRA. |
| Endpoint and Remote Worker Backup | Endpoint backup APIs from Druva, Acronis, and Carbonite protect laptops and remote devices and let IT centrally restore files after device loss or compromise. |
| Database and VM Snapshot Automation | Platform engineers script database, VM, and volume snapshots via cloud-native APIs (Amazon DLM, Azure Backup, NetApp) and integrate them into CI/CD and pre-change checkpoints. |

## Integrations

| Name | Description |
|------|-------------|
| Veeam | Backup, replication, and disaster recovery platform for VMs, physical servers, cloud workloads, and Microsoft 365 with a comprehensive REST API. |
| Commvault | Enterprise data protection and backup platform with REST APIs for jobs, clients, storage policies, and disaster recovery orchestration. |
| Rubrik | Cloud data management and backup platform with REST APIs covering SLA domains, snapshots, recovery, and ransomware investigation. |
| Cohesity | Hyperconverged data protection and backup platform with REST APIs for protection jobs, sources, views, and recovery operations. |
| AWS Backup | Centralized, policy-based AWS service that automates backup of EBS, RDS, DynamoDB, EFS, S3, and other AWS resources via API and IaC. |
| Microsoft Azure Backup | Azure-native backup service that protects VMs, files, SQL, and SAP HANA workloads, with REST APIs for vaults, policies, and recovery points. |
| Druva | SaaS-delivered data protection for endpoints, data centers, and cloud workloads with APIs for backups, restores, and compliance reporting. |
| Backblaze B2 | Low-cost cloud object storage commonly used as a backup target via S3-compatible APIs, supporting object lock and lifecycle rules. |

## Artifacts

Machine-readable API specifications organized by format.

### JSON Schema

- [Backup Job Schema](json-schema/backups-backup-job-schema.json)
- [Recovery Point Schema](json-schema/backups-recovery-point-schema.json)

### JSON Structure

- [Backup Job Structure](json-structure/backups-backup-job-structure.json)
- [Recovery Point Structure](json-structure/backups-recovery-point-structure.json)

### JSON-LD

- [Backups Context](json-ld/backups-context.jsonld)

## Vocabulary

- [Backups Vocabulary](vocabulary/backups-vocabulary.yaml) — Unified taxonomy mapping resources, actions, workflows, and personas across enterprise, SaaS, cloud, and open-source backup and disaster recovery platforms

## Network

This index references the following backup and data protection provider repositories:

- [Acronis](https://github.com/api-evangelist/acronis)
- [AWS Backup](https://github.com/api-evangelist/aws-backup)
- [Amazon S3 Glacier](https://github.com/api-evangelist/amazon-s3-glacier)
- [Backblaze](https://github.com/api-evangelist/backblaze)
- [Backupify](https://github.com/api-evangelist/backupify)
- [CloudAlly](https://github.com/api-evangelist/cloudally)
- [Cohesity](https://github.com/api-evangelist/cohesity)
- [Commvault](https://github.com/api-evangelist/commvault)
- [Druva](https://github.com/api-evangelist/druva)
- [Keepit](https://github.com/api-evangelist/keepit)
- [Microsoft Azure Backup](https://github.com/api-evangelist/microsoft-azure-backup)
- [Microsoft Azure Site Recovery](https://github.com/api-evangelist/microsoft-azure-site-recovery)
- [NetApp](https://github.com/api-evangelist/netapp)
- [OwnBackup](https://github.com/api-evangelist/ownbackup)
- [Spanning](https://github.com/api-evangelist/spanning)
- [Spin.AI](https://github.com/api-evangelist/spin-ai)
- [Veritas NetBackup](https://github.com/api-evangelist/veritas-netbackup)
- [VMware](https://github.com/api-evangelist/vmware)
- [Veeam](https://github.com/api-evangelist/veeam)
- [Rubrik](https://github.com/api-evangelist/rubrik)
- [HYCU](https://github.com/api-evangelist/hycu)
- [Rewind](https://github.com/api-evangelist/rewind)
- [Wasabi](https://github.com/api-evangelist/wasabi)
- [Restic](https://github.com/api-evangelist/restic)
- [BorgBackup](https://github.com/api-evangelist/borgbackup)
- [Duplicati](https://github.com/api-evangelist/duplicati)
- [Carbonite](https://github.com/api-evangelist/carbonite)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
