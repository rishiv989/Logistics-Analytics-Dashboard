# Logistics Analytics Dashboard

This project is a end-to-end data analytics and engineering pipeline for logistics data. It handles raw e-commerce logistics datasets (Olist), processes them to build structured fact and dimension tables, loads the structured data into a PostgreSQL database, and prepares it for analytics dashboards.

## Project Structure

```text
├── dashboard/               # Streamlit/Dash applications (placeholder)
├── data/
│   ├── raw/                 # Raw Olist CSV datasets
│   └── processed/           # Aggregated KPIs and fact tables
├── notebooks/               # Jupyter Notebooks for execution stages
│   ├── 01_data_understanding.ipynb
│   ├── 02_build_fact_table.ipynb
│   └── 03_load_to_postgres.ipynb
├── sql/                     # SQL scripts for database schemas (placeholder)
├── src/                     # Python source files (placeholder)
├── screenshots/             # Visual dashboard documentation (placeholder)
├── requirements.txt         # Project package dependencies
└── .gitignore               # Ignored local files (venv, caches, etc.)
```

## Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/rishiv989/Logistics-Analytics-Dashboard.git
cd Logistics-Analytics-Dashboard
```

### 2. Set Up a Virtual Environment
Create and activate a virtual environment to manage dependencies locally:

**On Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

**On macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Running the Pipeline
Execute the Jupyter Notebooks in the `notebooks/` directory sequentially:
1. `01_data_understanding.ipynb` - Initial data profiling and exploration.
2. `02_build_fact_table.ipynb` - Building order fact tables and compiling state and monthly KPIs.
3. `03_load_to_postgres.ipynb` - Loading processed clean tables into a PostgreSQL database.

## Technologies Used
- **Language**: Python
- **Libraries**: Pandas, NumPy, Jupyter
- **Database**: PostgreSQL
