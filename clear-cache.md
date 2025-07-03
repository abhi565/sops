---
title: "Clear Application Cache"
file: "clear-cache.md"
last_updated: "2025-07-03"
owner: "DevOps Team"
tags: [cache, kubernetes, cloudflare, configmap, troubleshooting]
category: "Application Maintenance"
---

# 🧹 Clear Application Cache SOP

**Purpose:** Clear various cache layers to resolve stale configuration or data issues.

---

## 🧭 Scope of Caches

- Application-level in-memory cache (e.g., Spring, Redis)
- CDN (Cloudflare, Akamai)
- Browser-side cache
- Kubernetes ConfigMap/Secret based cache

---

## 🔧 Procedure

### ➤ 1. Clear Application Cache

If the app exposes a cache clear endpoint:

```bash
curl -X POST http://<app-url>/actuator/clearCache
