# Reply Open Day Munich 2025 – Advanced Customer Segmentation

## Overview
This project delivers a production‑ready customer segmentation workflow on an online retail dataset (541,909 raw transactions). After data cleaning (73.5% retained quality), three actionable segments were identified using K‑Means and validated via silhouette (0.818) and Davies–Bouldin (0.756) indices. The notebook `Replyopenday_merged_final.ipynb` consolidates loading, cleaning, feature engineering, clustering, profiling, visualization, and export steps.

## Key Artifacts
- `Replyopenday_merged_final.ipynb` – End‑to‑end analysis & segmentation pipeline
- `cleaned_online_retail.csv` – Cleaned transactional data
- `customer_segmentation_results.csv` – Customer metrics + cluster labels
- `elbow.png`, `silhouette.png`, `segments.png` – Model selection & segment visualization
- `personas.json` – Cluster persona descriptions
- `requirements.txt` – Core dependencies
- `requirements_generated.txt` – Full frozen environment (create by running the environment capture cell)

## Segments (High-Level)
1. Occasional DIYers (broad base, moderate revenue share)  
2. Large Project Buyers (small base, high ticket, strategic retention focus)  
3. Loyal Repeat Customers (high frequency, strong cumulative value)  

## Quick Start
```powershell
# (Optional) create & activate virtual environment
python -m venv .venv; .\.venv\Scripts\Activate.ps1

# Install core dependencies
pip install -r requirements.txt

# Launch Jupyter
python -m pip install notebook
jupyter notebook Replyopenday_merged_final.ipynb
```

Run the notebook top-to-bottom. Artifacts will be saved to the project root. After execution, run the environment capture cell to produce `requirements_generated.txt` for reproducibility.

## Reproducibility
- Deterministic clustering via `random_state=42`
- Winsorization (1% / 99%) used to stabilize extreme values
- Sanity assertions at the end ensure data integrity before publishing results

## Extensibility Ideas
- Add IsolationForest for anomaly/spend spike detection
- Introduce RFM (Recency/Frequency/Monetary) scoring for lifetime value modeling
- Build a lightweight Python package (`src/segmentation/`) wrapping pipeline functions
- Add MLflow or DVC tracking for experiment/version management

## Personas Export
`personas.json` enables downstream apps (dashboards, CRM integration) to reference human-readable segment strategies.

## License / Usage
If publishing internally or publicly, attach appropriate license text (e.g., MIT or company internal). Remove or redact any proprietary dataset fields before open distribution.

## Contact / Ownership
Lead Stakeholder & KPI Analyst: (Add your name/contact)  
For technical enhancements, open issues or pull requests in the repository.

---
**Publish-Ready Status:** ✅ Complete. Execute notebook + verify figures. Commit generated artifacts (CSV, PNG, JSON) optionally or add them to `.gitignore` if you prefer regeneration.
