> [!NOTE]
> Based on skills measured prior to March 4, 2024
> 
> Content currently under development

# Mitigate threats by using Defender for Cloud (15–20%)

Microsoft Defender for Cloud is a comprehensive _cloud-native application protection platform (CNAPP)_ that safeguards cloud-based applications across multicloud and hybrid environments. The platform is made up of the following key components:
- **Cloud Security Posture Management (CSPM)**: This aspect focuses on proper configuration and deployment of your cloud and on-premises resources. It identifies steps to secure your environment, ensuring that your cloud setup adheres to best practices1.
- **Cloud Workload Protection (CWP)**: Defender for Cloud provides specific protections for servers, containers, storage, databases, and other workloads. It helps shield your applications from various cyber threats and vulnerabilities1.
- **DevOps Security**: By unifying security management at the code level across multiple pipelines (including GitHub, Azure DevOps, and GitLab), Defender for Cloud empowers security teams to protect applications from code to cloud. It correlates DevOps security findings with contextual cloud security insights, allowing prioritized remediation in code1.

Link: https://portal.azure.com/#view/Microsoft_Azure_Security/SecurityMenuBlade/~/0

## Implement and maintain cloud security posture management

**Assign and manage regulatory compliance policies, including Microsoft cloud security benchmark (MCSB)**

![Policies](https://github.com/alfonso-greenbrook/SC-200-Microsoft-Security-Operations-Analyst/blob/9e213394649ff63ae4d83f6b46a5fb5423b45090/Part2-Defender-for-Cloud/Policies.png?raw=true)
- Assign security standards to specific scopes such as Azure subscriptions, AWS accounts, and GCP projects that have Defender for Cloud enabled.
- Defender for Cloud continually assesses the environment in scope against standards. Based on assessments, it shows in-scope resources as being compliant or noncompliant with the standard and provides remediation recommendations.
- Microsoft Defender for Cloud > Regulatory compliance > Manage compliance policies > _{subscription or management group}_ > Security policies
- _Microsoft Cloud Security Benchmark (MCSB)_ is a comprehensive set of best practices and recommendations designed to enhance the security of cloud resources (Azure and multi-cloud environments).

**Improve the Microsoft Defender for Cloud secure score by applying recommended remediations**

![Recommendations](https://github.com/alfonso-greenbrook/SC-200-Microsoft-Security-Operations-Analyst/blob/c9c6c2d19525a9502f5321e0c2e9632bd5a0d08f/Part2-Defender-for-Cloud/Recommendations.png?raw=true)
- Remediate security recommendations from the recommendations list. Option to remediate each recommendation manually for each resource, or use the _Fix_ option (when available) to resolve an issue on multiple resources quickly.
- There is the option to enforce or deny recommendations to improve the secure score and make sure that users don't create resources that negatively affect your score.


**Configure plans and agents for Microsoft Defender for Servers**

![DefenderforServers](https://github.com/alfonso-greenbrook/SC-200-Microsoft-Security-Operations-Analyst/blob/c9c6c2d19525a9502f5321e0c2e9632bd5a0d08f/Part2-Defender-for-Cloud/Azure_Arc.png?raw=true)
- Microsoft Defender for Servers offers two paid plans: Plan 1 (P1) and Plan 2 (P2)
- **Azure Arc** allows you to onboard Amazon Web Services (AWS), Google Cloud Platform (GCP), and on-premises machines to Azure.
- Historically, Defender for Servers used the **Log Analytics** agent and **Azure Monitor** agent to collect information from compute resources.
  - However, due to an updated strategy, these agents will be phased out by August 2024.
  - Going forward, Defender for Servers features will be provided through Microsoft Defender for Endpoint integration or agentless scanning.

**Configure and manage Microsoft Defender for DevOps**

![DefenderforDevOps](https://github.com/alfonso-greenbrook/SC-200-Microsoft-Security-Operations-Analyst/blob/c9c6c2d19525a9502f5321e0c2e9632bd5a0d08f/Part2-Defender-for-Cloud/DevOps_Security.png?raw=true)
- Secures DevOps environments; with the following capabilities:
  - Unified Visibility
  - Strengthened Cloud Resource Configuration
  - Prioritisation of critical issues in code
  - Manage DevOps environments (Azure DevOps, GitHub, and GitLab environments)
- Microsoft Defender for Cloud > Environment settings > Add environment > Azure DevOps/GitHub/GitLab
- Microsoft Defender for Cloud > DevOps security > Add environment > Azure DevOps/GitHub/GitLab

**Configure and manage Microsoft Defender External Attack Surface Management (EASM)**

![DefenderEASM](https://github.com/alfonso-greenbrook/SC-200-Microsoft-Security-Operations-Analyst/blob/c9c6c2d19525a9502f5321e0c2e9632bd5a0d08f/Part2-Defender-for-Cloud/EASM_Resource.png?raw=true)
- Continuously discovers and maps digital attack surfaces to provide an external view of your online infrastructure.
- Discovery and inventory: Domains, Hostnames, Web Pages, IP Blocks, IP Addresses, ASNs, SSL Certificates, WHOIS Contacts
- Dashboards, Managing assets, User permissions
- Microsoft Defender EASM > Create > Basics > Review + Create

## Configure environment settings in Microsoft Defender for Cloud

**Plan and configure Microsoft Defender for Cloud settings, including selecting target subscriptions and workspaces**

![TargetSubscription](https://github.com/alfonso-greenbrook/SC-200-Microsoft-Security-Operations-Analyst/blob/2703f380280cda5d08055b6b425386b9b58b8e67/Part2-Defender-for-Cloud/Target_Subscription.png?raw=true)
- Set up management groups > Enable Continuous Export > Configure data retention > Configure Defender for Cloud settings
- Microsoft Defender for Cloud > Environment settings > Subscription or workspace


**Configure Microsoft Defender for Cloud roles**

![RBACRoles](https://github.com/alfonso-greenbrook/SC-200-Microsoft-Security-Operations-Analyst/blob/c9c6c2d19525a9502f5321e0c2e9632bd5a0d08f/Part2-Defender-for-Cloud/RBAC_Roles.png?raw=true)
– Defender for Cloud workspace > Access control (IAM) tab > Add role assignment > role > user or group
- Uses Azure role-based access control (Azure RBAC) to provide built-in roles:
  - **Security Reader**: Provides read-only access to Defender for Cloud. Users with this role can view recommendations, alerts, security policies, and security states but cannot make changes.
  - **Security Admin**: Similar to the Security Reader, but with additional capabilities. Users in this role can update security policies and dismiss alerts and recommendations.
- Additional roles:
  - Contributor / Owner (Resource group level)
  - Contributor (Subscription level)
  - Owner (Subscription level)

**Assess and recommend cloud workload protection**

**Enable plans for Microsoft Defender for Cloud**

![DefenderPlans](https://github.com/alfonso-greenbrook/SC-200-Microsoft-Security-Operations-Analyst/blob/2703f380280cda5d08055b6b425386b9b58b8e67/Part2-Defender-for-Cloud/Defender_Plans.png?raw=true)

**Configure automated onboarding of Azure resources**

**Connect compute resources by using Azure Arc**

**Connect multi-cloud resources by using Environment settings**

## Respond to alerts and incidents in Microsoft Defender for Cloud
Set up email notifications

Create and manage alert suppression rules

Design and configure workflow automation in Microsoft Defender for Cloud

Remediate alerts and incidents by using Microsoft Defender for Cloud recommendations

Manage security alerts and incidents

Analyze Microsoft Defender for Cloud threat intelligence reports
