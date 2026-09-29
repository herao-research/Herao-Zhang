# Greater Bay Area Marine Protected Areas (GBA MPAs)

## Project Overview
This project focuses on the spatial definition, geometric reconstruction, and ecological boundary modeling of marine protected areas, marine reserves and marine parks within the Greater Bay Area. Because a unified spatial dataset for the Greater Bay Area (GBA) spanning multiple jurisdictions does not exist publicly, this database was constructed by synthesizing multi-source regional registries, legal decrees, and satellite georeferencing:

## Spatial Methodology & QGIS Analysis
* **Coordinate Reference System:** Projected using **CGCS2000 / 3-degree Gauss-Kruger CM 114E (EPSG:4574)** to guarantee zero distance distortion.

### 1. Hong Kong Marine Protected Areas (HK MPAs)
* **Data Origin:** Agriculture, Fisheries and Conservation Department (AFCD), Hong Kong SAR Government.
* **Methodology:** Due to spatial access constraints, official AFCD boundary maps and zoning charts were extracted and georeferenced as raster overlays directly within the QGIS canvas, allowing for precise manual head-up digitization of boundary polygons.

### 2. Mainland Chinese Marine Protected Areas (Non-HK MPAs)
To map the reserves across the regions, data was compiled using a multi-tiered validation approach:
* **Global Databases:** Baseline geometric boundaries for established national reserves were pulled directly from the **World Database on Protected Areas (WDPA)** via protectedplanet.net and filtered down to the Guangdong maritime administrative zone.
* **Government Decrees & Legal Texts:** Core attributes and boundary rules—such as the 2018 Jiangmen Municipal Marine Ecosystem Protection Plan establishing the **Wuzhu Island Marine Special Protected Area**—were sourced directly from local government gazettes to define exact coordinate and coverage.
* **Key Academic Benchmark & Auxiliary Datasets:** Primary coordinate anchors and spatial coverage figures were cross-referenced against the supplementary datasets from the peer-reviewed paper:
  * *Reference:* **"China’s little-known efforts to protect its marine ecosystems safeguard some habitats but omit others."** 
  * *Application:* The auxiliary dataset published alongside this study was utilized as a primary spatial reference to verify, cross-check, and ground-truth the geographical coordinates and calculated coverage extents of localized marine reserves.
* **Geographic Registries:** Public spatial descriptions (e.g., the 500-meter limit) and local naming conventions were cross-referenced against **Baidu Baike (百度百科)** data streams to ensure absolute naming alignment.

---

## Interactive Spatial Boundary Map
Below is the completely interactive, zoomable web map displaying the calculated reserve polygon and its underlying attribute data table:
<iframe src="https://herao-research.github.io/Herao-Zhang/gba-mpas.html" 
        width="100%" 
        height="600px" 
        style="border: 2px solid #ddd; border-radius: 8px; box-shadow: 0px 4px 12px rgba(0,0,0,0.08);"
        allowfullscreen>
</iframe>

<!-- MAP WILL BE EMBEDDED DIRECTLY BELOW THIS LINE IN PHASE 3 -->

---
[🔙 Back to Projects Directory](./projects.md) | [🏠 Return to Homepage](./index.html)
