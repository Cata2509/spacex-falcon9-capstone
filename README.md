# SpaceX Falcon 9 First-Stage Landing Prediction

Capstone project completed as part of the IBM Data Science Professional Certificate. The project studies historical Falcon 9 launches and predicts whether the first stage will land successfully.

## Project workflow

1. Collect launch data from the SpaceX REST API.
2. Extract launch records from Wikipedia through web scraping.
3. Clean and transform the collected data.
4. Explore launch outcomes with SQL and Python visualizations.
5. Analyze launch-site geography with Folium.
6. Build an interactive Plotly Dash dashboard.
7. Train, tune, and evaluate classification models.

## Repository structure

```text
notebooks/
  01_data_collection_api.ipynb
  02_web_scraping.ipynb
  03_data_wrangling.ipynb
  04_eda_sql.ipynb
  05_eda_visualization.ipynb
  06_launch_site_location_folium.ipynb
  08_machine_learning_prediction.ipynb
dashboard/
  spacex_dash_app.py
images/
  dashboard/
  folium/
```

## Main technologies

- Python, Pandas and NumPy
- Beautiful Soup and Requests
- SQLite and SQL magic
- Matplotlib, Seaborn and Plotly
- Folium
- Dash
- Scikit-learn

## Running the notebooks

Install the dependencies:

```bash
python -m pip install -r requirements.txt
```

Open JupyterLab and run the notebooks in numerical order:

```bash
jupyter lab
```

## Running the dashboard

Download the course dashboard dataset into the `dashboard` directory:

```text
https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DS0321EN-SkillsNetwork/datasets/spacex_launch_dash.csv
```

Then run:

```bash
cd dashboard
python spacex_dash_app.py
```

The dashboard provides launch-site filtering, a successful-launch pie chart, a payload-range selector, and a payload-versus-outcome scatter plot.

## Author

Catalin Niculescu

