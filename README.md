# SpaceX Launch Data Analysis

A data analysis project exploring SpaceX orbital launch operations — launch cadence, mission success rates, rocket utilization, booster reusability, landing performance, launchpad activity, and payload trends — using Python, Pandas, and Matplotlib.

## Project Objective

This project performs a comprehensive engineering-focused analysis of SpaceX's historical orbital launch records. Each chart is framed around a specific engineering question, followed by data-driven interpretation and insight, to demonstrate how raw launch data can be turned into meaningful operational conclusions.

## Dataset

- **Source:** [SpaceX Launch Data on Kaggle](https://www.kaggle.com/datasets/patelris/spacex-launches-rockets-and-starlink-dataset)
- **Underlying data:** SpaceX API v4
- **File:** `spacex_launches.csv` (205 launch records, 15 columns)

Main variables include `date_utc`, `rocket_name`, `success`, `crew_count`, `payloads_count`, `cores_reused`, `landing_success`, `landing_type`, and `launchpad_name`.

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/ARY-2007/spacex-launch-analysis
   cd spacex-launch-analysis
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Make sure `spacex_launches.csv` is in the same folder as the notebook.
4. Open `project1.ipynb` in Jupyter (or VS Code / Google Colab) and run all cells from top to bottom.

## Project Structure

```
.
├── project1.ipynb          # main analysis notebook
├── spacex_launches.csv     # dataset
├── requirements.txt        # Python dependencies
├── README.md                # this file
├── page1.png                # Mission Overview (exported chart summary)
├── page2.png                # Rocket & Booster Performance (exported chart summary)
└── page3.png                # Launch Operations & Payload (exported chart summary)
```

## Key Findings

- SpaceX's annual launch cadence increased sharply after 2016, with a especially steep rise between 2020 and 2022.
- The overall mission success rate across all recorded launches is approximately **88.3%**.
- **Falcon 9** dominates the launch record and shows the highest reliability (~90% success rate) compared to Falcon 1 (~40%) and Falcon Heavy (~60%).
- **ASDS** (droneship) landings account for the largest share of booster recovery attempts and successes, reflecting the operational preference for downrange recovery.
- Booster reuse was minimal before 2016 and grew substantially from the late 2010s onward, peaking in 2022 — indicating growing maturity of SpaceX's reusable launch operations.
- The vast majority of missions are uncrewed; crewed missions remain a small but operationally distinct fraction of total launches.
- Annual payload activity shows a generally increasing trend, reaching its highest recorded level in 2022.

## Tools

- Python
- Pandas
- Matplotlib
