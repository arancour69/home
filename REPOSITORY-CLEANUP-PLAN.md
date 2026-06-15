# 🧹 Repository Cleanup & Organization Plan

## Overview
This document outlines the strategy for cleaning up, organizing, and consolidating the 108+ repositories in the arancour69 account.

---

## Phase 1: Archive Inactive Repositories ⏳

### Step 1.1: Repositories to Archive (Low Risk)
These have not been updated since 2019-2020 and are clearly test/practice projects:

```
[ ] test                  (created: 2020, no description)
[ ] test-1                (created: 2020, no description)
[ ] hello-world           (created: 2020, GitHub tutorial)
[ ] Sample                (created: 2020, sample project)
[ ] WinZipKata            (created: 2025, practice TDD project)
[ ] yupp                  (created: 2020, fork, last push: 2019)
[ ] ZAltevi               (created: 2020, testing, last push: 2019)
[ ] xxx                   (created: 2020, fork, last push: 2015)
[ ] xxx.m3u               (created: 2020, fork, last push: 2019)
```

### Step 1.2: Repositories to Review/Consolidate (Medium Risk)
These are duplicates or related to each other:

```
Duplicates to merge:
[ ] iptv vs iptv-2                    → Keep: iptv (most active)
[ ] watchiptv vs watchiptv-1           → Keep: watchiptv
[ ] kodi-iptv-addons vs kodi-iptv-addons-1 → Consolidate into one
[ ] M3U vs M3U-1                       → Keep: m3u (primary)
[ ] listas vs listas-1                 → Consolidate
[ ] IPTV-3 vs IPTV-4 vs IPTV-5        → Review and merge active content
```

### Step 1.3: Repositories to Keep (High Value)
These are actively maintained or have unique functionality:

```
MUST KEEP:
✅ iptvnator              - Primary cross-platform player
✅ html-iptv-player       - Web-based player
✅ PlaylistEditorTV       - Windows playlist editor
✅ iptv                   - Main playlist repository
✅ iptv-pro.github.io     - Logo/EPG service
✅ kodi.addons            - Main Kodi addon repo
✅ repository.kodibae     - Kodi repository
✅ here-and-bak-again_html-epg-viewer - EPG service
```

---

## Phase 2: Add GitHub Topics 🏷️

### Topic Mapping Strategy

**Core Topics:**
```
iptv           → All IPTV-related projects
kodi           → Kodi addons and integrations
m3u            → Playlist file handling
epg            → Electronic Program Guide
streaming      → Streaming technology
media-player   → Video player apps
```

**Secondary Topics:**
```
addon          → Addon/extension projects
enigma2        → Enigma2 DVR system
windows        → Windows-specific apps
web            → Web-based tools
html           → HTML/web technologies
```

### Topic Application Plan

| Repository | Topics |
|------------|--------|
| iptvnator | #iptv #media-player #streaming |
| html-iptv-player | #iptv #media-player #web #epg |
| PlaylistEditorTV | #iptv #media-player #windows |
| iptv | #iptv #m3u #playlist |
| iptv-pro.github.io | #iptv #epg #logo |
| kodi.addons | #kodi #addon #iptv |
| repository.kodibae | #kodi #addon #iptv |
| enigma2-plugins | #enigma2 #kodi #addon |
| here-and-bak-again_html-epg-viewer | #iptv #epg #web |

---

## Phase 3: Create Consolidated Hub Repository 🎯

### New Repository: `iptv-tools-hub`

**Purpose:** Central directory and documentation for all IPTV tools

**Contents:**
```
iptv-tools-hub/
├── README.md                          # Main hub documentation
├── TOOLS-DIRECTORY.md                 # Categorized tool listings
├── SETUP-GUIDES/
│   ├── iptv-player-setup.md          # Player configuration guides
│   ├── kodi-addon-setup.md            # Kodi addon installation
│   ├── m3u-playlist-setup.md          # Playlist file handling
│   └── epg-guide-setup.md             # EPG integration guide
├── ARCHITECTURE.md                    # How tools integrate
├── CONTRIBUTING.md                    # Contributing guidelines
├── MIGRATION-GUIDE.md                 # Help for users migrating tools
└── ROADMAP.md                         # Future plans and improvements
```

---

## Phase 4: Documentation Updates 📚

### What to Update in Each Repository

1. **README.md**
   - Add reference to hub repository
   - Add "Related Projects" section
   - Add topic badges
   - Update setup instructions

2. **CONTRIBUTING.md**
   - Link to hub documentation
   - Explain relationship to other tools

3. **.github/config.yml** (if applicable)
   - Add topics programmatically
   - Add labels for issues

---

## Implementation Checklist

### Week 1: Archive Phase
- [ ] Create list of repos to archive
- [ ] Export any important data from test repos
- [ ] Set repos to archived status
- [ ] Update README on each archived repo with deprecation notice

### Week 2: Topic Phase
- [ ] Add topics to all active repositories
- [ ] Verify topic coverage
- [ ] Create GitHub saved filters for topic searches

### Week 3: Hub Creation
- [ ] Create new `iptv-tools-hub` repository
- [ ] Add hub documentation
- [ ] Link hub from each related repository
- [ ] Create inter-project reference matrix

### Week 4: Documentation
- [ ] Update all README files with hub links
- [ ] Create setup guides
- [ ] Document API/integration points
- [ ] Create contribution workflow

---

## Expected Benefits

✅ **Organization**
- Clear categorization of 100+ repos
- Easy discovery of related tools
- Reduced confusion about which tool to use

✅ **Maintenance**
- Identify duplicate efforts
- Find consolidation opportunities
- Track relationships between projects

✅ **Accessibility**
- New users can find appropriate tools quickly
- Setup guides reduce onboarding time
- Examples and documentation improve code quality

✅ **Growth**
- Clear architecture enables new contributors
- Better documentation attracts users
- Organized structure supports future expansion

---

## Risk Mitigation

| Risk | Mitigation |
|------|-----------|
| Archiving active repo by mistake | Review each repo's activity first |
| Breaking user workflows | Keep all repos accessible, just reorganized |
| Missing topic assignments | Use systematic checklist |
| Incomplete documentation | Assign clear owners per section |

---

## Timeline

```
Week 1 (Jun 15-21)   → Archival + Backup
Week 2 (Jun 22-28)   → Topics + Metadata
Week 3 (Jun 29-Jul 5) → Hub Creation
Week 4 (Jul 6-12)    → Documentation
```

---

**Approval Status:** ⏳ Awaiting confirmation

**Next Steps:**
1. Review this plan
2. Approve archival list
3. Confirm topic taxonomy
4. Begin Phase 1

---

**Document Version:** 1.0
**Last Updated:** June 15, 2026
