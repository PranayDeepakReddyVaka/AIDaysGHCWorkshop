# Project Requirements Document (PRD) for Infineon Product Dashboard

## Goal

Build a modern, interactive dashboard for Infineon revenue data by region

## Technology Stack

**TODO**: 

- **Frontend**: Streamlit (for building the dashboard)
- **Backend**: Python (for data processing and visualization)
- **Data Visualization Libraries**: Plotly, Matplotlib, Seaborn (for creating charts and graphs)

All project dependencies must be managed using a `requirements.txt` file. We would also like to use Python's built-in `venv` module to create an isolated virtual environment for development and deployment. 

## Data

Our Infineon product data is stored in the data folder as a CSV file named `infineon_product_data.csv`. The data includes the following columns:

```
product_name, product_family, product_category, tags, applications, url, image_url, price, region, units_sold, production_date
```
An example row might look like this:

```
XENSIV™ BGT60ATR24C	XENSIV™	Sensor	XENSIV™,60GHz radar sensors for automotive	Automotive	https://www.infineon.com/cms/en/product/sensor/radar-sensors/radar-sensors-for-automotive/60ghz-radar/bgt60atr24c/	https://www.infineon.com/export/sites/default/media/products/Sensors/PG-VFWLB-76-1-web.png_11474957.png	$25.92 	South America	40	1/27/2025
```	


## Directory Structure

Most of the directory structure is already set up, but here’s a quick overview of what it should look like:

```
GithubCopilotWorkshop/
├── data/                                       # contains data related to dashboard
│   └── infineon_product_data.csv               # contains product data
├── pictures/                                   # **TODO:** Would you like to use visual input? 
│   └── dashboard_mockup_1.png                  
│   └── Colour_palette.png                      # Recommended colours (reflects company theme)
├── requirements.txt                            # Python dependencies^
├── PRD.md                                      # Project Requirements Document (PRD) for the dashboard
├── README.md                                   # Project documentation
└── streamlit_app.py                            # Source code for the dashboard and deployment

```

### Aesthetics
I would like it to be a light theme

## Acceptance Criteria
- Built in Streamlit, deployable, and responsive.
- All data is clearly formatted and visuals are user-friendly.

