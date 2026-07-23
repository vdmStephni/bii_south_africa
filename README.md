# Workflow for producing a segment-based BII land use and land use intensity layer for South Africa

**Date:** 23 July 2026  
**Repository organised by:** S. van der Merwe

## Summary

This workflow produces a segment-based land use and land use intensity layer for calculating a South African Biodiversity Intactness Index (BII). The workflow:

1. creates a national segmentation layer;
2. reclassifies the South African National Land Cover data into broad BII land-use and intensity classes;
3. allocates one dominant BII land-use class to each segment using proportional cover and a sequential decision tree; and
4. assigns a land-use intensity score from 0 to 1 to each segment.

Available biome-specific data can subsequently be used to refine intensity scores for untransformed segments. This has initially been tested in the Thicket biome.


## Output

The intended national output is a two-band raster:

1. `bii_land_use`: dominant BII land-use class per segment.
2. `bii_land_use_intensity`: land-use intensity scaled from 0 to 1 per segment.

## Render the website

Open the project in RStudio or a terminal and run:

```bash
quarto preview
```
