# SAC Excel Add-in – Blank Screen

## Problem
User login leads to blank screen (office.html).

## Solution
### 1. Clean up local user configuration
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


# SAP Analytics Cloud (SAC) Excel Add-in – Blank Screen

A troubleshooting guide for resolving the issue where the SAP Analytics Cloud add-in for Microsoft Excel displays a blank screen (`office.html`) during user login.

## 🔴 Problem
When a user attempts to log in via the SAC Excel Add-in, the authentication process fails, and a blank screen (`office.html`) is displayed instead of the login prompt or dashboard.

---

## 🛠️ Solution

### 1. Clean up local user configuration
Cached add-in settings can become corrupted and block proper loading. For affected users, please clear the local Cache folder:

1. Close Microsoft Excel.
2. Delete the following folder:
   %LOCALAPPDATA%\Microsoft\Office\16.0\Wef\

3. Restart Excel and try logging in again.

### 2. Deploy the SAC Excel Add-in centrally
To prevent this issue from reoccurring, the add-in should be managed at the tenant level.

> [!IMPORTANT]
> The add-in **must be deployed centrally via the Microsoft 365 Admin Center** and should not be installed manually by individual users.

For official documentation on central deployment, see:
🔗 [SAP Help Portal: Login leads to blank screen](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD_OFFICE/2b73edbc8f8f4189a36bc7a2e038185c/db2f874261824d63adb3ca198f65ce55.html)

---

## 📖 SAP References
For more detailed technical background, refer to the following SAP Notes (SAP Support Portal credentials required):

* **[SAP Note 3603475](https://me.sap.com/notes/3603475/E)** – *SAP Analytics Cloud, add-in for Microsoft Excel – Login leads to blank screen*
* **[SAP Note 3192210](https://me.sap.com/notes/3192210)** – *Logon to SAC does not work and a blank page is opened in browser when using SAC add-in in Excel desktop*
