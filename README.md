<div align="center">
  <img src="https://fiatools.org/logos/fiatools_logo.png" alt="FIAtools" width="320">
  
  <h1>FIAtools</h1>
  
  <p><strong>Python ecosystem for forest inventory applications</strong></p>
  
  <p>
    <a href="https://fiatools.org"><img src="https://img.shields.io/badge/website-fiatools.org-2D5016" alt="Website"></a>
    <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-2D5016" alt="License: MIT"></a>
  </p>
</div>

---

FIAtools is a unified Python ecosystem for working with USDA Forest Service Forest Inventory and Analysis (FIA) data. From raw survey plots to growth projections to spatial analysis—all with consistent interfaces and proper statistical methods.

## Affiliation

Developed in collaboration with USDA Forest Service Research & Development. These tools provide programmatic access to Forest Inventory and Analysis (FIA) data but are not part of the official FIA Program.

<div align="center">
  <table>
    <tr>
      <td align="center" width="25%">
        <a href="https://github.com/mihiarc/pyfia">
          <img src="https://fiatools.org/logos/pyfia_logo.png" width="80"><br>
          <strong>pyFIA</strong><br>
          <sub>Data Foundation</sub>
        </a>
      </td>
      <td align="center" width="25%">
        <a href="https://github.com/mihiarc/gridfia">
          <img src="https://fiatools.org/logos/gridfia_logo.png" width="80"><br>
          <strong>gridFIA</strong><br>
          <sub>Spatial Analysis</sub>
        </a>
      </td>
      <td align="center" width="25%">
        <a href="https://github.com/mihiarc/pyfvs">
          <img src="https://fiatools.org/logos/pyfvs_logo.png" width="80"><br>
          <strong>pyFVS</strong><br>
          <sub>Growth Modeling</sub>
        </a>
      </td>
      <td align="center" width="25%">
        <a href="https://github.com/mihiarc/askfia">
          <img src="https://fiatools.org/logos/askfia_logo.png" width="80"><br>
          <strong>askFIA</strong><br>
          <sub>AI Interface</sub>
        </a>
      </td>
    </tr>
  </table>
</div>

## The Tools

### [pyFIA](https://github.com/mihiarc/pyfia) — Data Foundation

High-performance Python API for FIA survey data. DuckDB + Polars backend delivers 10-100x faster queries than EVALIDator with exact statistical compatibility.

```python
from pyfia import FIA, biomass, tpa

with FIA("database.duckdb") as db:
    db.clip_by_state(37)  # North Carolina
    trees = tpa(db, tree_domain="STATUSCD == 1")
    carbon = biomass(db, by_species=True)
```

### [gridFIA](https://github.com/mihiarc/gridfia) — Spatial Analysis

Access BIGMAP raster data for 327 tree species at 30m resolution. Zarr-based storage for efficient spatial queries and diversity calculations.

```python
from gridfia import GridFIA

api = GridFIA()
api.download_species(state="Oregon", species_codes=["0131"])
metrics = api.calculate_metrics(calculations=["shannon_diversity"])
```

### [pyFVS](https://github.com/mihiarc/pyfvs) — Growth Modeling

Python implementation of the Forest Vegetation Simulator (Southern variant). Simulate growth and yield for loblolly, shortleaf, longleaf, and slash pine.

```python
from pyfvs import Stand

stand = Stand.initialize_planted(species="LP", trees_per_acre=500, site_index=70)
stand.grow(years=30)
```

### [askFIA](https://github.com/mihiarc/askfia) — AI Interface

Natural language queries for forest data. Ask questions in plain English and get answers powered by the entire FIAtools ecosystem.

```python
from askfia import AskFIA

fia = AskFIA()
answer = fia.ask("What's the total forest area in Maine?")
```

## How They Connect

```
┌─────────────────────────────────────────────────────────────┐
│                         askFIA                              │
│                  Natural Language Interface                 │
└─────────────────────────┬───────────────────────────────────┘
                          │
          ┌───────────────┼───────────────┐
          ▼               ▼               ▼
    ┌──────────┐    ┌──────────┐    ┌──────────┐
    │  pyFIA   │    │ gridFIA  │    │  pyFVS   │
    │  Survey  │◄──►│  Spatial │◄──►│  Growth  │
    │   Data   │    │   Data   │    │  Models  │
    └──────────┘    └──────────┘    └──────────┘
          │               │               │
          └───────────────┼───────────────┘
                          ▼
    ┌─────────────────────────────────────────────────────────┐
    │                    FIA Data Sources                     │
    │         DataMart  ·  BIGMAP API  ·  EVALIDator          │
    └─────────────────────────────────────────────────────────┘
```

## Installation

Install individual tools as needed:

```bash
pip install pyfia        # Survey data analysis
pip install gridfia      # Spatial raster analysis
pip install pyfvs        # Growth simulation
pip install askfia       # AI interface
```

Or clone this monorepo with all submodules:

```bash
git clone --recurse-submodules https://github.com/mihiarc/fiatools.git
```

## Use Cases

| Use Case | Tools | Description |
|----------|-------|-------------|
| **Carbon Accounting** | pyFIA | State/county carbon stock estimates with uncertainty |
| **Timber Supply** | pyFIA + pyFVS | Project future timber availability |
| **Biodiversity** | gridFIA | Species richness and diversity indices |
| **Site Analysis** | pyFIA + gridFIA | Combine survey and spatial data |
| **Research Queries** | askFIA | Natural language data exploration |

## By the Numbers

| Metric | Value |
|--------|-------|
| Tree species covered | 327 |
| Raster resolution | 30m |
| FIA plots integrated | 212,000+ |
| Query speedup | 10-100x |

## Documentation

- **Website:** [fiatools.org](https://fiatools.org)
- **pyFIA docs:** [mihiarc.github.io/pyfia](https://mihiarc.github.io/pyfia/)
- **Citation guide:** [docs-templates/CITATION-GUIDE.md](docs-templates/CITATION-GUIDE.md)
- **Brand guidelines:** [docs-templates/BRAND-GUIDELINES.md](docs-templates/BRAND-GUIDELINES.md)

## Repository Structure

```
fiatools/
├── pyfia/           # Survey data analysis (submodule)
├── gridfia/         # Spatial analysis (submodule)
├── pyfvs/           # Growth modeling (submodule)
├── askfia/          # AI interface (submodule)
├── logos/           # PNG logos for all tools
├── landing-page/    # fiatools.org source
├── marketing/       # Conference materials
└── docs-templates/  # README headers, citations, brand guide
```

## Citation

```bibtex
@software{fiatools2025,
  title = {FIAtools: A Python Ecosystem for Forest Inventory Applications},
  author = {Mihiar, Christopher},
  year = {2025},
  url = {https://fiatools.org}
}
```

## Contributing

Contributions welcome! Each tool has its own issue tracker:

- [pyFIA issues](https://github.com/mihiarc/pyfia/issues)
- [gridFIA issues](https://github.com/mihiarc/gridfia/issues)
- [pyFVS issues](https://github.com/mihiarc/pyfvs/issues)
- [askFIA issues](https://github.com/mihiarc/askfia/issues)

## License

MIT License — see individual repos for details.

---

<div align="center">
  <sub>Built with 🌲 by <a href="https://github.com/mihiarc">Chris Mihiar</a> · USDA Forest Service Southern Research Station</sub>
</div>
