# Contributing to Awesome Launch List

Thank you for your interest in contributing! This guide will help you add new directories, guest post sites, or other marketing resources to the list.

## 🎯 What We're Looking For

### Ideal Submissions:
- ✅ **Free platforms** (preferred) or freemium with free tier
- ✅ **Active and maintained** - regularly updated, responsive
- ✅ **High quality** - Domain Rating 30+ preferred
- ✅ **Legitimate** - No spam, link farms, or low-quality sites
- ✅ **Verified** - You've used it or can confirm it works

### We Don't Accept:
- ❌ Spam sites or link farms
- ❌ Dead/inactive platforms (404 errors, abandoned)
- ❌ Paid-only services (unless exceptional value)
- ❌ Very low quality sites (DR < 20, poor content)
- ❌ Duplicate entries

---

## 📝 How to Contribute

### Option 1: GitHub Issue (Easiest)

1. Go to [Issues](https://github.com/ah8571/awesome-launch-list/issues)
2. Click **"New Issue"**
3. Use the template below:

```markdown
**Resource Name:** [Name]
**URL:** [https://...]
**Category:** [SaaS Directory / Guest Post Site / Launch Platform]
**Domain Rating:** [Number or "Unknown"]
**Submission Cost:** [Free / Paid / Unknown]
**Description:** [Brief description]
**Why it's valuable:** [Why should we add it?]
**Personal experience:** [Have you used it? What was the result?]
```

We'll review and add it within 3-5 days.

---

### Option 2: Pull Request (For Developers)

1. **Fork the repository**
   ```bash
   git clone https://github.com/ah8571/awesome-launch-list.git
   cd awesome-launch-list
   ```

2. **Create a new branch**
   ```bash
   git checkout -b add-new-directory
   ```

3. **Add your entry to the appropriate JSON file**

   **For SaaS Directories** (`data/saas-directories.json`):
   ```json
   {
     "id": "unique-id-slug",
     "name": "Directory Name",
     "url": "https://example.com",
     "description": "Brief description of the directory",
     "type": ["SaaS Directory", "Launch Platform"],
     "domainRating": 50,
     "submissionType": "free",
     "followType": "dofollow",
     "listedOn": ["your-source"],
     "notes": "Any additional notes or tips"
   }
   ```

   **For Guest Post Sites** (`data/guest-posts.json`):
   ```json
   {
     "id": "unique-id-slug",
     "name": "Site Name",
     "url": "https://example.com",
     "description": "What topics they cover",
     "niche": ["Marketing", "Technology"],
     "dr": 45,
     "listedOn": ["your-source"],
     "submissionGuidelines": "Link to guidelines if available",
     "notes": "Any tips for getting accepted"
   }
   ```

4. **Validate your JSON**
   ```bash
   # Make sure JSON is valid
   python3 -c "import json; json.load(open('data/saas-directories.json'))"
   ```

5. **Commit and push**
   ```bash
   git add data/
   git commit -m "Add [Directory Name] to SaaS directories"
   git push origin add-new-directory
   ```

6. **Create Pull Request**
   - Go to GitHub and create a PR
   - Explain what you're adding and why
   - Include any relevant stats (DR, traffic, etc.)

---

## 🔍 Data Quality Standards

### Required Fields:
- **name** - Official name of the platform
- **url** - Working URL (we'll verify)
- **description** - Clear, concise description (1-2 sentences)

### Preferred Fields:
- **domainRating** - Ahrefs DR (we can look this up if you don't have it)
- **submissionType** - free/paid/freemium
- **type** - Accurate categorization

### Optional But Helpful:
- **notes** - Tips for using the platform
- **submissionGuidelines** - Link to submission rules
- **followType** - dofollow/nofollow (for link building)

---

## ✅ Approval Process

1. **Submission received** - Via issue or PR
2. **Review** (1-3 days) - We check:
   - Site is active and working
   - Quality meets our standards
   - No duplicates exist
   - Data is accurate
3. **Verification** - We may test the submission process
4. **Approval** - Merged and credited
5. **Rejection** - We'll explain why and suggest alternatives

---

## 📊 What Happens After Approval

- ✅ Added to JSON data files
- ✅ Appears in our interactive tools
- ✅ Available via GitHub API
- ✅ Your contribution is credited in commit history
- ✅ Included in next website update

---

## 🌟 Recognition

**Top Contributors** will be recognized in:
- Our monthly updates
- Special "Contributors" section (coming soon)
- Social media shoutouts
- Thank you in README

---

## 💡 Suggestions Beyond Directories

We're also interested in:
- 📚 **Guides** - Tactical advice on using these resources
- 🔧 **Tools** - Scripts to validate data, check links, etc.
- 📊 **Data improvements** - Better categorization, missing DRs, etc.
- 🎯 **Case studies** - Real examples of successful launches

See something that could be better? Open an issue!

---

## 📧 Questions?

- **GitHub Issues:** [Create an issue](https://github.com/ah8571/awesome-launch-list/issues)
- **Email:** contact@plantingmoon.com
- **Website:** [plantingmoon.com](https://plantingmoon.com)

---

## 📄 Code of Conduct

Be respectful, constructive, and helpful. We're all here to help startups succeed.

- ✅ Provide constructive feedback
- ✅ Be patient with new contributors
- ✅ Help improve data quality
- ❌ Don't spam or promote low-quality sites
- ❌ Don't submit competitors' sites with malicious intent

---

**Thank you for helping make this resource better for everyone!** 🚀

---

*Maintained by [Planting Moon](https://plantingmoon.com) - Development & Marketing Agency*
