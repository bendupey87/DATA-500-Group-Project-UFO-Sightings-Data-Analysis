# DATA 501 Final Project - UFO Sightings Analysis

## Project Overview
This project analyzes UFO sighting data from 1995-2014 to answer three key research questions about temporal patterns, internet reporting effects, and population density correlations.

## Directory Structure

```
final_code_and_data/
├── README.md                           # This file
├── data/                              # All required data files
│   ├── scrubbed.csv                   # Main UFO sightings dataset (NUFORC via Kaggle)
│   ├── ntia-analyze-table.csv         # Internet adoption data (NTIA)
│   └── apportionment.csv              # US population data (Census)
│
└── jupyter_notebooks/                 # Executable Jupyter notebooks
    └── data_501_final_project.ipynb   # Main analysis notebook
```

## How to Run

### Prerequisites
- Python 3.7+
- Jupyter Notebook or JupyterLab
- Required Python packages:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - plotly
  - scipy
  - statsmodels
  - holidays
  - scikit-learn

### Installation
```bash
# Install required packages
pip install pandas numpy matplotlib seaborn plotly scipy statsmodels holidays scikit-learn
```

### Running the Analysis
1. Navigate to the `jupyter_notebooks` directory
2. Launch Jupyter:
   ```bash
   cd jupyter_notebooks
   jupyter notebook data_501_final_project.ipynb
   ```
3. Run all cells in order (Cell → Run All)

**IMPORTANT**: The notebook uses relative paths (`../data/filename.csv`) to access data files. Make sure you run it from within the `jupyter_notebooks` directory.

## Project Structure for Submission

This entire `final_code_and_data` folder is ready to be zipped and submitted. The notebook will run completely self-contained within this directory structure.

To submit:
1. Zip the entire `final_code_and_data` folder
2. Submit the zip file

## Analyses Included

### Part 1: Temporal Analysis
- When do people report UFO sightings?
- Seasonal, weekly, and hourly patterns
- Long-term trends (1995-2014)
- Statistical modeling of temporal patterns
- Holiday effects

### Part 2: Internet Effect Analysis  
- Is the rise in reports a reporting artifact?
- Correlation between internet adoption and UFO reports
- Statistical significance testing
- Time series comparison

### Part 3: Population Density Analysis
- How does population correlate with sightings?
- Geographic distribution patterns
- State-level analysis
- Per capita considerations

## Key Findings

1. **Temporal Patterns**: Sightings peak in summer months, on weekends, and at 9-10 PM - all driven by human leisure time and visibility

2. **Internet Effect**: Internet adoption explains ~90% of the increase in UFO reports (r ≈ 0.95, p < 0.001) - the "boom" is largely a reporting artifact

3. **Population Density**: Sightings concentrate in populous states and urban areas - more observers naturally means more reports

## Team Members
- Ben - Temporal analysis
- Isabella - Internet reporting analysis  
- Carly - Population density analysis

## Data Sources
- **NUFORC UFO Data**: National UFO Reporting Center via Kaggle
- **Internet Data**: National Telecommunications and Information Administration (NTIA)
- **Population Data**: U.S. Census Bureau

## Notes
- All file paths in the notebook are relative and will work when run from the `jupyter_notebooks` directory
- Visualizations include both static (matplotlib/seaborn) and interactive (plotly) charts
- The notebook is designed to run from start to finish without manual intervention
- Runtime: Approximately 2-5 minutes depending on system performance

## Contact
For questions about this analysis, please contact the project team through the course portal.

---

**Last Updated**: December 2025
