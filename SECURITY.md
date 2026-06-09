# 🔐 SECURITY POLICY — MISSION_RS_SDA

**Repository:** MISSION_RS_SDA — Remote Sensing & Satellite Data Analysis  
**Maintainer:** Gouragopal Mohapatra (GOURGOPAL618)  
**Last Updated:** June 2025

---

## 🛡️ Scope

This security policy applies to all code, notebooks, scripts, and configuration files
within this repository.

---

## ⚠️ Sensitive Data — Never Commit These

The following must NEVER be pushed to this repository under any circumstances:

| Type | Example | Action |
|------|---------|--------|
| GEE API credentials | `ee.Authenticate()` tokens | Store locally only |
| NASA Earthdata login | Username / password | Use `.env` file |
| Google Drive API keys | OAuth client secrets | Add to `.gitignore` |
| ESA Copernicus tokens | Access tokens | Never hardcode |
| Any personal API key | Any service | Use environment variables |

---

## 🔒 Best Practices Followed in This Repository

- ✅ No API keys or credentials hardcoded in any notebook
- ✅ All authentication done via local environment — not committed
- ✅ `.gitignore` includes `.env`, `credentials.json`, `token.json`
- ✅ GEE authentication uses `ee.Authenticate()` interactively — token stays local
- ✅ Exported GeoTIFFs with sensitive location data not pushed to repo
- ✅ All datasets used are open-source (Sentinel-2, Landsat — publicly available)

---

## 🌐 Data Sources — All Open & Licensed

| Dataset | Provider | License |
|---------|----------|---------|
| Sentinel-2 imagery | ESA Copernicus | Open — free access |
| Landsat-8 imagery | NASA / USGS | Open — public domain |
| SRTM DEM | NASA | Open — public domain |
| Odisha boundaries | Bhuvan NRSC | Open — government data |
| All training datasets | Self-generated / synthetic | Owned by author |

No proprietary or restricted datasets are used anywhere in this repository.

---

## 🚨 Reporting a Security Issue

If you find any accidentally committed credential, sensitive file, or security
vulnerability in this repository:

1. **Do NOT open a public GitHub Issue**
2. Contact directly via GitHub: [@GOURGOPAL618](https://github.com/GOURGOPAL618)
3. Describe what you found — it will be addressed within 48 hours
4. Accidental commits will be purged from git history immediately

---

## ©️ Copyright & Intellectual Property

All code, analysis, and documentation in this repository is original work by:

**Gouragopal Mohapatra**  
Independent Researcher | Odisha, India  
Protected under the **Copyright Act 1957, India**

Unauthorized reproduction, redistribution, or commercial use without explicit
written permission is prohibited.

---

## 🔄 Policy Updates

This policy will be updated as the repository grows.  
Any major change will be noted here with date.

| Version | Date | Change |
|---------|------|--------|
| v1.0 | June 2025 | Initial policy created |

---

*Maintained by JAGANNATH_CODE_SANCTUM*
