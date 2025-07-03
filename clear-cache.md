# 🧹 Clear Application Cache SOP

**File:** clear-cache.md  
**Last Updated:** 2025-07-03  
**Owner:** DevOps Team  
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
