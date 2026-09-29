# Greater Bay Area Marine Protected Areas (GBA MPAs)

## Project Overview
A unified, comprehensive spatial dataset for Marine Protected Areas (MPAs) spanning multiple jurisdictions in the **Greater Bay Area (GBA)** does not currently exist publicly. 

My direct involvement in this spatial mapping initiative emerged from collaborative work alongside **Dr. Andy Cornish** focusing on **Hong Kong Marine Protected Areas (HKMPAs)**. Through analyzing the localized conservation boundaries of Hong Kong's marine parks and the intend to see the connectivity of MPAs within the Greater Bay Area, I developed a strong interest in regional marine ecology management. This inspired me to independently expand the research scope and leverage **QGIS** to synthesize, model, and digitize a unified cross-border spatial database for the broader GBA maritime protection zones.

## Spatial Methodology & QGIS Analysis
* **Coordinate Reference System:** Projected using **CGCS2000 / 3-degree Gauss-Kruger CM 114E (EPSG:4574)** to guarantee zero distance distortion.

### 1. Hong Kong Marine Protected Areas (HK MPAs)
* **Data Origin:** Agriculture, Fisheries and Conservation Department (AFCD), Hong Kong SAR Government.
* **Methodology:** Due to spatial access constraints, official AFCD boundary maps and zoning charts were extracted and georeferenced as raster overlays directly within the QGIS canvas, allowing for precise manual head-up digitization of boundary polygons.

### 2. Mainland Marine Protected Areas (Non-HK MPAs)
To map the reserves across the regions, data was compiled using a multi-tiered validation approach:
* **Global Databases:** Baseline geometric boundaries for established national reserves were pulled directly from the **World Database on Protected Areas (WDPA)** via protectedplanet.net and filtered down to the Guangdong maritime administrative zone.
* **Government Documents and Proposals:** Core attributes and boundary rules—such as the 2018 Jiangmen Municipal Marine Ecosystem Protection Plan establishing the **Wuzhu Island Marine Special Protected Area**—were sourced directly from local government documents to define exact coordinate and coverage.
* **Key Academic Benchmark & Auxiliary Datasets:** Primary coordinate anchors and spatial coverage figures were cross-referenced against the supplementary datasets from the peer-reviewed paper:
  * *Reference:* **"Bohorquez, J. J., Dudgeon, C. L., Gownaris, N. J., & Pikitch, E. K. (2021). China’s little-known efforts to protect its marine ecosystems safeguard some habitats but omit others. Science Advances, 7(46), Article eabj1569. https://doi.org/10.1126/sciadv.abj1569"** 
  * *Application:* The auxiliary dataset published alongside this study was utilized as a primary spatial reference to verify, cross-check, and ground-truth the geographical coordinates and calculated coverage extents of localized marine reserves.
* **Geographic Registries:** Public spatial descriptions (e.g., the 500-meter limit) and local naming conventions were cross-referenced against **Baidu Baike (百度百科)** data streams to ensure absolute naming alignment.

---

## Interactive Spatial Boundary Map
Below is the completely interactive, zoomable web map displaying the calculated reserve polygon and its underlying attribute data table:
<iframe src="https://herao-research.github.io/Herao-Zhang/gba-mpas/index.html" 
        width="100%" 
        height="600px" 
        style="border: 2px solid #ddd; border-radius: 8px; box-shadow: 0px 4px 12px rgba(0,0,0,0.08);"
        allowfullscreen>
</iframe>

<!-- MAP WILL BE EMBEDDED DIRECTLY BELOW THIS LINE IN PHASE 3 -->

---
[🔙 Back to Projects Directory](./projects.md) | [🏠 Return to Homepage](./index.html)
