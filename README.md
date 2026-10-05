# GitSync

## Integrations
|Name|Description|
|----|-----------|
|CA Service Desk Manager|CA Service Desk Manager is designed to help IT service desk analysts make every moment count through a dynamic experience so they can deliver great customer service without the fear of overbearing processes or metrics. With the solution, teams can embrace teamwork rather than working from siloed knowledge stashes and disjointed communications.|
|CrowdStrike Falcon|CrowdStrike Falcon is the leader in next-generation endpoint protection, threat intelligence and incident response through cloud-based endpoint protection.|
|Google Chronicle|Google SecOps enables you to examine the aggregated security information for your enterprise going back for months or longer. Use Google SecOps to search across all of the domains accessed from within your enterprise. To enable the Google API client to communicate with the Backstory API you will need Google Developer Service Account Credential, https://developers.google.com/identity/protocols/OAuth2#serviceaccount.|
|Microsoft 365 Defender|Microsoft 365 Defender is a unified pre- and post-breach enterprise defense suite that natively coordinates detection, prevention, investigation, and response across endpoints, identities, email, and applications to provide integrated protection against sophisticated attacks.|
|Microsoft Graph Mail|Microsoft 365 and Office 365 deliver the power of cloud productivity to businesses of all sizes, helping save time, money, and free up valued resources. The Microsoft 365 and Office 365 plans combine the familiar Microsoft Office desktop suite with cloud-based versions of Microsoft's next-generation communications and collaboration services (including Office for the web, Microsoft Exchange Online, Microsoft Teams, and Microsoft SharePoint Online) to help users be productive from virtually anywhere through the Internet. This integration uses Microsoft Graph Mail API to communicate with Microsoft 365 and Office 365 services.|
|Palo Alto Cortex XDR|Cortex XDR - XDR is the world’s first detection and response app that natively integrates network, endpoint and cloud data to stop sophisticated attacks.  Cortex XDR accurately detects threats with behavioral analytics and reveals the root cause to speed up investigations.|


## Connectors
|Name|Description|Has Mappings|
|----|-----------|------------|
|stageupconnector|Pull information about Rule based alerts from Google Chronicle. Note: dynamic list is used for filtering purposes. For all of the details please visit the documentation portal.|True|


## Playbooks
|Name|Description|
|----|-----------|
|stageupPlaybook|test description|
|stageupblock|An embedded workflow that can receive inputs and return an output.|


## Visual Families
|Name|Description|
|----|-----------|
|stageupvisualfamilies|stageupvisualfamilies|


## Jobs
|Name|Description|
|----|-----------|
|Google Chronicle Alerts Creator Job|This job will sync new SOAR alerts with Chronicle SIEM.Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.|
|Google Chronicle Sync Job|This job will synchronize information about Chronicle SOAR Cases and Chronicle SOAR Alerts with Chronicle SIEM. Note: This job is only supported from Chronicle SOAR version 6.1.44 and higher.|
|stageupjob|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|

