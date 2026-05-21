## Tracking Urban Heat in Zurich
This project conducts a time series analysis of Landsat satellite data over Zurich from 1985-2024. 
## Objective
To identify changes in NDVI and Land Surface Temperature (LST) across Zurich districts. Factoring in average district income to see if urban heat island effects are distributed unequally across income levels.

## Data Sources
* **Landsat 8 LST:** Annual summer summaries (30m resolution). Time period: Triannual from 1985-2024
* **City Boundaries:** Vector neighborhood layers provided by the City of Zurich.
* **District Single Household Income** Values provided by the City of Zurich. Time period: Annually: 1999-2023
* **City Zone Polygon Data** Zoning regulations provided by the City of Zurich.
* *Note: Due to file size constraints, raw `.tif` files are not tracked in this repository. Instead use the "Landsat_Zurich.zarr" file found in the processed data folder. ".tif" files were originally downloaded from this Earth Engine script (https://code.earthengine.google.com/91d27c7125052b205c344843c20c4b1d) and were then compiled into one rioxarray dataset and saved as a .zarr file.*

## Reproducing the environment.
This project requires multiple specific geospatial packages. To recreate the environment:
1. Ensure you have Conda installed.
2. Run: `conda env create -f environment.yml`
3. Activate: `conda activate zurich-heat-env`

### Usage
1. Download the data files from the repository. Place the city polygon/vector files into a 'data/raw/' folder and the satellite raster .zarr file into 'data/processed' folder.
2. Create an 'outputs' folder for the exported maps and figures
3. Run the entire "Workflow.ipynb" notebook from top to bottom. The important and data heavy trend maps will be exported to the "outputs" folder as html or png files.
