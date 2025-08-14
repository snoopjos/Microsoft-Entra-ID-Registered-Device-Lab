# Microsoft-Entra-ID-Registered-Device-Lab
Showcasing how to join a clients personal device to Entra ID registered

## Scenario
You are an Azure Administrator at an MSP.
A new contractor joins an SMB client. They will use their personal Windows 11 laptop to access company Microsoft 365 resources (SharePoint, Teams, Outlook).
The client wants:

The personal device registered in Entra ID (not joined).

Conditional Access so that only registered devices can access certain company resources.

### Step 1 - Prepare the Environment
- Confirm Entra ID Premium P1/P2 is active in your lab tenant (required for Conditional Access).

### Step 2 - Create the Test User
- In Entra ID → Users, create a test user.
- Assign an appropriate Microsoft 365 license (E3/E5 or Business Premium for lab purposes).