# SAC Excel Add-in – Blank Screen

## Problem
User login leads to blank screen (office.html).

## Solution
1. Clean up local user configuration
For affected users, please delete the following folder:
%LOCALAPPDATA%\Microsoft\Office\16.0\Wef\
This removes cached add-in settings that may block proper loading.

### 2. Deploy the SAC Excel Add-in centrally
The add-in must be deployed via Microsoft 365 Admin Center  
and **must not be installed manually by users**.
[SAP Analytics Cloud, add-in for Microsoft Excel – Login leads to blank screen](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD_OFFICE/2b73edbc8f8f4189a36bc7a2e038185c/db2f874261824d63adb3ca198f65ce55.html)

## SAP Reference
[3603475 - SAP Analytics Cloud, add-in for Microsoft Excel – Login leads to blank screen)](https://me.sap.com/notes/3603475/E)  
[3192210 - Logon to SAC does not work and a blank page is opened in browser when using SAC add-in in Excel desktop](https://me.sap.com/notes/3192210)
