# FIAtools Brand Guidelines

## Overview

FIAtools is a Python ecosystem for forest inventory analysis. The brand identity reflects professionalism, scientific rigor, and the natural domain of forestry research while maintaining modern, technical appeal.

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

**Don't:**
- Oversell or use marketing hyperbole
- Assume users know FIA database structure
- Skip over statistical methodology details
- Use jargon without explanation

### Example Copy

✓ "pyFIA calculates post-stratified estimates following Bechtold & Patterson (2005), producing results statistically compatible with EVALIDator."

✗ "pyFIA is the ultimate solution for all your forest data needs!"

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
  
  <sub>Part of the **FIAtools** ecosystem</sub>
</div>
```

### Documentation Site

- Sidebar navigation with tool colors
- Code blocks with syntax highlighting
- Collapsible sections for detailed methodology

### Conference Poster

- Large tree ring visualization as focal point
- Four-column layout for tool overview
- QR code to GitHub/documentation

### Slide Deck

- Title slide: Full ecosystem logo, subtitle
- Section dividers: Tool color backgrounds
- Content slides: Minimal, code-focused

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

## Contact

For brand questions or asset requests:

**Chris Mihiar**  
chris.mihiar@usda.gov  
github.com/mihiarc
