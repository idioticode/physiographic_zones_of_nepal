# Physiographic Zones of Nepal - GIS Shapefiles Repository

Welcome to the repository dedicated to providing GIS shapefiles for the **physiographic zones of Nepal**. This repository serves as a comprehensive and easy-to-access resource for researchers, GIS analysts, and developers interested in Nepal's geography. The data provided here can be easily incorporated into various spatial analysis and mapping projects.

## About the Repository

This repository contains shapefiles representing the five distinct **physiographic zones of Nepal**, which divide the country into different geological and topographical regions:

- **High Mountain**: Includes the highest regions of the country, home to the Himalayas and Mount Everest.
- **Middle Mountain**: The central mountain belt, characterized by rugged terrain and significant climatic diversity.
- **Hill**: A diverse zone of hilly landscapes, typically located between the Terai and the Middle Mountain.
- **Siwalik**: The outermost foothills of the Himalayas, marked by lower elevations and rolling terrain.
- **Terai**: The lowland plains region of Nepal, home to the majority of the population and significant agricultural land.

## Shapefile Versions

The repository includes two distinct sets of shapefiles based on different versions of Nepal's geographical delineations:

1. **Older Map of Nepal**:  
   Based on the geographical boundaries before May 20, 2020. This version includes the territories of Nepal as per the previous official delineations.

2. **Updated Map of Nepal**:  
   This updated version incorporates new territories (Kalapani, Limpiyadhura, and Lipulekh) that Nepal officially reclaimed on May 20, 2020, thereby increasing the country’s total area to **147,516 square kilometers**.
   
## GeoJSON Files

For convenience, the **physiographic region boundaries of Nepal** have been provided in **GeoJSON format**, which allows for seamless integration into various GIS and data science environments. The GeoJSON format is ideal for use in **R**, **Python**, and other spatial analysis platforms, and can be easily imported without any need for unzipping or other preprocessing.

You can directly access the polygon boundaries of the regions using the following raw URLs:

- **Old version** (archival):  
  [https://raw.githubusercontent.com/idioticode/physiographic_zones_of_nepal/main/geojson_files/physiography_nepal_old.geojson](https://raw.githubusercontent.com/idioticode/physiographic_zones_of_nepal/main/geojson_files/physiography_nepal_old.geojson)

- **Updated version** (recommended):  
  [https://raw.githubusercontent.com/idioticode/physiographic_zones_of_nepal/main/geojson_files/physiography_nepal_updated.geojson](https://raw.githubusercontent.com/idioticode/physiographic_zones_of_nepal/main/geojson_files/physiography_nepal_updated.geojson)

These **GeoJSON files** are compatible with popular spatial libraries such as:

- `sf` (Simple Features) in **R**
- `geopandas` in **Python**

This compatibility ensures that users can easily manipulate, visualize, and analyze the data in their preferred software environment.

Feel free to use these files in your mapping projects, overlay analyses, or any geospatial workflows that involve the physiographic zoning of Nepal.

## Usage

To use these shapefiles, simply download the appropriate files directly from this repository. These files can be loaded into GIS applications such as **QGIS**, **ArcGIS**, or programming languages like **R** and **Python** for spatial analysis, visualization, and further research.

Example usage in **R**:
```r
library(sf)
shapefile_url <- "https://raw.githubusercontent.com/idioticode/physiographic_zones_of_nepal/main/geojson_files/physiography_nepal_updated.geojson"
physio_data <- st_read(shapefile_url)
plot(physio_data)
```

Example usage in **Python**
```
import geopandas as gpd
url = "https://raw.githubusercontent.com/idioticode/physiographic_zones_of_nepal/main/geojson_files/physiography_nepal_updated.geojson"
gdf = gpd.read_file(url)
gdf.plot()
```
