# Content Guide - Page Descriptions

This guide explains each page on the Terpsichore website and how to edit them.

## 📄 Home Page (`content/_index.md`)

**URL:** `/` (root)

**What it contains:**
- Welcome message
- Upcoming concerts (2016 schedule - update as needed)
- Recently completed concerts

**Key sections:**
- "Bienvenue" (Welcome) - Introduction
- "Prochains concerts" (Upcoming Concerts) - Current schedule
- "Derniers concerts" (Recent Concerts) - Past performances

**To edit:**
```bash
nano content/_index.md
```

**Important:** Update concert dates regularly to keep information current.

---

## 📖 About Us (`content/qui-sommes-nous.md`)

**URL:** `/qui-sommes-nous/`

**What it contains:**
- Introduction to the ensemble
- The Choir subsection
- The Conductor subsection
- Repertoire information

**Key sections:**
- Overview of Terpsichore
- Le Choeur (The Choir)
- Le Chef (The Conductor)
- Répertoire (Musical Repertoire)

**To edit:**
```bash
nano content/qui-sommes-nous.md
```

This is a comprehensive page that combines information about both the choir and conductor.

---

## 🎤 The Choir (`content/le-choeur.md`)

**URL:** `/le-choeur/`

**What it contains:**
- Choir founding and history
- Musical repertoire details
- Ensemble composition information
- Repertoire by musical period

**Key sections:**
- About the founding (1978)
- Parcours (History and performances)
- Composition (about 20 singers)
- Répertoire (detailed list by era)

**To edit:**
```bash
nano content/le-choeur.md
```

**Note:** This page is dedicated to the choir itself. Update repertoire if you add new pieces.

---

## 👨‍🎓 The Conductor (`content/le-chef.md`)

**URL:** `/le-chef/`

**What it contains:**
- Xavier Haag's biography
- Educational background
- Teaching experience
- Professional activities
- Musical specializations

**Key sections:**
- Formation (Education and training)
- Expérience Pédagogique (Teaching experience)
- Activités Professionnelles (Professional work)
- Spécialisations (Specialties - baroque music, opera)

**To edit:**
```bash
nano content/le-chef.md
```

**Note:** Update dates and titles as Xavier's career evolves.

---

## 🤝 Join Us (`content/nous-rejoindre.md`)

**URL:** `/nous-rejoindre/`

**What it contains:**
- Information about joining the choir
- Requirements and prerequisites
- What the ensemble offers
- Contact information

**Key sections:**
- À propos de nous (About the choir)
- Ce que nous proposons (What we offer)
- Conditions (Requirements)
- Nous Contacter (Contact information)

**To edit:**
```bash
nano content/nous-rejoindre.md
```

**Important:** Keep contact information current. This is how interested singers will reach you!

---

## 📝 Markdown Format Tips

All content files use **Markdown** format. Here are useful syntax tips:

### Headings
```markdown
## Main heading (H2)
### Subheading (H3)
#### Smaller heading (H4)
```

### Text Formatting
```markdown
**bold text**
*italic text*
~~strikethrough~~
```

### Lists
```markdown
- Bullet point 1
- Bullet point 2
  - Nested point

1. Numbered item 1
2. Numbered item 2
```

### Links
```markdown
[Link text](https://example.com)
[Link text](mailto:email@example.com)
```

### Code
```markdown
`inline code`

```
code block
```
```

---

## 🎯 Content Best Practices

### For Home Page
- Keep upcoming concerts updated
- Remove past concerts from "Prochains concerts"
- Move completed events to "Derniers concerts"
- Update dates in YYYY-MM-DD format for clarity

### For About Pages
- Keep biographical information accurate
- Update years and positions
- Add new achievements
- Maintain French language throughout

### For Join Us Page
- Keep email address current
- Update rehearsal information if available
- Mention any skill requirements (or lack thereof)
- Include federation membership details

### General Rules
- Always write in French
- Use proper French grammar and accents
- Keep formatting consistent
- Test changes locally before pushing:
  ```bash
  hugo server
  ```

---

## 🔍 Front Matter (Technical)

Each markdown file starts with YAML front matter:

```yaml
---
title: "Page Title"
---
```

**Important:** Always include the `title` field. This is used:
- In the browser tab
- In search results
- For page identification

---

## 📊 Page Statistics

| Page | File | URL | Length |
|------|------|-----|--------|
| Home | `_index.md` | `/` | ~400 words |
| About Us | `qui-sommes-nous.md` | `/qui-sommes-nous/` | ~800 words |
| The Choir | `le-choeur.md` | `/le-choeur/` | ~350 words |
| The Conductor | `le-chef.md` | `/le-chef/` | ~350 words |
| Join Us | `nous-rejoindre.md` | `/nous-rejoindre/` | ~250 words |

---

## ✏️ Quick Edit Commands

```bash
# Edit home page
nano content/_index.md

# Edit about us page
nano content/qui-sommes-nous.md

# Edit choir page
nano content/le-choeur.md

# Edit conductor page
nano content/le-chef.md

# Edit join us page
nano content/nous-rejoindre.md
```

---

## 🚀 After Editing

1. **Test locally:**
   ```bash
   cd /Users/gotcha/co/terpsichore-website
   hugo server
   ```
   Visit: http://localhost:1313

2. **Commit changes:**
   ```bash
   git add .
   git commit -m "Update: [describe changes]"
   git push
   ```

3. **GitHub deploys automatically** (2-5 minutes)

---

## 🆘 Common Edits

### Update Concert Dates
Edit `content/_index.md`, section "Prochains concerts"

### Change Choir Info
Edit `content/le-choeur.md` or `content/qui-sommes-nous.md`

### Update Contact Email
Edit `content/nous-rejoindre.md`, section "Nous Contacter"

### Add New Composer to Repertoire
Edit `content/le-choeur.md`, section "Répertoire"

### Update Xavier's Biography
Edit `content/le-chef.md`

---

## 📖 Format Reference

Each page should follow this structure:
1. Title (H2) - `## Title`
2. Introduction paragraph
3. Subsections (H3) - `### Subheading`
4. Content with lists where appropriate

---

## 🌐 Multilingual Note

**Current:** All pages are in French (as required)

If you need to add English translations later:
- Create separate `_index.en.md` files
- Update `hugo.toml` to add language configuration
- Consult Hugo documentation for i18n setup

For now, maintain French throughout!

---

**Remember:** After editing any file, test locally and push to deploy automatically!
