# FIAtools Branding Package

This package contains all branding assets, templates, and guidelines for the FIAtools Python ecosystem.

## Contents

```
fia-branding/
├── logos/
│   ├── fiatools-logo.svg      # Unified ecosystem logo
│   ├── pyfia-logo.svg         # pyFIA tool logo
│   ├── gridfia-logo.svg       # gridFIA tool logo
│   ├── pyfvs-logo.svg         # pyFVS tool logo
│   └── askfia-logo.svg        # askFIA tool logo
│
├── landing-page/
│   └── index.html             # Complete landing page (deploy to GitHub Pages)
│
├── marketing/
│   └── one-pager.html         # Conference/presentation one-pager (print to PDF)
│
├── docs-templates/
│   ├── README-HEADERS.md      # Copy-paste headers for each repo
│   ├── CITATION-GUIDE.md      # BibTeX citations for publications
│   └── BRAND-GUIDELINES.md    # Full brand guide
│
└── README.md                  # This file
```

## Quick Start

### 1. Update Repository READMEs

Copy the appropriate header from `docs-templates/README-HEADERS.md` to each repository.

### 2. Deploy Landing Page

The `landing-page/index.html` is a standalone file that can be:
- Deployed to GitHub Pages
- Hosted on Netlify/Vercel
- Used as a template for a documentation site

### 3. Print Marketing Materials

Open `marketing/one-pager.html` in a browser and print to PDF for conferences.

### 4. Host Logos

Consider creating a `fiatools-branding` repository to host SVG logos so they can be referenced via raw.githubusercontent.com URLs in READMEs.

## Color Quick Reference

| Tool | Primary | Light |
|------|---------|-------|
| pyFIA | `#2D5016` | `#4A7C23` |
| gridFIA | `#1B7C74` | `#2A9D8F` |
| pyFVS | `#8B6914` | `#B8860B` |
| askFIA | `#006D6D` | `#008B8B` |

## Font Stack

```css
--font-display: 'Playfair Display', Georgia, serif;
--font-body: 'IBM Plex Sans', system-ui, sans-serif;
--font-mono: 'IBM Plex Mono', 'Fira Code', monospace;
```

Google Fonts import:
```html
<link href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@400;500&family=IBM+Plex+Sans:wght@300;400;600;700&family=Playfair+Display:wght@400;600&display=swap" rel="stylesheet">
```

## Next Steps

1. **Create `fiatools-branding` repo** to host assets
2. **Update each tool's README** with new headers
3. **Deploy landing page** to fiatools.org or GitHub Pages
4. **Add CITATION.cff** files to each repository
5. **Create social media assets** (Twitter/LinkedIn cards)

## License

Branding assets are provided for use with FIAtools projects. The underlying tools are MIT licensed.
