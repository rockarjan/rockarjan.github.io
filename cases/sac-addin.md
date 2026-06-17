# SAC Excel Add-in – Blank Screen

## Problem
User login leads to blank screen (office.html).

## Root Cause
Store-installed add-in missing:
- AppDomains configuration
- Redirect permissions

## Solution
1. Delete:
   %LOCALAPPDATA%\Microsoft\Office\16.0\Wef\
2. Deploy add-in centrally via Microsoft 365

1. Clean up local user configuration
For affected users, please delete the following folder:
%LOCALAPPDATA%\Microsoft\Office\16.0\Wef\
This removes cached add-in settings that may block proper loading.

2. Deploy the SAC Excel Add-in centrally
The add-in must be deployed centrally via Microsoft 365 Admin Center and not installed manually by users.
[SAP Analytics Cloud Excel Add-in Documentation](https://eur01.safelinks.protection.outlook.com/?url=https%3A%2F%2Fhelp.sap.com%2Fdocs%2FSAP_ANALYTICS_CLOUD_OFFICE%2F2b73edbc8f8f4189a36bc7a2e038185c%2Fdb2f874261824d63adb3ca198f65ce55.html&data=05%7C02%7Cjan.rockar%40semperitgroup.com%7C5e989535905344de031a08decc406a0f%7C47f440790021417780c968531941e357%7C0%7C0%7C639172774230328257%7CUnknown%7CTWFpbGZsb3d8eyJFbXB0eU1hcGkiOnRydWUsIlYiOiIwLjAuMDAwMCIsIlAiOiJXaW4zMiIsIkFOIjoiTWFpbCIsIldUIjoyfQ%3D%3D%7C0%7C%7C%7C&sdata=02pajbkojyfVB%2FPHU4Vs098EJje0dQrbHEu3zCKP4v0%3D&reserved=0)



## Business Impact
Blocked Liquidity Planning testing.

## SAP Reference
Note 3603475

---

../index.md
`
