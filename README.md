# Microsoft-Entra-ID-Registered-Device-Lab
Showcasing how to join a clients personal device to Entra ID registered

## Scenario
You are an Azure Administrator at an MSP.
A new contractor joins an SMB client. They will use their personal Windows 11 laptop to access company Microsoft 365 resources (SharePoint, Teams, Outlook).
The client wants:

The personal device registered in Entra ID (not joined).

Conditional Access so that only registered devices can access certain company resources.

### Step 1 - Prepare the environment
- In M365 admin center, activate Microsoft Entra ID Premium P1/P2 (required for Conditional Access).

### Step 2 - Create the test user
- In Entra ID → Users, create a test user.
- Assign Microsoft Entra P2 license.

### Step 3 - Deploy a Windows VM and RDP into OS
- Windows 11 Vm created and RDP'd into OS.

### Step 4 - Register device using test user
- Connect to domain using test user UPN.
- Device showing as registered in Entra ID.

<!-- Note that its not possible to switch user account in OS when its a VM opposed to using VirtualBox -->

### Step 5 - Conditional Policy
- Policy created and activated. Allowing access only to Office 365 products.