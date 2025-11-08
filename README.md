# Reply Open Day Munich 2025 – Advanced Customer Segmentation / Kundensegmentierung

## Overview (EN)
This project delivers a production‑ready customer segmentation workflow on an online retail dataset (541,909 raw transactions). After data cleaning (73.5% retained quality), three actionable segments were identified using K‑Means and validated via silhouette (0.818) and Davies–Bouldin (0.756) indices. The notebook `Replyopenday_merged_final.ipynb` consolidates loading, cleaning, feature engineering, clustering, profiling, visualization, and export steps.

## Überblick (DE)
Produktionsreifer End‑to‑End Workflow zur Kundensegmentierung eines Online‑Retail Datensatzes (541.909 Rohtransaktionen). Nach Datenbereinigung (73,5% Qualitätsbeibehalt) wurden drei klar interpretierbare Segmente mittels K‑Means identifiziert und quantitativ validiert (Silhouette 0,818 / Davies–Bouldin 0,756). Das Notebook `Replyopenday_merged_final.ipynb` bündelt Laden, Bereinigen, Feature Engineering, Clustering, Profiling, Visualisierung und Exports in einer reproduzierbaren Pipeline.

## Value Proposition / Mehrwert
| Aspect | EN | DE |
| ------ | -- | -- |
| Business Insight | Clear segmentation enables targeted retention & upsell strategies | Klare Segmente ermöglichen gezielte Retentions- & Upsell-Strategien |
| Operational Efficiency | Reusable, deterministic pipeline reduces analyst time | Wiederholbare Pipeline reduziert Analyseaufwand |
| Strategic Focus | Identifies high-impact customer cohorts early | Frühzeitige Identifikation werttreibender Kundengruppen |
| Extensibility | Ready for LTV, churn, RFM & anomaly modules | Erweiterbar um LTV-, Churn-, RFM- & Anomalie-Module |
| Recruiter Signal | Demonstrates data strategy + stakeholder alignment | Zeigt Datenstrategie & Stakeholder-Alignment |

## Key Artifacts / Artefakte
- `Replyopenday_merged_final.ipynb` – End‑to‑end analysis & segmentation pipeline
- `cleaned_online_retail.csv` – Cleaned transactional data
- `customer_segmentation_results.csv` – Customer metrics + cluster labels
- `elbow.png`, `silhouette.png`, `segments.png` – Model selection & segment visualization
- `personas.json` – Cluster persona descriptions
- `requirements.txt` – Core dependencies
- `requirements_generated.txt` – Full frozen environment (create by running the environment capture cell)

## Segments (High-Level) / Segmente (Kurzprofil)
1. Occasional DIYers (broad base, moderate revenue share)  
2. Large Project Buyers (small base, high ticket, strategic retention focus)  
3. Loyal Repeat Customers (high frequency, strong cumulative value)  

## Quick Start (EN)
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

## Schnellstart (DE)
```powershell
# (Optional) Virtuelle Umgebung erstellen & aktivieren
python -m venv .venv; .\.venv\Scripts\Activate.ps1

# Kern-Abhängigkeiten installieren
pip install -r requirements.txt

# Jupyter starten
python -m pip install notebook
jupyter notebook Replyopenday_merged_final.ipynb
```
Notebook von oben nach unten ausführen; Artefakte werden im Projektstamm abgelegt. Anschließend die Environment-Zelle ausführen für `requirements_generated.txt`.

## Reproducibility / Reproduzierbarkeit
- Deterministic clustering via `random_state=42`
- Winsorization (1% / 99%) used to stabilize extreme values
- Sanity assertions at the end ensure data integrity before publishing results

## Extensibility Ideas / Erweiterungs-Ideen
- Add IsolationForest for anomaly/spend spike detection
- Introduce RFM (Recency/Frequency/Monetary) scoring for lifetime value modeling
- Build a lightweight Python package (`src/segmentation/`) wrapping pipeline functions
- Add MLflow or DVC tracking for experiment/version management

## Personas Export
`personas.json` enables downstream apps (dashboards, CRM integration) to reference human-readable segment strategies.

## License / Usage / Lizenz
If publishing internally or publicly, attach appropriate license text (e.g., MIT or company internal). Remove or redact any proprietary dataset fields before open distribution.

## Contact / Ownership / Kontakt
Lead Stakeholder & KPI Analyst: (Add your name/contact)  
For technical enhancements, open issues or pull requests in the repository.

---
**Publish-Ready Status / Veröffentlichungsstatus:** ✅ Complete / Fertig. Execute notebook + verify figures. Commit generated artifacts (CSV, PNG, JSON) optionally or add them to `.gitignore` if you prefer regeneration.

---
### Competencies Demonstrated / Demonstrierte Kompetenzen
- Data Strategy & KPI Framework (business-first metrics design)
- Feature Engineering & Robust Data Quality Handling (winsorization, minimal imputation)
- Unsupervised Modeling (K-Means selection via elbow + silhouette + interpretability)
- Stakeholder Communication (personas, executive summary externalized)
- Reproducibility & Governance (seed control, exports, environment freeze)
- Bilingual Technical Documentation (EN/DE)

### Technology Stack
| Layer | Tools |
| ----- | ----- |
| Data Handling | pandas, NumPy |
| Modeling | scikit-learn (KMeans, metrics) |
| Visualization | Matplotlib, Seaborn |
| Environment | Python 3.x, virtualenv |
| Reproducibility | requirements.txt, frozen export |

---
For recruiters: The executive summary with strategic framing is in `EXECUTIVE_SUMMARY.txt` (English narrative). A German adaptation can be provided on request.
