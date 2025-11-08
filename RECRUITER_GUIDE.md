# 🎯 Reply Open Day Munich 2025 - Customer Segmentation Project

## Quick Links for Recruiters

**📊 Live Project Showcase**: https://pratheekdk9919.github.io/Reply-Open-Day-Munich-/  
**📁 GitHub Repository**: https://github.com/pratheekdk9919/Reply-Open-Day-Munich-  
**📓 Interactive Notebook**: [View on GitHub](https://github.com/pratheekdk9919/Reply-Open-Day-Munich-/blob/main/Replyopenday_merged_final.ipynb)  
**📄 Executive Summary**: [Read Here](https://github.com/pratheekdk9919/Reply-Open-Day-Munich-/blob/main/EXECUTIVE_SUMMARY.txt)

---

## 🎬 30-Second Pitch

Production-ready **end-to-end ML pipeline** analyzing **541,909 retail transactions** to identify **3 actionable customer segments**. Demonstrates:
- ✅ Data strategy & KPI design
- ✅ Robust feature engineering (winsorization, interpretability heuristics)
- ✅ Unsupervised ML (K-Means with micro-cluster avoidance)
- ✅ Professional visualizations & bilingual documentation (EN/DE)
- ✅ Full reproducibility (seed control, environment freeze, version control)

---

## 💼 Why This Project Stands Out

| Dimension | Achievement |
|-----------|-------------|
| **Scale** | Half-million+ transactions, 4.3K customers |
| **Quality** | 73.5% data retained post-cleaning (robust handling) |
| **Business Impact** | Personas exportable for CRM/dashboard integration |
| **Technical Depth** | Custom k-selection heuristic, outlier documentation |
| **Presentation** | GitHub Pages showcase + bilingual docs |
| **Reproducibility** | Complete environment freeze, Git LFS for large files |

---

## 📈 Key Results

### Customer Segments Identified

1. **🔵 Base Value Seekers** (4,095 customers | 94.4%)  
   - Avg spend: £1,328 | Avg frequency: 4.1 orders  
   - *Strategy*: Retention campaigns, cross-sell bundles

2. **🔴 Enterprise Outlier** (1 customer | 0.02%)  
   - Avg spend: £1.44M | Avg frequency: 1,441 orders  
   - *Strategy*: White-glove service, contract management

3. **🟢 Emerging Loyalists** (242 customers | 5.6%)  
   - Avg spend: £8,763 | Avg frequency: 6.4 orders  
   - *Strategy*: Loyalty program enrollment, premium product upsells

### Technical Metrics
- **Clustering Method**: K-Means (interpretability-aware heuristic)
- **Optimal K**: 3 (balanced separation, micro-cluster avoidance)
- **Feature Set**: Total spend, purchase frequency, average order value
- **Preprocessing**: Winsorization (1%/99%), standard scaling, minimal imputation

---

## 🛠️ Technical Stack

**Languages & Libraries**:  
Python 3.x | pandas | NumPy | scikit-learn | Matplotlib | Seaborn

**Tools**:  
Jupyter Notebook | Git | GitHub | GitHub Pages | Git LFS

**Methodologies**:  
K-Means Clustering | Elbow Method | Silhouette Analysis | Feature Scaling | Outlier Detection

---

## 🎓 Demonstrated Competencies

### Data Engineering & Strategy
- Business-first KPI design (return rate, AOV, frequency)
- Robust data quality pipeline (missing value strategy, type coercion)
- Feature engineering (weekday derivation, transaction flags)

### Machine Learning
- Unsupervised clustering with interpretability guardrails
- Custom heuristic for k-selection (prevent micro-clusters)
- Model evaluation (elbow, silhouette, Davies-Bouldin)
- Transparent outlier handling & documentation

### Software Engineering
- Reproducible pipelines (fixed seeds, environment management)
- Version control best practices (Git workflow, LFS)
- Professional documentation (README, executive summary, code comments)

### Communication & Presentation
- Bilingual technical docs (English & German)
- Interactive GitHub Pages showcase
- Persona export (JSON) for downstream integration
- Stakeholder-ready visualizations

---

## 📂 Repository Structure

```
Reply-Open-Day-Munich-/
├── docs/
│   └── index.html              # GitHub Pages showcase
├── legacy/                      # Archived original notebooks
├── Replyopenday_merged_final.ipynb  # Main analysis pipeline
├── cleaned_online_retail.csv   # Processed dataset
├── customer_segmentation_results.csv  # Segments + labels
├── elbow.png / silhouette.png / segments.png  # Visualizations
├── personas.json               # Cluster descriptions
├── requirements.txt            # Core dependencies
├── requirements_generated.txt  # Full frozen environment
├── EXECUTIVE_SUMMARY.txt       # Business narrative
└── README.md                   # Project documentation
```

---

## 🚀 Quick Start (For Technical Review)

```powershell
# Clone repository
git clone https://github.com/pratheekdk9919/Reply-Open-Day-Munich-.git
cd Reply-Open-Day-Munich-

# Setup environment
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt

# Launch notebook
jupyter notebook Replyopenday_merged_final.ipynb
```

Run cells top-to-bottom. All artifacts regenerate in ~5 minutes.

---

## 🌟 Extensibility Roadmap

Future enhancements documented in notebook:
- **RFM Analysis**: Recency/Frequency/Monetary scoring for CLV modeling
- **Outlier Mitigation**: Z-score filtering + re-clustering for balanced segments
- **Anomaly Detection**: IsolationForest or DBSCAN for spend spikes
- **Modularization**: Extract to Python package with CLI
- **Experiment Tracking**: MLflow/DVC integration for parameter sweeps

---

## 📞 Contact & Discussion

**GitHub**: [@pratheekdk9919](https://github.com/pratheekdk9919)  
**Project Page**: https://pratheekdk9919.github.io/Reply-Open-Day-Munich-/

Open to discussing:
- Technical implementation details
- Business application of segments
- Scalability & production deployment
- Team collaboration & agile workflows

---

## 🏆 Recruiter Takeaway

This project demonstrates **end-to-end ML capability** from raw data to production-ready insights:

✅ **Strategic thinking** (KPI design, stakeholder alignment)  
✅ **Technical rigor** (reproducibility, outlier handling, interpretability)  
✅ **Communication skills** (bilingual docs, interactive showcase)  
✅ **Production mindset** (environment management, version control, extensibility)

**Ready for review. Let's discuss how these skills apply to your team's challenges.**

---

*Last Updated: November 2025 | Status: ✅ Production-Ready*
