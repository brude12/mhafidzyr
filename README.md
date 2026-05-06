# wildfire_GEE
Wildfire in Riau 

## Project Overview
This project automates the detection and classification of forest fire burn severity using the Delta Normalized Burn Ratio (dNBR). By leveraging the Python API for Google Earth Engine (`geemap`), this workflow processes high-resolution multitemporal Sentinel-2 Harmonized imagery without downloading heavy datasets locally.

**Study Area:** Riau, Indonesia (A region historically prone to peatland and forest fires).

## Tech Stack
*   **Language:** Python
*   **Cloud Platform:** Google Earth Engine (GEE)
*   **Libraries:** `geemap`, `earthengine-api`
*   **GIS Desktop (Validation):** QGIS

## Methodology
1.  **Data Acquisition:** Accessed Sentinel-2 Harmonized Surface Reflectance data.
2.  **Cloud Masking:** Applied automated bitmask filtering (QA60) to remove cloud and cirrus interference, ensuring high data accuracy.
3.  **Index Calculation:** Computed pre-fire and post-fire NBR using Near-Infrared (NIR) and Short-Wave Infrared (SWIR) bands.
4.  **Severity Classification:** Calculated dNBR and classified the results based on USGS standards to determine burn severity levels (Low to High).
5.  **Data Export:** Automated the export of the final raster dataset to Google Drive for local GIS ingestion.

## Results & Visualization
https://drive.google.com/file/d/1-5xecb-z57HXF6Ct32jsHDHqih3Tv5rK/view?usp=sharing

The analysis successfully isolated the High Severity burn areas, providing actionable spatial data that can be used for recovery planning and environmental monitoring.

