# AZ-104 Managing Identity

*Purpose:* To Create a windows server to create a hybrid environment for identity management lab tasks
*Requirements*
- Windows Server Promoted to DC running AD.
-- Entra Sync
- Azure Tenant with Entra syncing from on-prem AD
- Write back from EntraID to on Prem AD
### Associated Lab Tasks
[Lab 01 - Manage Microsoft Entra ID Identities](https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_01-Manage_Entra_ID_Identities.html)
### Tasks
- Install Windows Server 
- Promote to DC
- Manually Create Users using GUI
- Bulk Create Users using powershell
-- Use generative AI to create CSV with 50 user accounts split across 5 departments
-- Create/refactor Powershell script to bulk create users accounts in AD
-- Create Azure test tenant
-- Install Entra Connect and Sync on Prem Tenant to Entra
-- Configure write back from Entra to AD.

### Notes
domain name 'Pwlab'
test.user created manually using gui.


