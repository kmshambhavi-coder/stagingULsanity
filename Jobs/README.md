## Google Chro
This job will synchronize information about Chronicle SOAR Cases and Chronicle SOAR Alerts with Chronicle SIEM.
 Note: This job is only supported from Chronicle SOAR version 6.1.44 and higher.


**Run Interval In Seconds:** 3600

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String|True|Default Environment|
|API Root|String|True|https://backstory.googleapis.com|
|User's Service Account|Password|False|*****|
|Workload Identity Email|Password|False|*****|
|Max Hours Backwards|String|False|24|
|Verify SSL|Boolean|False|true|

## Google Chronicle Alerts Creator Job
This job will sync new SOAR alerts with Chronicle SIEM.
Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.


**Run Interval In Seconds:** 60

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String|True|Default Environment|
|API Root|String|True|https://staging-chronicle.sandbox.googleapis.com/v1alpha/projects/spsstg-ym2k3/locations/us/instances/1e9b8a5b-af1a-43ee-ae4a-72efc1475f42|
|User's Service Account|Password|False|*****|
|Workload Identity Email|Password|False|*****|
|Verify SSL|Boolean|False|true|

## Google Chronicle Sync Job
This job will synchronize information about Chronicle SOAR Cases and Chronicle SOAR Alerts with Chronicle SIEM.
 Note: This job is only supported from Chronicle SOAR version 6.1.44 and higher.


**Run Interval In Seconds:** 60

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String|True|Default Environment|
|API Root|String|True|https://staging-chronicle.sandbox.googleapis.com/v1alpha/projects/spsstg-ym2k3/locations/us/instances/1e9b8a5b-af1a-43ee-ae4a-72efc1475f42|
|User's Service Account|Password|False|*****|
|Workload Identity Email|Password|False|*****|
|Max Hours Backwards|String|False|24|
|Verify SSL|Boolean|False|true|

## stageupjob
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** 600

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|True|Default Environment|
|Api Root|String|False|https://api-gcptesting.xdr.us.paloaltonetworks.com|
|Api Key|Password|True|*****|
|Api Key ID|String|True|56|
|Max Hours Backwards|Integer|True|24|
|User Mapping JSON|String|False|{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean|False|true|

