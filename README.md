# UV Exposure & Melanoma Incidence Analysis
A project to explore the relationship between long-term ultraviolet (UV) exposure and melanoma incidence across U.S. counties using public health datasets.

## How to Use
1. Clone this repository.
2. Install the required Python packages:  
   pip install -r requirements.txt
3. Open `uv-exposure-melanoma-analysis.ipynb` in Jupyter Notebook or JupyterLab.

### Research Questions
- Which U.S. states experience the highest average UV exposure over time?
- Do states with highest UV exposure also have the highest rate of reported melanoma?

## Data Sources

- The <a href="https://gis.cancer.gov/tools/uv-exposure/" target="_blank">County Level UV Exposure Data for the Continental United States </a> dataset, presented here as `uv_county` includes historical Average Daily Global Solar Radiation estimates (AVGLO) - a proxy measure for UV - in Wh/m² by county in the Continental US for the period 1961-1990 and the more recent 5-year average measures (2020 - 2024);

- <a href="https://statecancerprofiles.cancer.gov/incidencerates/index.php?stateFIPS=00&areatype=county&cancer=053&race=00&sex=0&age=001&stage=999&type=incd&sortVariableName=rate&sortOrder=default&output=0#results" target="_blank">State Cancer Profiles, from National Cancer Institute </a>data as `melanoma_county` displays
  melanoma reported cases per county in 2023.

### Insights

- States with consistently higher UV exposure tend to show higher melanoma incidence rates, however the relationship is not perfectly linear.
- States with higher UV exposure do not necessarily have the highest rates of reported melanoma.

### Future enhancements:
- Incorporate demographic normalization (age, race) through data obtained from **SEER*Stat**, a statistical software tool used to analyze cancer data from the SEER Program (Surveillance, Epidemiology, and End Results), which is maintained by the National Cancer Institute.<br>

- Integrate U.S. Census population change and migration data because since melanoma reflects cumulative exposure, future work should consider population mobility to ensure that long-term UV exposure is appropriately interpreted at the county level.

### Author

Brytner Evangelista