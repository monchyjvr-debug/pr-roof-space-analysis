# Puerto Rico Roof Space Analysis

Analysis of residential and building roof suitability for solar installations across all municipalities of Puerto Rico using the NREL PV Rooftop Database (PVRDB-PR).

## Project Overview

This project evaluates available roof space for solar photovoltaic systems in Puerto Rico. It identifies buildings with insufficient suitable roof area and provides summaries and interactive maps at the municipality level.

The analysis helps understand where roof space constraints may limit solar adoption across the island.

## Data Source

- **NREL PV Rooftop Database for Puerto Rico (PVRDB-PR)**  
  Lidar-derived dataset of suitable roof surfaces (developable planes) for nearly all buildings in Puerto Rico.  
  [Official dataset page](https://data.openei.org/submissions/2862)

## Key Features

- Extraction and aggregation of roof area data by building and municipality
- Classification of buildings based on minimum suitable roof area (configurable in ft²)
- Summary statistics by municipality (quantity and percentage of buildings with insufficient roof space)
- Interactive Choropleth maps
- Heatmaps
- Export of results to CSV and HTML

## Project Structure
pr-roof-space-analysis/
├── notebooks/
│   └── 01_roof_space_analysis.ipynb
├── data/
│   └── (summary CSV files)
├── outputs/
│   ├── PR_Roof_Space_Choropleth_Quantity.html
│   ├── PR_Roof_Space_HeatMap_Quantity.html
│   └── maps/
├── requirements.txt
├── README.md
└── .gitignore

## Requirements

- Python 3.9+
- Libraries listed in `requirements.txt`

Install dependencies:

```bash
pip install -r requirements.txt

How to Run

Clone the repository:Bash
git clone https://github.com/YOUR_USERNAME/pr-roof-space-analysis.git
cd pr-roof-space-analysis

Install the required packages:Bash
pip install -r requirements.txt


Run the cells in order. You can adjust the minimum roof area threshold (in square feet) in the configuration cell.
jupyter notebook notebooks/01_roof_space_analysis.ipynb

Configuration
MIN_AREA_FT2 = 215   # Adjust this value as needed

License
This project is released under the MIT License.
Acknowledgments

National Renewable Energy Laboratory (NREL) for the PV Rooftop Database for Puerto Rico
OpenStreetMap and related building footprint sources used in the original dataset
Tableau Project link https://public.tableau.com/views/NumberofPuertoRicoBuildingswithlessthan150squarefeetofrooftop/Hoja1?:language=es-ES&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

