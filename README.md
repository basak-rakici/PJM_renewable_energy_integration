# Energy Systems Repository

This repository contains code and data for analyzing power system cases, running optimal power flow (OPF), computing reliability indices, and performing sensitivity analyses for different generation scenarios.

## Repository Structure

basak-rakici/

├─ data/ # Input data files (tracked via Git LFS)

├─ results/ # Output files and visualizations

├─ Base_Case.ipynb # 2023 case input generation, OPF, reliability index

├─ Sensitivity_Cases.ipynb # 2030 case, OPF, reliability index, sensitivity analysis

├─ PostProcessData.ipynb # Visualizations of generation mix, load, network, and sensitivity/congestion results

├─ requirements.txt # Python dependencies

├─ .gitattributes # Git LFS configuration


### Data

The `data/` folder contains input datasets required for running the notebooks. Notable files include:

- **[IPM Regions Shapefile](https://www.epa.gov/sites/production/files/2019-08/ipm_v6_regions.zip)** – Regions used for the analysis.  
- **[US Counties Shapefile](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html)** – County boundaries for visualization and network mapping.  
- Other input data files are stored locally in the `data/` folder and tracked via Git LFS.


## Notebooks

- **Base_Case.ipynb**  
  - Generates input files for the 2023 case  
  - Runs Optimal Power Flow (OPF)  
  - Calculates reliability indices  

- **Sensitivity_Cases.ipynb**  
  - Generates input files for the 2030 case  
  - Runs OPF and calculates reliability indices  
  - Performs sensitivity analysis for wind, solar, and offshore generation  

- **PostProcessData.ipynb**  
  - Produces visualizations for generation mix, load, and network for 2023 and 2030 cases  
  - Creates visuals for sensitivity analysis  
  - Creates visuals for congestion under changes in wind, solar, and offshore generation  

## Setup Instructions

1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/basak-rakici.git
   cd basak-rakici
   
2. Install dependencies:
  pip install -r requirements.txt

3. Make sure Git LFS is installed and pull large data files:
  git lfs install
  git lfs pull
4. Open notebooks in order:

  Base_Case.ipynb
  
  Sensitivity_Cases.ipynb
  
  PostProcessData.ipynb

## Notes

data/ contains input datasets; intermediate or large outputs can be stored in results/.

Ensure that large files are managed via Git LFS to avoid repository size issues.



