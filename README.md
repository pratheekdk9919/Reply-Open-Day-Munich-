# Reply Open Day Munich 2025 – Advanced Customer Segmentation / Kundensegmentierung

## Overview (EN)
This project delivers a production‑ready customer segmentation workflow on an online retail dataset (541,909 raw transactions). After data cleaning (73.5% retained quality), three actionable segments were identified using K‑Means with interpretability safeguards (micro‑cluster avoidance). The notebook `Replyopenday_merged_final.ipynb` consolidates loading, cleaning, feature engineering, clustering (with heuristic selection), profiling, visualization, and export steps.

## Überblick (DE)
Produktionsreifer End‑to‑End Workflow zur Kundensegmentierung eines Online‑Retail Datensatzes (541.909 Rohtransaktionen). Nach Bereinigung (73,5% Qualitätsbeibehalt) wurden drei interpretierbare Segmente mittels K‑Means identifiziert (Heuristik verhindert Mikro‑Cluster). Das Notebook `Replyopenday_merged_final.ipynb` vereint Laden, Bereinigen, Feature Engineering, Clustering, Profiling, Visualisierung & Exporte.

## Value Proposition / Mehrwert
| Aspect | EN | DE |
| ------ | -- | -- |
| Business Insight | Targeted retention & upsell strategies | Zielgerichtete Retentions- & Upsell-Strategien |
| Operational Efficiency | Deterministic pipeline saves analyst time | Deterministische Pipeline spart Analysezeit |
| Strategic Focus | Early identification of high-impact cohorts | Früherkennung werttreibender Kundengruppen |
| Extensibility | Ready for LTV, churn, RFM, anomaly modules | Erweiterbar um LTV-, Churn-, RFM-, Anomalie-Module |
| Recruiter Signal | Shows data strategy & stakeholder alignment | Zeigt Datenstrategie & Stakeholder-Alignment |

## Key Artifacts / Artefakte
- `Replyopenday_merged_final.ipynb` – End‑to‑end pipeline
- `cleaned_online_retail.csv` – Bereinigte Transaktionsdaten
- `customer_segmentation_results.csv` – Kundenmetriken + Cluster
- `elbow.png`, `silhouette.png`, `segments.png` – Modellselektion & Segmentvisualisierung
- `personas.json` – Beschreibungen / personas
- `requirements.txt` – Kernabhängigkeiten
- `requirements_generated.txt` – Vollständige eingefrorene Umgebung

## Segments (High-Level) / Segmente (Kurzprofil)
1. Base Value Seekers / Preisbewusste Basis (breite Basis, moderat)
2. Enterprise / Project Outlier (extrem hoher Einzelwert – dokumentierter Ausreißer)
3. Emerging Loyalists / Aufbauende Loyalisten (höhere Frequenz + Premium AOV)

Note: A single extreme outlier remains (Cluster 1). Retained intentionally for transparency; can be excluded via spend/frequency z‑score filtering if a strictly balanced segmentation is required.

## Quick Start (EN)
```powershell
# (Optional) create & activate virtual environment
python -m venv .venv; .\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
python -m pip install notebook
jupyter notebook Replyopenday_merged_final.ipynb
```
Run top-to-bottom; artifacts are written to project root. Execute the environment capture cell last to refresh `requirements_generated.txt`.

## Schnellstart (DE)
```powershell
python -m venv .venv; .\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
python -m pip install notebook
jupyter notebook Replyopenday_merged_final.ipynb
```
Von oben nach unten ausführen; Artefakte werden im Stammverzeichnis erzeugt. Danach Environment-Zelle für `requirements_generated.txt`.

## Reproducibility / Reproduzierbarkeit
- Fixed `random_state=42` in all stochastic steps
- Winsorization (1% / 99%) stabilizes extremes
- Sanity assertions validate integrity & persona coverage
- Environment freeze for deterministic reinstall

## Extensibility Ideas / Erweiterungs-Ideen
- RFM / CLV module
- Outlier mitigation + re-clustering (remove single-point segment)
- IsolationForest or DBSCAN for anomaly tagging
- Modularize pipeline into a lightweight package + CLI
- Add MLflow tracking & parameter sweeps

## Personas Export
`personas.json` supports downstream dashboards / CRM enrichment.

## License / Usage / Lizenz
Attach appropriate license (e.g., MIT) if open-sourcing; remove proprietary fields before distribution.

## Contact / Ownership / Kontakt
Owner / Analyst: <Your Name / Kontakt>
For enhancements, open an Issue or PR.

---
**Status:** ✅ Publish-ready (with documented outlier segment). For a balanced variant, filter the extreme outlier and re-run cells 13–19.

### Competencies Demonstrated / Kompetenzen
- Data Quality Engineering & KPI Framework
- Unsupervised Modeling (K‑Means + heuristic selection)
- Outlier Analysis & Interpretability Controls
- Reproducibility & Environment Governance
- Bilingual Technical Communication (EN/DE)

### Technology Stack
| Layer | Tools |
| ----- | ----- |
| Data Handling | pandas, NumPy |
| Modeling | scikit-learn |
| Visualization | Matplotlib, Seaborn |
| Environment | Python 3.x, virtualenv |
| Reproducibility | requirements.txt, frozen export |

---
Executive summary: see `EXECUTIVE_SUMMARY.txt` (EN). German adaptation on request.
