# Exoplanet Transit Detection Pipeline 🪐

An automated data engineering pipeline that ingests raw telescope telemetry, applies digital signal filtering, and utilizes the Box Least Squares (BLS) algorithm to detect periodic exoplanet transits.

## Overview
This project processes time-series data from the NASA Kepler and TESS missions. It demonstrates core concepts in signal processing and data automation:
*   **Automated Data Ingestion:** Programmatic retrieval of target pixel files via the MAST archive.
*   **Digital Signal Processing (DSP):** Flattening baselines and removing instrumental noise/outliers from raw light curves.
*   **Algorithmic Detection:** Applying BLS periodograms to isolate repeating transit signals in high-noise environments.

## Tech Stack
*   **Language:** Python
*   **Libraries:** `lightkurve`, `numpy`, `pandas`, `matplotlib`

## How to Run
1. Install dependencies: `pip install -r requirements.txt`
2. Run the pipeline: `python pipeline.py`
3. Results (phase-folded plots) will output to the `/results` directory.
