# 🛠️ Login Issue Troubleshooting Guide

**File:** login-issue-troubleshoot.md  
**Last Updated:** 2025-07-03  
**Owner:** Support Team  
**Purpose:** Identify and resolve user login issues across identity systems.

---

## 👀 Common Symptoms

- Invalid credentials  
- Login redirects back to the same page  
- HTTP 403/500 errors  
- SSO redirect loop  
- MFA not triggered  

---

## 🧪 Diagnostic Steps

### ➤ 1. Confirm User Status

#### Check in LDAP:
```bash
ldapsearch -x uid=<username>
