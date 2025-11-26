# GEMINI.md

## Project Overview

This project is a data analysis exercise for a Data Analyst role at BEON TECH. The objective is to analyze airport data from Newark International Airport (EWR) to identify key metrics and improve the airport's administration. The analysis is performed in a Jupyter Notebook (`analysis.ipynb`) and uses several CSV datasets related to flights, airlines, airports, planes, and weather in the NYC area.

The main technologies used are Python with the following libraries:
*   **Data Manipulation and Analysis:** pandas, numpy, duckdb
*   **Data Visualization:** matplotlib, seaborn, plotly
*   **Dashboarding:** streamlit
*   **Jupyter Notebook:** ipykernel

The analysis aims to answer questions about:
*   Overall airport connectivity.
*   Flight delays and their correlation with weather.
*   Airline rankings by flight volume and seat availability.
*   Most common airplane manufacturers and models.

## Building and Running

### 1. Set up the Python Environment

This project uses `uv` for package management. To create the virtual environment and install the dependencies, run:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt 
```
*Note: a `requirements.txt` file was not provided, but can be generated from `pyproject.toml` using `uv pip freeze > requirements.txt` or a similar command.*

### 2. Launch the Jupyter Notebook

To explore the data analysis and see the results, run the following command to start the Jupyter Notebook server:

```bash
jupyter notebook
```

Then, open `analysis.ipynb` in your browser.

### 3. (Optional) Run the Streamlit Dashboard

The `pyproject.toml` file includes `streamlit` as a dependency, suggesting that a Streamlit dashboard might be part of the project. If a Streamlit script is created (e.g., `app.py`), it can be run with:

```bash
# TODO: Create a streamlit app.py from the notebook
streamlit run app.py
```

## Development Conventions

*   The analysis is performed in a Jupyter Notebook.
*   Data is read from CSV files.
*   The `duckdb` library is used, which suggests that some data manipulation might be performed using SQL queries on pandas DataFrames.
*   Visualization is done using `matplotlib`, `seaborn`, and `plotly`.
