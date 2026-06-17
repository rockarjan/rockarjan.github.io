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

## Business Impact
Blocked Liquidity Planning testing.

## SAP Reference
Note 3603475

---

../index.md
`
