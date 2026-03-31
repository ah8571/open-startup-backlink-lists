# 🚀 Open Startup Backlink Lists

> A curated collection of startup backlink lists for launching and growing your product. SaaS directories, guest posting sites, and related discovery platforms — all in one place.

**Maintained by [Planting Moon](https://plantingmoon.com)** - We build MVPs and execute launch strategies for startups.

[![License](https://img.shields.io/badge/license-GPL%20v3-blue.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![Last Updated](https://img.shields.io/badge/updated-March%202026-green.svg)](https://github.com/ah8571/open-startup-backlink-lists)

---

## 📊 What's Inside

| Resource Type | Count | Best For |
|--------------|-------|----------|
| 🏢 [Directories](#-directories) | 423 | B2B SaaS, Dev Tools, Product Discovery |
| ✍️ [Guest Post Sites](#-guest-post-sites) | 660 | Link Building, SEO, Content Marketing |
| 🔖 Social Bookmarks | Coming Soon | Quick Wins, Traffic Boost |

**Total Resources:** 1,083 (and growing)

---

## 🧱 Architecture

This repo has two data layers:

- **Canonical datasets** - `data/directories.json` and `data/guest-posts.json`
- **Review queue** - unverified candidates that still need duplicate checks, DR lookup, or manual review

**Source of truth:** `data/directories.json` is the canonical directories dataset. The Planting Moon website copy is generated from it and should not be treated as the primary place to edit entries.

The canonical SaaS dataset uses richer directory typing so entries can support real filtering: multiple `type` tags, DR, submission type, follow type, source attribution, and notes.

**Recommended workflow:**
1. Add new finds to the review queue first.
2. Verify duplicate status, DR, submission path, and overall quality.
3. Promote approved entries into `data/directories.json`.
4. Regenerate the Planting Moon site copy from the canonical dataset.

---

## 🎯 Interactive Tools

Don't want to browse JSON? Use our free interactive backlink tools with filtering and sorting:

- **[Directories Explorer](https://plantingmoon.com/directories)** - Filter by DR, type, cost, and export filtered lists
- **[Guest Post Sites Database](https://plantingmoon.com/guest-posts)** - Search by niche, authority
- **[All Resources Landing Page](https://plantingmoon.com/resources)** - Combined view of everything

---

## 📥 Quick Access

### For Marketers & Founders
🔗 **[Browse All Resources →](https://plantingmoon.com/resources)**  
📥 **[Open Directories Explorer →](https://plantingmoon.com/directories)**  
📥 **[Open Guest Post Database →](https://plantingmoon.com/guest-posts)**

### For Developers
```javascript
// Fetch Directories
fetch('https://raw.githubusercontent.com/ah8571/open-startup-backlink-lists/main/data/directories.json')
  .then(res => res.json())
  .then(data => console.log(data.directories));

// Fetch Guest Post Sites
fetch('https://raw.githubusercontent.com/ah8571/open-startup-backlink-lists/main/data/guest-posts.json')
  .then(res => res.json())
  .then(data => console.log(data.guestPosts));
```

---

## 🏢 SaaS Directories

423 verified platforms where you can submit your SaaS product for discovery and backlinks.

### Top 10 by Domain Rating:
1. **SourceForge** (DR: 92) - Open-source software repository
2. **TechCrunch** (DR: 92) - Tech news and product launches
3. **Product Hunt** (DR: 91) - #1 platform for launching tech products
4. **G2** (DR: 91) - B2B software reviews and comparisons
5. **Capterra** (DR: 90) - Enterprise software directory
6. **CrunchBase** (DR: 90) - Company and funding database
7. **Startup88** (DR: 88) - Startup directory
8. **FinancesOnline** (DR: 87) - Business software reviews
9. **Launched by Lovable** (DR: 87) - Product launch platform
10. **AngelList** (DR: 87) - Startup jobs and funding

**Data includes:**
- ✅ Domain Rating (DR)
- ✅ Submission cost (Free/Paid)
- ✅ Platform type
- ✅ Follow/nofollow links
- ✅ Detailed descriptions

📄 **[View Full Data](data/directories.json)** | 🌐 **[Interactive Tool](https://plantingmoon.com/saasdirectories)**

---

## ✍️ Guest Post Sites

660 high-quality blogs and publications accepting guest contributions. Perfect for building backlinks and establishing authority.

### By Niche:
- **Marketing:** 150+ sites
- **Technology:** 200+ sites
- **Business:** 180+ sites
- **Lifestyle:** 63+ sites

### By Domain Rating:
- **70+ DR:** 45 sites
- **50-70 DR:** 128 sites
- **30-50 DR:** 165 sites

**Data includes:**
- ✅ Domain Rating (DR)
- ✅ Niche categories
- ✅ Submission guidelines
- ✅ Source aggregations
- ✅ Contact information

📄 **[View Full Data](data/guest-posts.json)** | 🌐 **[Interactive Tool](https://plantingmoon.com/guest-posts)**

---

## 📝 Potential New Entries

If you find a promising source list, like a personal spreadsheet or curated post that still needs review, add those candidates to the review queue instead of pushing them straight into the live dataset.

The queue lives in `data/potential-directories.json` and is meant for:

- candidates with unknown DR
- entries that may already exist under another name
- directories that still need manual submission testing
- bulk finds from third-party lists that need cleanup first

The queue intentionally mirrors the basic directory shape used by the live dataset, so review entries can carry:

- `name`, `url`, `description`
- `type` tags for filtering and categorization
- placeholder values like `domainRating: "unknown"` or `submissionType: "unknown"`
- `listedOn`, `notes`, and `reviewStatus`

📄 **[View Review Queue](data/potential-directories.json)**

---

## 🤝 Contributing

Found a new directory or guest post site? We'd love to add it!  
See **[CONTRIBUTING.md](CONTRIBUTING.md)** for guidelines.

**What we accept:**
- ✅ Free submission opportunities (preferred)
- ✅ High-quality, active platforms
- ✅ Verified domain ratings when possible
- ✅ Detailed, accurate information

**What we don't accept:**
- ❌ Spam sites or link farms
- ❌ Dead/inactive platforms
- ❌ Sites requiring payment only (we prefer free)
- ❌ Low-quality directories (DR < 20)

---

## 📚 Guides (Coming Soon)

We're adding tactical guides to help you make the most of these resources:

- 📘 **Directory Submission Checklist** - Step-by-step process
- 📗 **Guest Posting Strategy** - Get accepted and build authority
- 📙 **Product Hunt Launch Guide** - Hit #1 Product of the Day
- 📕 **Cold Email Templates** - Outreach that gets responses

---

## 🌟 Why This Exists

We compiled this data from directory submission sources with attribution. Now we're open-sourcing it to help the startup community.

---

## 🏢 About Planting Moon

This data is maintained by **[Planting Moon](https://plantingmoon.com)**, a development and marketing agency specializing in:

- 💻 **Web & Mobile App Development**
- 🚀 **MVP Development & Product Launch**
- 📈 **SEO, PPC & Social Media Growth Strategies**

**Launching a product?** We can help with everything from development to marketing strategy.  
**[Schedule a Free Consultation →](https://plantingmoon.com/contact)**

---

## 📊 Data Quality

**Last Updated:** March 31, 2026  
**Update Frequency:** Monthly  
**Verification:** All entries manually reviewed  
**Sources:** 13+ aggregators and our own research

We occasionally add more to this list when the site makes sense or from recommendations from the community.

---

## 🔗 Links

- **Website:** [plantingmoon.com](https://plantingmoon.com)
- **Interactive Tools:** [plantingmoon.com/resources](https://plantingmoon.com/resources)
- **Contact:** [plantingmoon.com/contact](https://plantingmoon.com/contact)

---

## 📄 License

**GNU GPL v3** - Free to use, modify, and distribute under the same license.

When using this data, please credit: *"Data from [Open Startup Backlink Lists](https://github.com/ah8571/open-startup-backlink-lists) by [Planting Moon](https://plantingmoon.com)"*

---

**Last Updated:** March 31, 2026 | **Total Resources:** 1,083
