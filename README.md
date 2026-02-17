# 🍄 Annual Fungi Reports

[![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=flat&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Python](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/)
[![iNaturalist](https://img.shields.io/badge/data-iNaturalist-green.svg)](https://www.inaturalist.org/)

A comprehensive data analysis and visualization project focused on fungi observations in Georgia. This repository contains Jupyter notebooks that analyze mushroom sightings collected through the iNaturalist platform, generating detailed end-of-year reports with insights into species distribution, temporal trends, and geographic hotspots.

## 📊 Overview

This project analyzes fungi observation data from Georgia to provide insights into:
- **Species diversity** and distribution patterns
- **Temporal trends** in fungal observations across months and years
- **Geographic hotspots** where fungi are most commonly observed
- **Edible and medicinal species** of particular interest to researchers and enthusiasts
- **Data quality metrics** for iNaturalist observations

## ✨ Features

- **Comprehensive Data Analysis**: Processes thousands of fungi observations with detailed taxonomic information
- **Interactive Visualizations**: 
  - Folium-based interactive maps with marker clustering
  - Time-series trend analysis showing seasonal patterns
  - Summary bar charts for quick statistics overview
  - Top species rankings and comparisons
- **Species Classification**: Identifies and categorizes 77+ edible species and 46+ medicinal species
- **Quality Assessment**: Evaluates identification agreements and positional accuracy
- **Annual Reports**: Generates detailed end-of-year summaries of fungi activity

## 📁 Repository Contents

- `Georgia EOY Fungi Reports.ipynb` - Main Jupyter notebook for analyzing Georgia fungi observations
- `README.md` - This file

## 🔬 Data Source

The analysis uses data from **[iNaturalist](https://www.inaturalist.org/)**, a citizen science platform where naturalists record and share biodiversity observations worldwide.

### Data Specifications:
- **Geographic Scope**: Georgia, USA (place_id=23)
- **Taxonomic Filter**: Iconic taxa = Fungi
- **Data Quality**: Verifiable observations only, spam filtered
- **Temporal Coverage**: Annual datasets (e.g., 2024 data with 19,092+ observations)
- **Data Fields**: 47 columns including observation dates, GPS coordinates, species identification, user information, and quality metrics

### Query Parameters:
```
quality_grade=any
identifications=any
iconic_taxa[]=Fungi
place_id=23
year=2024
verifiable=true
spam=false
```

## 🛠️ Installation & Setup

### Prerequisites

- Python 3.x
- Jupyter Notebook or JupyterLab

### Required Libraries

Install the required Python packages:

```bash
pip install numpy pandas matplotlib seaborn folium
```

Or install from a requirements file:

```bash
pip install -r requirements.txt
```

**Dependencies:**
- `numpy` - Numerical computing
- `pandas` - Data manipulation and analysis
- `matplotlib` - Static plotting
- `seaborn` - Statistical data visualization
- `folium` - Interactive maps with Leaflet.js

## 🚀 Usage

1. **Clone the repository**:
   ```bash
   git clone https://github.com/EcologicalDataAlliance/Annual-Fungi-Reports.git
   cd Annual-Fungi-Reports
   ```

2. **Prepare your data**:
   - Download fungi observation data from iNaturalist
   - Place the CSV file in a `./data/` directory
   - Update the file path in the notebook if needed

3. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook "Georgia EOY Fungi Reports.ipynb"
   ```

4. **Run the analysis**:
   - Execute cells sequentially from top to bottom
   - The notebook will generate visualizations and statistics
   - An interactive map (`fungi_observations_map 2024.html`) will be saved

## 📈 Generated Outputs

The notebook produces:

1. **Statistical Summaries**:
   - Total observation counts
   - Number of unique species identified
   - Edible and medicinal species counts
   - Data quality metrics

2. **Visualizations**:
   - Monthly trend line plots showing observation patterns
   - Bar charts comparing annual statistics (log-scale)
   - Top 10 most observed fungi species
   - Top 5 edible species rankings
   - Top 5 medicinal species rankings

3. **Interactive Maps**:
   - HTML map file with clustered markers
   - Geographic hotspots visualization
   - Regional observation density

## 🔍 Key Insights Generated

- Seasonal patterns in fungal fruiting and observation activity
- Species richness and diversity metrics
- Identification of observation hotspots for conservation planning
- Trends in citizen science participation
- Inventory of edible and medicinal species for research

## 🤝 Contributing

Contributions are welcome! Areas for enhancement:
- Additional geographic regions beyond Georgia
- Multi-year comparative analysis
- Advanced statistical modeling
- Machine learning for species prediction
- Enhanced visualization techniques
- Integration with other biodiversity databases

## 📝 License

Please check the repository for license information. Note that iNaturalist data is subject to individual observation licenses (typically CC-BY, CC-BY-NC, or CC0).

## 🙏 Acknowledgments

- **iNaturalist** community for collecting and verifying observations
- Citizen scientists who contribute fungi observations
- **Ecological Data Alliance** for maintaining this analysis project

## 📧 Contact

For questions or collaboration opportunities, please open an issue in this repository.

---

**Note**: This project is designed for educational, research, and conservation purposes. Always consult expert mycologists before consuming any wild fungi, as misidentification can be dangerous or fatal.
