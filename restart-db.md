---
title: "Restart Database Procedure"
file: "restart-db.md"
last_updated: "2025-07-03"
owner: "DBA Team"
tags: [database, restart, db2, mysql, postgresql]
category: "Database Operations"
---

# 🔁 Restart Database Procedure

**Purpose:** Safely restart the database service to resolve availability or performance issues.

---

## ✅ Pre-checks

1. Inform stakeholders of the downtime window.
2. Ensure there are no active critical transactions:
   - Confirm with the application support team.
   - Optionally, run workload monitoring queries.
3. Check current DB status:

```bash
systemctl status db2inst1
