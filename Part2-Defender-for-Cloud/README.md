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

Improve the Microsoft Defender for Cloud secure score by applying recommended remediations

Configure plans and agents for Microsoft Defender for Servers

Configure and manage Microsoft Defender for DevOps

Configure and manage Microsoft Defender External Attack Surface Management (EASM)

## Configure environment settings in Microsoft Defender for Cloud
Plan and configure Microsoft Defender for Cloud settings, including selecting target subscriptions and workspaces

Configure Microsoft Defender for Cloud roles

Assess and recommend cloud workload protection

Enable plans for Microsoft Defender for Cloud

Configure automated onboarding of Azure resources

Connect compute resources by using Azure Arc

Connect multi-cloud resources by using Environment settings

## Respond to alerts and incidents in Microsoft Defender for Cloud
Set up email notifications

Create and manage alert suppression rules

Design and configure workflow automation in Microsoft Defender for Cloud

Remediate alerts and incidents by using Microsoft Defender for Cloud recommendations

Manage security alerts and incidents

Analyze Microsoft Defender for Cloud threat intelligence reports
