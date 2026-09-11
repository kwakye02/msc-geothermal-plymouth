# MSc Dissertation Code and Data

This repository contains the code, data and outputs used for the MSc dissertation on closed-loop geothermal potential and residential heat demand coverage in Plymouth.

## Project Structure

```text
01_Data/
  Raw/          Raw input datasets
  Processed/    Cleaned and model-ready datasets

02_Code/
  LSOA_level_method/    Heat demand and LSOA-level data preparation notebooks
  Geothermal_model/     Geology, geothermal supply, sensitivity and uncertainty notebooks

03_Outputs/
  Figures/      Final Monte Carlo and PRCC figures
  Maps/         Final QGIS map exports
  Tables/       Final appendix tables

QGIS_PROJECT/
  geothermal_project.qgz
  derived_layers/
```

## Environment

The Python environment is defined in:

```text
environment.yml
```

Create the environment with:

```bash
conda env create -f environment.yml
conda activate geothermal_plymouth
```

## Notebook Order

Run the notebooks in this order:

```text
02_Code/LSOA_level_method/01_boundaries.ipynb
02_Code/LSOA_level_method/02_energy_consumption.ipynb
02_Code/LSOA_level_method/03_epc_heating_system.ipynb
02_Code/LSOA_level_method/04_heat_demand_2024.ipynb

02_Code/Geothermal_model/01_Prepare_Digimap_Geology.ipynb
02_Code/Geothermal_model/02_Closed_Loop_Geothermal_Supply.ipynb
02_Code/Geothermal_model/03_Compare_Supply_With_Heat_Demand.ipynb
02_Code/Geothermal_model/04_Sensitivity_Analysis.ipynb
02_Code/Geothermal_model/05_Uncertainty_Analysis.ipynb
```

## Outputs

Final dissertation outputs are stored in:

```text
03_Outputs/Figures
03_Outputs/Maps
03_Outputs/Tables
```

The QGIS project is stored in:

```text
QGIS_PROJECT/geothermal_project.qgz
```
