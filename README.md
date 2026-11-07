<h2 align="center">Swaminathan Sankaran</h2>

<p align="center">
MS Data Science @ University at Buffalo · graduating December 2026<br>
I build ML systems and check whether their results actually hold up.<br>
Open to data science, ML engineering and AI engineering roles.
</p>

<p align="center">
<a href="https://www.swaminathansankaran.com">Website</a> ·
<a href="https://www.linkedin.com/in/swaminathan-sankaran-02643524b/">LinkedIn</a> ·
<a href="https://www.swaminathansankaran.com/assets/swaminathan_resume.pdf">Résumé (PDF)</a>
</p>

---

## Featured Projects

### [US Electricity Demand Forecast Audit](https://github.com/jinnn11/grid-forecast-audit)

Pre-registered audit of 10 years of day-ahead electricity demand forecasts for 50+ US grid operators (6.1M hourly records from EIA-930). Found three errors in EIA's public data, verified against the operators' own records, that made forecast accuracy appear to decline. Once they are corrected, the 10-year trend is flat, and California's 2025 forecast error falls from 8.3% to 2.4%.

`Python` `pandas` `Time Series` `Statistical Testing` `Data Quality`

---

### [Compositional Grounding Probes](https://github.com/jinnn11/compositional-grounding-probes)

Diagnostic benchmark for testing whether open-vocabulary segmentation models understand compositional prompts such as negation, spatial relations, attribute binding, and fine-grained categories. Built with Grounding DINO and SAM, with 914 human-verified probes across 608 images. Analysis revealed severe grounding failures, including 20.7% negation accuracy and 0/51 spatial pair consistency.

`Python` `PyTorch` `Grounding DINO` `SAM` `Computer Vision` `Vision-Language Models`

---

### [Drift-Aware MLOps Pipeline](https://github.com/jinnn11/drift-aware-mlops-pipeline)

Predicts term-deposit sign-ups (UCI Bank Marketing) with an XGBoost model served by FastAPI, with every prediction logged to PostgreSQL, drift checks in Evidently, Prometheus and Grafana, and retraining run by Airflow and tracked in MLflow. A retrained model only ships if it gains at least 0.005 PR-AUC on shifted data without losing more than 0.03 ROC-AUC on historical data; in a simulated recession, retraining lifted shifted-data PR-AUC from 0.84 to 0.89.

`Python` `XGBoost` `FastAPI` `PostgreSQL` `Airflow` `MLflow` `Evidently` `Docker`

---

### [CT Scan Tamper Classification](https://github.com/jinnn11/ct-tamper-classification)

Two-person team project: PyTorch models that classify 3D lung CT patches as authentic or GAN-tampered (tumors injected or removed), on a public 100-scan dataset. A 3D-to-2D compressor feeding ResNet-18 ranked first of five designs on scans held out of training.

`Python` `PyTorch` `Computer Vision` `Medical Imaging`

---

### [Molecular Similarity Prediction](https://github.com/jinnn11/molecular-similarity-prediction)

Contrastive pretraining of 2D-image, 3D-conformer and fingerprint encoders on 291,742 drug-like molecules (GEOM-Drugs), tested on 200 rated molecule pairs. The averaged embedding similarity reaches a Pearson correlation of 0.90 with no training on the ratings, and the three views turn out largely redundant.

`Python` `PyTorch` `RDKit` `Contrastive Learning`

---

### Currently

An LLM benchmark for pulling revenue, net income and EPS out of earnings press releases, with every answer graded automatically against SEC filings, including my own LoRA fine-tune of Qwen3-8B.

### Technical Interests

LLM Evaluation · Time Series & Forecasting · MLOps · Computer Vision · Vision-Language Models
