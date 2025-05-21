# Travel Reservations App

This project is a dashboard to draw some insights regarding infineon products. It is built using Pandas library while using Postgres to retrieve data from a infineon_product_data.csv. The dashboard is deployed on a web application using streamlit.


## Features

- View available hotel rooms.
- Make a reservation.
- Cancel a reservation.
- View all reservations.

## Technologies Used

- **Backend**: Flask (Python)
- **Frontend**: VueJS (loaded via CDN), Tailwind CSS (via CDN)
- **Data Storage**: Local JSON files

## Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.x
- pip3 (Python package installer)

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

## Usage

- The homepage displays available hotel rooms.
- Use the reservation form to book a room.
- View and manage reservations through the "Reservations" page.


**Example `infineon_product_data.csv` structure:**

```csv
product_id,product_name,product_category,industry,unit_cost (€),units_produced,region,production_date,units_sold
P1001,AURIX™ TC3xx MCU,Processor,Healthcare,5.50,137,South America,2025-05-10,120
P1002,CoolMOS™ C7,Memory Chip,Automotive,3.20,58,Middle East,2025-05-12,45
P1003,XENSIV™ TLI4971 Current Sensor,Sensor,Consumer Electronics,2.75,142,Africa,2025-05-15,130
P1004,OPTIGA™ TPM Security Chip,Security IC,IoT,4.10,95,Asia-Pacific,2025-05-18,80
```