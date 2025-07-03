
---

### ✅ `sops/login-issue-troubleshoot.md`

```markdown
---
title: "Login Issue Troubleshooting Guide"
file: "login-issue-troubleshoot.md"
last_updated: "2025-07-03"
owner: "Support Team"
tags: [authentication, sso, login, debug, ldap, jwt]
category: "User Access & Identity"
---

# 🛠️ Login Issue Troubleshooting Guide

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
