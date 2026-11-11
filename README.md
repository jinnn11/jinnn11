<h2 align="center">Nathan Sankaran</h2>

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

### [SEC Earnings Extraction: LLM Benchmark, Fine-Tuning and Serving](https://github.com/jinnn11/sec-earnings-bench)

Links about 4,700 SEC earnings releases to the XBRL figures in each company's matching 10-Q/10-K, with an auto-grader that scores LLM-extracted revenue, net income and EPS and classifies every error. Across 9 LLMs, a figure-plus-unit reply format cut open-model errors 65%. A LoRA fine-tune of Qwen3-8B raised accuracy on 37 unseen companies from 89.1% to 99.2% (+10.1 points, 95% CI +5.1 to +15.6); served in FP8 with vLLM on one H100, it reads 6,143 releases an hour at $0.56 per 1,000.

`Python` `PyTorch` `PEFT (LoRA)` `vLLM` `AWQ` `pandas`

---

### [US Electricity Demand Forecast Audit](https://github.com/jinnn11/grid-forecast-audit)

Pre-registered audit of 10 years of day-ahead electricity demand forecasts for 50+ US grid operators (6.1M hourly records from EIA-930). Found three errors in EIA's public data, verified against the operators' own records, that made forecast accuracy appear to decline. Once they are corrected, the 10-year trend is flat, and California's 2025 forecast error falls from 8.3% to 2.4%.

`Python` `pandas` `Time Series` `Statistical Testing` `Data Quality`

---

### [Compositional Grounding Probes](https://github.com/jinnn11/compositional-grounding-probes)

Diagnostic benchmark for testing whether open-vocabulary segmentation models understand compositional prompts such as negation, spatial relations, attribute binding, and fine-grained categories. Built with Grounding DINO and SAM, with 914 human-verified probes across 608 images. Analysis revealed severe grounding failures, including 20.7% negation accuracy and 0/51 spatial pair consistency.

`Python` `PyTorch` `Grounding DINO` `SAM` `Computer Vision` `Vision-Language Models`

---

### [Drift-Aware Retraining: Experiment and MLOps Pipeline](https://github.com/jinnn11/drift-aware-mlops-pipeline)

Should a model be retrained when its data drifts, or on a schedule? On 36 months of Lending Club loans with outcomes arriving 1–6 months late, quarterly retraining matched monthly within 0.001 PR-AUC with 69% fewer retrains, while drift triggers needed up to 60% more retrains for the same accuracy. In an injected-drift benchmark, input-only drift tests missed concept drift that a label-based calibration test caught every time (89–97% alarm precision). The rules run in an MLOps pipeline I built: FastAPI with every prediction logged to PostgreSQL, Evidently drift checks on the logged predictions, Airflow retraining tracked in MLflow, a held-out promotion gate and one-step rollback.

`Python` `XGBoost` `SciPy` `FastAPI` `PostgreSQL` `Evidently` `Airflow` `MLflow` `Docker`

---

### [CT Scan Tamper Classification](https://github.com/jinnn11/ct-tamper-classification)

Two-person team project: PyTorch models that classify 3D lung CT patches as authentic or GAN-tampered (tumors injected or removed), on a public 100-scan dataset. A 3D-to-2D compressor feeding ResNet-18 ranked first of five designs on scans held out of training.

`Python` `PyTorch` `Computer Vision` `Medical Imaging`

---

### [Molecular Similarity Prediction](https://github.com/jinnn11/molecular-similarity-prediction)

Contrastive pretraining of 2D-image, 3D-conformer and fingerprint encoders on 291,742 drug-like molecules (GEOM-Drugs), tested on 200 rated molecule pairs. The averaged embedding similarity reaches a Pearson correlation of 0.90 with no training on the ratings, and the three views turn out largely redundant.

`Python` `PyTorch` `RDKit` `Contrastive Learning`

---

### Technical Interests

LLM Evaluation · Time Series & Forecasting · MLOps · Computer Vision · Vision-Language Models
