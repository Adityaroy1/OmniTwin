# OmniTwin – Urban Environmental Digital Twin (prototype)

## Run
    pip install -r requirements.txt
    streamlit run app.py

Keep `app.py`, `engine.py` and `requirements.txt` in the SAME folder
(app.py does `import engine as E`). Python 3.10+ recommended.

## Files
- engine.py  – data prep, forecasting, back-test, source attribution, scenarios (no UI)
- app.py     – Streamlit UI: map, forecast/validation, attribution, scenarios, method

## Data
- No upload  -> synthetic Pune-like demo data (5 neighbourhoods, 2022-2024).
- Upload CSV -> minimum columns: Date, PM2.5, Traffic_Index, Wind_Speed (daily, >= 210 days).
  Optional: station, lat, lon, temp, humidity, rain, industrial_index.
