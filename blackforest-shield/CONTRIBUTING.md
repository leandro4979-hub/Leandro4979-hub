# Contributing to BlackForest Shield

Thank you for your interest in contributing! BlackForest Shield is a community-driven project.

---

## 🎯 Ways to Contribute

### 1. Report Issues

#### False Positives (site breaking)
- **File issue:** [GitHub Issues](https://github.com/leandro4979-hub/blackforest-shield/issues)
- **Include:**
  - Website URL
  - What's broken (ads, content, layout?)
  - Screenshot
  - Filter list version

#### Missing Domains
- **Submit with evidence:**
  - Domain name
  - What does it do? (tracker, malware, etc.)
  - Source of evidence
  - Regional relevance

### 2. Suggest Domains

Submit new domains to block:

```markdown
**Domain:** example-tracker.com
**Category:** Tracking/Profiling
**Evidence:** 
  - Link to threat report
  - Affected region: DE/CH/AT
**Impact:** Used by 50+ sites
```

---

## 📋 Contribution Guidelines

### Be Respectful
- Assume good intent
- Provide evidence for claims
- Welcome feedback gracefully

### Submission Standards

1. **Accuracy Required**
   - Provide credible evidence
   - Link to threat reports
   - Test before submitting

2. **No Broad Nukes**
   - Specific hostnames only
   - No overly broad wildcards
   - Test for false positives

3. **Documentation**
   - Comment why domain is included
   - Link to evidence

---

## 🛠️ Filter List Format

BlackForest Shield uses **ABP (Adblock Plus) syntax**:

```
! Comment (starts with !)
||domain.de^          ! Exact hostname match
||*.ad.de^            ! Wildcard match (use sparingly)
```

**Rules:**
- ✅ `||domain.de^` — Exact hostname (PREFERRED)
- ⚠️ `/regex/` — Test for catastrophe
- ❌ `||*.de^` — Too broad (breaks everything)

---

## 🔄 Pull Request Process

### Step 1: Fork & Create Branch
```bash
git clone https://github.com/YOUR-USERNAME/blackforest-shield.git
git checkout -b add-tracker-domain
```

### Step 2: Make Changes

Edit `filters.txt`:
```
! New Tracker Entry
||new-tracker.de^      ! [Category] Description
                       ! Evidence: https://threat-report.com
```

### Step 3: Submit Pull Request

**PR Template:**
```markdown
## What does this add?
Brief description.

## Why?
- Evidence/threat report
- Regional relevance
- Impact (sites affected)

## Testing
- Tested on 5 German sites: ✅
- No false positives: ✅
```

---

## ✅ Contributor Checklist

- [ ] Read this CONTRIBUTING.md
- [ ] Checked existing issues (no duplicates)
- [ ] Provided credible evidence
- [ ] Tested for breakage (on 5+ sites)
- [ ] Added comments explaining why
- [ ] Included regional relevance
- [ ] Followed filter syntax rules
- [ ] No broad/destructive wildcards

---

## 🏆 Recognition

Contributors will be:
- ✅ Listed in CHANGELOG
- ✅ Mentioned in monthly digest
- ✅ Featured on project page

---

<div align="center">

**Thank you for helping make the internet safer and faster!** 🛡️

[Start Contributing](https://github.com/leandro4979-hub/blackforest-shield/issues)

</div>

---

**Last Updated:** June 2026 | **Version:** 1.0