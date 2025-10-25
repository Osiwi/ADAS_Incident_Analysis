# ADAS / ADS Road Incident Analysis

This project analyzes reported road incidents involving:
- ADAS (Advanced Driver Assistance Systems)
- ADS (Automated Driving Systems)
- Non-ADAS/Other vehicles as a baseline

## What the notebook does
- Ingests multiple safety incident CSV files (ADAS, ADS, OTHER).
- Standardizes column names and merges sources.
- Explores patterns like:
  - frequency of incidents
  - severity distribution
  - contributing factors (e.g. environment, human error, system behavior)
- Compares ADAS vs ADS vs non-automated vehicles.
- Builds visual summaries to support safety insights.

## Data privacy
The raw incident data contains sensitive transportation safety information and is **not** included in this public repository.

To reproduce:
1. Place your own CSVs in a local `data/` folder (not tracked by git):
   - `SGO-2021-01_Incident_Reports_ADAS.csv`
   - `SGO-2021-01_Incident_Reports_ADS.csv`
   - `SGO-2021-01_Incident_Reports_OTHER.csv`
2. Use the relative paths in the notebook:
   ```python
   adas_file_path = 'data/SGO-2021-01_Incident_Reports_ADAS.csv'
   ads_file_path = 'data/SGO-2021-01_Incident_Reports_ADS.csv'
   other_file_path = 'data/SGO-2021-01_Incident_Reports_OTHER.csv'
