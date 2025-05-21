# Travel Reservations App

This project is a dashboard to draw some insights regarding infineon products. It is built using Pandas library while using Postgres to retrieve data from a infineon_product_data.csv. The dashboard is deployed on a web application using streamlit.


## Contents of Dashboard

**Product-Level Visualizations**
- **Bar Chart**: Units produced vs. units sold for each product.
- **Scatter Plot**: Unit cost (€) vs. units produced for each product.
- **Pie Chart**: Distribution of product categories across all products.
- **Line Chart**: Units produced over time (based on `production_date`).

**Category-Level Visualizations**
- **Stacked Bar Chart**: Units produced by product category and region.
- **Pie Chart**: Proportion of units sold by product category.
- **Treemap**: Hierarchical view of product categories and their respective units produced.

**Region-Level Visualizations**
- **Choropleth Map**: Units produced or sold by region (if geographical data is available).
- **Pie Chart**: Product category distribution for each region.
- **Bar Chart**: Total units produced or sold by region.

**Industry-Level Visualizations**
- **Bar Chart**: Units produced by industry.
- **Pie Chart**: Distribution of industries across all products.
- **Bubble Chart**: Industry vs. units produced, with bubble size representing unit cost.

**Time-Based Visualizations**
- **Line Chart**: Units produced or sold over time (based on `production_date`).
- **Area Chart**: Cumulative units produced or sold over time.
- **Heatmap**: Production activity by date and region.

**Cost-Based Visualizations**
    - **Histogram**: Distribution of unit costs (€) across all products.
    - **Box Plot**: Unit cost (€) by product category or industry.
    - **Scatter Plot**: Unit cost (€) vs. units sold.

**Comparative Visualizations**
    - **Dual-Axis Chart**: Units produced vs. units sold for each product.
    - **Radar Chart**: Comparison of units produced, units sold, and unit cost for different product categories.
    - **Grouped Bar Chart**: Units produced and units sold for each region.


- Add filters for:
  - Product category
  - Region
  - Industry
  - Production date range
  - Unit cost range




## Technologies Used

- **Development**: Python, Postgres
- **Deployment & Interaction**: Streamlit

Before you begin, ensure you have the following installed:

- Python 3.x
- pip3 (Python package installer)
- These visualizations can be implemented using libraries like Plotly, Matplotlib, Searborn in Python

## Project Structure

```
infineon-copilot-workshop/
├── data/                                       # contains data related to dashboard
│   └── infineon_product_data.csv               # contains product data
├── images/                                     # relevant images to understand how the dashboard should look like
│   └── dashboard_mockup_1.png                  # Mockup idea on how the dashboard should look like
│   └── dashboard_mockup_2.png                  # Mockup idea on how the dashboard should look like
│   └── Colour_palette.png                      # Recommended colours (reflects company theme)
├── requirements.txt                            # Python dependencies
├── README.md                                   # Project documentation
└── streamlit_app.py                            # Source code for the dashboard and deployment
└── Changelog.md                                # Logs change history.
```

## Setup Instructions

1.  **Clone the repository**:
    ```bash
    git clone <repository-url>
    cd project-root
    ```

2.  **Set up Python Virtual Environment & Install Backend Dependencies**:
    ```bash
    # Set up Python virtual environment (recommended)
    python -m venv venv
    On Windows use `venv\Scripts\activate`

    # Install Python dependencies
    pip install -r requirements.txt

    # Add a requirements.txt file
    pip freeze > requirements.txt
    ```


3.  **Run the Application**:
    ```bash
    # Ensure your virtual environment is active
    streamlit run dashboard.py
    ```

4.  **Access the application**:
    Open your browser and navigate to `http://127.0.0.1:5000`.

## Deployment


1.  **Run the below command to run the dashboard on local host**:
    ```bash
    # Ensure your virtual environment is active
    streamlit run dashboard.py
    ```
    The backend will run on `http://127.0.0.1:5000` and automatically reload when backend Python files change.

4.  **Refresh Browser**: Refresh your browser page (`http://127.0.0.1:5000`) to see the frontend changes.

<!-- 
## Usage

If you have a web app, write how would you want the user to interact with the app:
    - UI
    - Options available for user to performa an actions

 -->


**Example `infineon_product_data.csv` structure:**

```csv
product_id,product_name,product_category,industry,unit_cost (€),units_produced,region,production_date,units_sold
P1001,AURIX™ TC3xx MCU,Processor,Healthcare,5.50,137,South America,2025-05-10,120
P1002,CoolMOS™ C7,Memory Chip,Automotive,3.20,58,Middle East,2025-05-12,45
P1003,XENSIV™ TLI4971 Current Sensor,Sensor,Consumer Electronics,2.75,142,Africa,2025-05-15,130
P1004,OPTIGA™ TPM Security Chip,Security IC,IoT,4.10,95,Asia-Pacific,2025-05-18,80
```