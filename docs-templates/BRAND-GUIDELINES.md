# FIAtools Brand Guidelines

## Overview

FIAtools is a Python ecosystem for forest inventory applications. The brand identity reflects professionalism, scientific rigor, and the natural domain of forestry research while maintaining modern, technical appeal.

---

## Naming Strategy & Rationale

### The Name "FIAtools"

**FIA** in "FIAtools" stands for **Forest Inventory Applications** — a deliberate choice to differentiate from the official USDA program.

| Term | Meaning | When to Use |
|------|---------|-------------|
| **Forest Inventory Applications** | Our ecosystem of tools | Describing FIAtools, pyFIA, etc. |
| **Forest Inventory and Analysis (FIA)** | The official USDA program | Referring to the data source or program |

### Why This Matters

The USDA Forest Service operates the **Forest Inventory and Analysis (FIA) Program** — a congressionally mandated initiative that has collected forest data since 1930. To avoid confusion:

1. **We are not the FIA Program** — We build tools that work with FIA data
2. **We are affiliated with Forest Service R&D** — The research branch that includes FIA
3. **"Applications" vs "Analysis"** — This follows the pattern established by [FIESTA](https://github.com/USDAForestService/FIESTA) (Forest Inventory **ESTimation** and Analysis), another R&D tool

### Correct Usage Examples

**Describing the tools (use "Applications"):**
- ✓ "FIAtools: Python Ecosystem for Forest Inventory Applications"
- ✓ "pyFIA: A Python Library for Forest Inventory Applications"
- ✓ "Open-source tools for forest inventory applications"

**Describing the data source (use "and Analysis"):**
- ✓ "Access Forest Inventory and Analysis (FIA) data programmatically"
- ✓ "Query the FIA database using Python"
- ✓ "Built on USDA Forest Inventory and Analysis data"

**Incorrect usage:**
- ✗ "FIAtools: Python Ecosystem for Forest Inventory Analysis" (confuses with official program)
- ✗ "The official FIA Python library" (implies official status we don't have)
- ✗ "USDA FIA Tools" (implies official USDA product)

---

## Affiliation Statement

All major documentation (READMEs, documentation sites, about pages) must include an affiliation statement:

### Standard Affiliation Block

```markdown
## Affiliation

Developed in collaboration with USDA Forest Service Research & Development.
[Tool name] provides programmatic access to Forest Inventory and Analysis (FIA)
data but is not part of the official FIA Program.
```

### Tool-Specific Variations

| Tool | Affiliation Statement |
|------|----------------------|
| **FIAtools** (ecosystem) | "These tools provide programmatic access to Forest Inventory and Analysis (FIA) data but are not part of the official FIA Program." |
| **pyFIA** | "pyFIA provides programmatic access to Forest Inventory and Analysis (FIA) data but is not part of the official FIA Program." |
| **gridFIA** | "gridFIA provides access to Forest Service spatial data products but is not part of the official FIA Program." |
| **pyFVS** | "pyFVS is a Python implementation of the Forest Vegetation Simulator and is part of the FIA Python Ecosystem." |
| **askFIA** | "askFIA provides an AI-powered interface to Forest Inventory and Analysis (FIA) data but is not part of the official FIA Program." |

---

## Taglines

### Primary Tagline
> **"Open-source Python tools for FIA data"**

### Ecosystem Tagline
> **"Python Ecosystem for Forest Inventory Applications"**

### Individual Tool Taglines

| Tool | Tagline |
|------|---------|
| **pyFIA** | "The Python API for forest inventory data" |
| **gridFIA** | "Spatial raster analysis for forest biomass" |
| **pyFVS** | "Forest growth modeling in Python" |
| **askFIA** | "Ask questions, get forest answers" |

---

## Brand Architecture

### Umbrella Brand
**FIAtools** — The unified ecosystem identity

### Sub-brands
Each tool maintains its own identity while sharing common design language:

| Tool | Color | Role | Tagline |
|------|-------|------|---------|
| **pyFIA** | Forest Green | Data foundation | "The Python API for forest inventory data" |
| **gridFIA** | Blue-Green | Spatial analysis | "Spatial raster analysis for forest biomass" |
| **pyFVS** | Amber/Gold | Growth simulation | "Forest growth modeling in Python" |
| **askFIA** | Teal | AI interface | "Ask questions, get forest answers" |

---

## Related Official Tools

For context, these are official USDA Forest Service tools that work with FIA data:

| Tool | Full Name | Source | Language |
|------|-----------|--------|----------|
| **FIESTA** | Forest Inventory ESTimation and Analysis | USDA FS R&D | R |
| **rFIA** | R package for FIA database | Academic (validated by FS) | R |
| **FVS** | Forest Vegetation Simulator | USDA FS | Fortran |
| **EVALIDator** | FIA web query tool | USDA FIA Program | Web |

FIAtools complements these by providing a Python-native ecosystem.

---

## Color Palette

### Primary Colors

```
pyFIA
├── Primary:    #2D5016 (Forest Green)
└── Light:      #4A7C23 (Leaf Green)

gridFIA
├── Primary:    #1B7C74 (Ocean Teal)
└── Light:      #2A9D8F (Seafoam)

pyFVS
├── Primary:    #8B6914 (Timber)
└── Light:      #B8860B (Gold Oak)

askFIA
├── Primary:    #006D6D (Deep Teal)
└── Light:      #008B8B (Cyan)
```

### Neutral Colors

```
Text Primary:     #1a1a1a
Text Secondary:   #4a4a4a
Text Muted:       #7a7a7a
Background:       #fafaf8
Background Alt:   #f0efe9
Card Background:  #ffffff
```

### Color Usage

- Use primary colors for headers, icons, and accent elements
- Use light variants for hover states and secondary elements
- Maintain sufficient contrast for accessibility (WCAG AA)
- The tree ring motif uses graduated opacity of each tool's primary color

---

## Typography

### Font Stack

```css
--font-display: 'Playfair Display', Georgia, serif;
--font-body: 'IBM Plex Sans', system-ui, sans-serif;
--font-mono: 'IBM Plex Mono', 'Fira Code', monospace;
```

### Usage Guidelines

| Context | Font | Weight | Size |
|---------|------|--------|------|
| Hero headlines | Playfair Display | 400 | 3-4.5rem |
| Section headers | Playfair Display | 400-600 | 2-3rem |
| Body text | IBM Plex Sans | 300-400 | 0.9-1.1rem |
| Tool names | IBM Plex Mono | 600 | 1-1.3rem |
| Code blocks | IBM Plex Mono | 400 | 0.85-0.9rem |
| Captions/labels | IBM Plex Mono | 400-500 | 0.75-0.85rem |

### Fallbacks for Print/Offline

- Display: Georgia, Times New Roman
- Body: Segoe UI, Helvetica
- Mono: Consolas, Monaco

---

## Logo System

### Tree Ring Motif

The unifying visual element across all FIAtools branding is the **tree ring** (growth ring) concept:

- Represents data layers and temporal analysis
- Connects to forest/timber domain
- Each ring can represent a different tool in the ecosystem
- Center core symbolizes the foundation (FIA data)

### Logo Variations

1. **Full ecosystem logo** — Ring segments in four colors with "FIAtools" wordmark
2. **Individual tool logos** — Single-color ring with tool-specific overlay:
   - pyFIA: Data points on rings
   - gridFIA: Grid overlay on rings
   - pyFVS: Growth curves through rings
   - askFIA: Speech bubble/question mark

### Clear Space

Maintain minimum clear space equal to the height of the "F" in FIAtools around all logos.

### Minimum Sizes

- Digital: 32px height minimum
- Print: 0.5" height minimum

---

## Voice & Tone

### Brand Personality

- **Professional** — Academic rigor without stuffiness
- **Technical** — Precise terminology, assumes domain knowledge
- **Accessible** — Clear explanations, good documentation
- **Collaborative** — Open source ethos, community-focused

### Writing Guidelines

**Do:**
- Use active voice
- Be specific about capabilities and limitations
- Include code examples
- Reference scientific methodology
- Clearly distinguish tools from data sources

**Don't:**
- Oversell or use marketing hyperbole
- Assume users know FIA database structure
- Skip over statistical methodology details
- Use jargon without explanation
- Imply official USDA endorsement

### Example Copy

✓ "pyFIA calculates post-stratified estimates following Bechtold & Patterson (2005), producing results statistically compatible with EVALIDator."

✓ "Access USDA Forest Inventory and Analysis data through a clean Python API."

✗ "pyFIA is the ultimate solution for all your forest data needs!"

✗ "The official Python library for FIA data analysis."

---

## Visual Elements

### Backgrounds

- Use subtle noise texture overlay (2-4% opacity) for depth
- Gradient meshes should use tool colors sparingly
- Prefer off-white (#fafaf8) to pure white

### Cards & Containers

- Border radius: 2-4px (subtle, not rounded)
- Shadows: Use sparingly, prefer borders
- Top accent stripe: 3-4px in tool color

### Icons & Graphics

- Prefer line-based icons over filled
- Use consistent stroke width (1.5-2px)
- Animate subtly on hover (transitions, not bounces)

### Data Visualization

- Use tool color palette for charts
- Maintain accessibility with patterns/labels, not just color
- Include uncertainty visualization where applicable

---

## Application Examples

### GitHub README Header

```markdown
<div align="center">
  <img src="logo.svg" alt="pyFIA" width="120">

  # pyFIA

  **The Python API for forest inventory data**

  [badges]

  <sub>Part of the **FIAtools** ecosystem — Python tools for Forest Inventory Applications</sub>
</div>
```

### Documentation Site

- Sidebar navigation with tool colors
- Code blocks with syntax highlighting
- Collapsible sections for detailed methodology
- Affiliation statement in footer or about page

### Conference Poster

- Large tree ring visualization as focal point
- Four-column layout for tool overview
- QR code to GitHub/documentation
- Clear affiliation statement with USDA FS R&D

### Slide Deck

- Title slide: Full ecosystem logo, subtitle
- Section dividers: Tool color backgrounds
- Content slides: Minimal, code-focused
- Closing slide: Affiliation and contact info

---

## Citation Guidelines

### Ecosystem Citation

```bibtex
@software{fiatools,
  author = {Mihiar, Chris},
  title = {FIAtools: A Python Ecosystem for Forest Inventory Applications},
  year = {2025},
  url = {https://fiatools.org}
}
```

### Individual Tool Citations

Use "Forest Inventory Applications" in tool titles:
- "pyFIA: A Python Library for Forest Inventory Applications"
- "gridFIA: Spatial Analysis for Forest Inventory Applications"

See [CITATION-GUIDE.md](./CITATION-GUIDE.md) for complete citation formats.

---

## File Formats

### Logos

Provide in:
- SVG (primary, scalable)
- PNG (transparent background, @1x and @2x)
- PDF (print-ready)

### Color Profiles

- Digital: sRGB
- Print: CMYK (provide converted values)

---

## Quick Reference Card

| Element | Correct | Incorrect |
|---------|---------|-----------|
| Ecosystem name | FIAtools | FIA Tools, FIA-tools |
| Expansion | Forest Inventory Applications | Forest Inventory Analysis |
| Data source | Forest Inventory and Analysis (FIA) | Forest Inventory Analysis |
| Tool names | pyFIA, gridFIA, pyFVS, askFIA | PyFIA, PYFIA, GridFia |
| Affiliation | "Developed in collaboration with USDA FS R&D" | "Official USDA tool" |

---

## Contact

For brand questions or asset requests:

**Chris Mihiar**
chris.mihiar@usda.gov
github.com/mihiarc
