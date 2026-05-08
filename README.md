Time Series Analysis of Landsat Satellite Data over Zurich from 1985-2024. 
Analysis of changes in NDVI and Land Surface Temperature (LST) across Zurich Districts

## Project Structure

Zurich_Heat/
│
├── Notebooks/
│   └── Workflow.ipynb
│
├── data/
│   ├── raw/
│   └── processed/
│
└── outputs/

---

### Notebooks
Includes my main and only Notebook which is used for data cleaning, analysis and visualization
### 📁 data

#### raw/
- Original unmodified datasets
- Should always remain unchanged for reproducibility

#### processed/
- Cleaned and transformed datasets
- Ready for analysis or modeling

### 📤 outputs
Stores all generated artifacts:
- Charts and visualizations
- Exported datasets
- Reports and results
- Model outputs (if applicable)


### Setup
Use the Zurich_Heat.nc file to open up the datacube. Then you don't have to run the loop to open them all together. 
