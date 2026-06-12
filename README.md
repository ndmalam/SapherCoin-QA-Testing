<div align="center">

# 🔍 SapherCoin — Manual QA Testing Report

### A complete, professional bug report for a live blockchain crypto wallet application

[![Total Bugs](https://img.shields.io/badge/Total%20Bugs%20Found-43-blue?style=for-the-badge&logo=bugsnag)](https://github.com)
[![Critical](https://img.shields.io/badge/Critical-4-red?style=for-the-badge)](https://github.com)
[![High](https://img.shields.io/badge/High-7-orange?style=for-the-badge)](https://github.com)
[![Medium](https://img.shields.io/badge/Medium-20-yellow?style=for-the-badge)](https://github.com)
[![Low](https://img.shields.io/badge/Low-12-brightgreen?style=for-the-badge)](https://github.com)
[![Status](https://img.shields.io/badge/Status-FAILED%20%E2%9D%8C-red?style=for-the-badge)](https://github.com)
[![Testing Type](https://img.shields.io/badge/Testing-Manual%20%7C%20Functional-blueviolet?style=for-the-badge)](https://github.com)

---

**Tester:** Nadeem &nbsp;|&nbsp; **Test Period:** 29 May – 07 Jun 2026 &nbsp;|&nbsp; **Location:** Remote, India

</div>

---

## 📌 Project Overview

| Field | Details |
|---|---|
| **Project** | SapherCoin.com — Blockchain Crypto Wallet |
| **Company** | Sapher AllHeart Pvt Ltd |
| **Application URL** | https://app.saphercoin.com |
| **Explorer URL** | https://explorer.sapherchain.com |
| **Testing Type** | Manual Functional, Security, Session, API, UI/UX, Network |
| **Platforms Tested** | Web (Chrome, Firefox, Edge), Android (Chrome Mobile, Firefox Mobile) |
| **OS Tested** | Windows 11, Android 16 |
| **Final Status** | ❌ FAILED — Critical security and financial integrity issues identified |

---

## 🗂️ What Is in This Repository

```
SapherCoin-QA-Testing/
│
├── 📄 README.md                          ← You are here
├── 📊 SapherCoin_Bug_Report_Final.xlsx   ← Full bug report (download to view)
└── 📁 screenshots/                       ← Screenshots for all 43 bugs
    ├── BUG-001.png
    ├── BUG-002.png
    └── ... (BUG-001 to BUG-043)
```

---

## 📊 Bug Summary

### By Severity

| Severity | Count | % | Description |
|:---:|:---:|:---:|---|
| 🔴 **Critical** | 4 | 9% | Financial & auth security — must fix before go-live |
| 🟠 **High** | 7 | 16% | Major functional and security issues |
| 🟡 **Medium** | 20 | 47% | Incorrect output, validation, UX issues |
| 🟢 **Low** | 12 | 28% | UI inconsistencies and cosmetic issues |
| **Total** | **43** | 100% | |

### By Module

| Module | Bugs | Notes |
|---|:---:|---|
| Sign Up | 6 | Input validation and UI issues |
| Sign In | 9 | OTP, session, and authentication security |
| Sign In – Magic Link | 3 | ⚠️ All 3 are Critical security vulnerabilities |
| Session Management | 1 | Logout does not terminate all active sessions |
| Reset Password | 2 | Spaces-only password accepted — account lockout risk |
| Wallet Dashboard | 3 | Toast notification and navigation issues |
| **Coin Transfer** | **11** | **Highest bug count — core feature impacted** |
| Transaction History / Search | 3 | Hash copy and search validation issues |
| Blockchain Explorer | 5 | Error handling and display accuracy issues |

---

## 🚨 Critical Bugs Found

These 4 bugs have direct financial or security impact and must be fixed before the application can go live.

| Bug ID | Module | Issue | Impact |
|---|---|---|---|
| BUG-011 | Sign In (Magic Link) | Magic link can be reused unlimited times | Unauthorized wallet access if link is intercepted |
| BUG-012 | Sign In (Magic Link) | Expired magic link still authenticates user | Permanent unauthorized access vector via email |
| BUG-013 | Sign In (Magic Link) | Same magic link works across all browsers simultaneously | 3 active wallet sessions from one link |
| BUG-033 | Coin Transfer | Wallet balance mismatch after successful transfer | Financial discrepancy — money unaccounted for |

---

## ✅ Testing Coverage

| Area Tested | Status |
|---|:---:|
| Account Creation & Email Verification | ✅ Tested |
| Login — Email, Phone OTP, Magic Link | ✅ Tested |
| Session Management & Logout | ✅ Tested |
| Password Reset Flow | ✅ Tested |
| Wallet Dashboard & Address Display | ✅ Tested |
| Coin Transfer — Happy Path | ✅ Tested |
| Coin Transfer — Boundary & Negative Cases | ✅ Tested |
| Transaction History & Hash Verification | ✅ Tested |
| Blockchain Explorer Lookup | ✅ Tested |
| Network Interruption During Transfer | ✅ Tested |
| Browser Console / API Error Monitoring | ✅ Tested |
| Cross-browser Testing | ✅ Tested |
| Mobile Responsive Testing | ✅ Tested |

---

## 🧰 Skills Demonstrated

```
Manual Testing          Exploratory Testing     Functional Testing
Regression Testing      Security Testing        Session Management Testing
API Testing (Postman)   Blockchain Testing      Mobile Testing
Cross-browser Testing   Bug Reporting           Test Case Design
SQL Queries             Network Testing         UI/UX Validation
```

**Tools Used:** Postman · Git · Browser DevTools · Chrome · Firefox · Edge · Android

**Domain Knowledge:** Blockchain · Crypto Wallets · Transaction Hashes · Blockchain Explorer · Web3

---

## 📋 Bug Report Format

Each of the 43 bugs is documented with the following fields:

| Column | Description |
|---|---|
| Bug ID | Unique ID (BUG-001 to BUG-043) |
| Module / Page | App section where bug was found |
| Page URL | Exact URL of the bug |
| Bug Title | One-line description of the issue |
| Severity | Critical / High / Medium / Low |
| Priority | High / Medium / Low |
| Steps to Reproduce | Numbered steps to reproduce from scratch |
| Expected Result | What should happen |
| Actual Result | What actually happens |
| Device / Browser | Testing environment |
| Account Used | Which test account |
| Wallet Address | Blockchain wallet involved (if applicable) |
| Transaction Hash | TxHash for transfer-related bugs |
| Screenshot / Video | Evidence file reference |
| Status | Open / Fixed / Retest / Closed |
| Comments | Technical context and fix direction |

---

## 🔗 How to View the Report

1. Click **`SapherCoin_Bug_Report_Final.xlsx`** above
2. Click the **Download** button (raw file)
3. Open with Microsoft Excel or Google Sheets
4. The file has 3 sheets: **Bug Report** · **Test Summary** · **Legend & Guide**

---

## 👤 About the Tester

**Nadeem** — Manual QA Tester based in Patna, Bihar, India

Focused on functional and exploratory testing of web and mobile applications with special interest in fintech and blockchain applications. Currently building automation testing skills alongside active manual testing work.

📧 [nalam140@gmail.com](mailto:nalam140@gmail.com)  
🔗 [https://www.linkedin.com/in/nalam140](https://www.linkedin.com/in/nalam140)  
🌐 Available for remote work globally

---

## 📁 Other Projects

| Project | Type | Bugs Found | Link |
|---|---|---|---|
| SapherCoin Wallet | Blockchain / Fintech | 43 | This repo |
| *(Next project)* | *(Add here)* | — | — |

---

<div align="center">

*This report was prepared as part of a professional QA testing assignment.*  
*All testing was conducted on a test environment with test accounts and test coins only.*

</div>
