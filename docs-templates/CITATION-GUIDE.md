# FIAtools Citation Guide

## Citing the Ecosystem

If you use multiple FIAtools packages in your research, you may cite the ecosystem as a whole:

```bibtex
@software{fiatools2025,
  title = {FIAtools: A Python Ecosystem for Forest Inventory Applications},
  author = {Mihiar, Christopher},
  year = {2025},
  url = {https://github.com/mihiarc},
  note = {Includes pyFIA, gridFIA, pyFVS, and askFIA packages}
}
```

## Citing Individual Packages

### pyFIA

```bibtex
@software{pyfia2024,
  title = {pyFIA: A Python Library for Forest Inventory Applications},
  author = {Mihiar, Christopher},
  year = {2024},
  url = {https://github.com/mihiarc/pyfia},
  note = {High-performance Python API for USDA Forest Service FIA data}
}
```

### gridFIA

```bibtex
@software{gridfia2025,
  title = {gridFIA: Spatial Raster Analysis for USDA Forest Service BIGMAP Data},
  author = {Mihiar, Christopher},
  year = {2025},
  url = {https://github.com/mihiarc/gridfia},
  note = {Zarr-based storage and processing for forest biomass analysis}
}
```

### pyFVS

```bibtex
@software{pyfvs2025,
  title = {pyFVS: Python Implementation of the Forest Vegetation Simulator},
  author = {Mihiar, Christopher},
  year = {2025},
  url = {https://github.com/mihiarc/pyfvs},
  note = {Southern variant growth and yield simulation for pine species}
}
```

### askFIA

```bibtex
@software{askfia2025,
  title = {askFIA: Conversational AI Interface for Forest Inventory Data},
  author = {Mihiar, Christopher},
  year = {2025},
  url = {https://github.com/mihiarc/askfia},
  note = {Natural language queries for the FIAtools ecosystem}
}
```

---

## Related Citations

When using FIAtools, you should also cite the underlying data sources and methodologies:

### FIA Program

```bibtex
@techreport{bechtold2005,
  title = {The Enhanced Forest Inventory and Analysis Program—National Sampling Design and Estimation Procedures},
  author = {Bechtold, William A. and Patterson, Paul L.},
  year = {2005},
  institution = {USDA Forest Service, Southern Research Station},
  number = {SRS-GTR-80},
  url = {https://www.srs.fs.usda.gov/pubs/gtr/gtr_srs080/gtr_srs080.pdf}
}
```

### BIGMAP Data (for gridFIA)

```bibtex
@misc{fia_bigmap2018,
  title = {FIA BIGMAP Tree Species Aboveground Biomass},
  author = {{USDA Forest Service}},
  year = {2018},
  howpublished = {ImageServer},
  url = {https://di-usfsdata.img.arcgis.com/arcgis/rest/services/FIA_BIGMAP_2018_Tree_Species_Aboveground_Biomass/ImageServer},
  note = {30-meter resolution biomass estimates for 327 tree species}
}
```

### Forest Vegetation Simulator (for pyFVS)

```bibtex
@techreport{fvs_sn_variant,
  title = {The Southern (SN) Variant Overview},
  author = {{USDA Forest Service}},
  institution = {Forest Management Service Center},
  url = {https://www.fs.usda.gov/fmsc/fvs/documents/},
  note = {Essential FVS Southern Variant documentation}
}
```

---

## Example Acknowledgments Section

You may adapt this text for your publications:

> Forest inventory analyses were conducted using FIAtools (Mihiar, 2025), an open-source Python ecosystem for working with USDA Forest Service Forest Inventory and Analysis (FIA) data. Statistical estimation methods follow Bechtold and Patterson (2005). [Add specific package citations as needed based on which tools you used.]

---

## Version Information

When citing, consider noting the version used:

```bibtex
@software{pyfia2024,
  ...
  version = {0.1.0},
  ...
}
```

You can find version information in each package's `pyproject.toml` or by running:

```python
import pyfia
print(pyfia.__version__)
```
