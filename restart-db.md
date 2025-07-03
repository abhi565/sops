# 🔁 Restart Database Procedure

**Last Updated:** 2025-07-03  
**Owner:** DBA Team  
**Purpose:** To safely restart the database service to resolve performance or availability issues.

---

## ✅ Pre-checks

1. Inform stakeholders of downtime.
2. Ensure no active critical transactions (`check with application team`).
3. Check current DB status:

```bash
systemctl status db2inst1
