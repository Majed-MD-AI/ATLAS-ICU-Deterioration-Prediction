The purpose of ATLAS v0.4 is to demonstrate a clinically coherent prediction pipeline rather than optimize a headline metric.

---

## Data Leakage: Development Lesson

Earlier ATLAS experiments produced unrealistically high performance because the outcome was indirectly related to information also present in the predictors.

That failure became a central design lesson for v0.4.

The current pipeline addresses this by:

1. defining the clinical question before model training
2. separating observation and prediction windows in time
3. excluding future-derived variables such as completed ICU length of stay from predictors
4. grouping validation by patient
5. reporting realistic rather than optimized performance

This development history is intentionally preserved because identifying and correcting leakage is an important part of clinical machine-learning practice.

---

## Limitations

- Small MIMIC-IV demo cohort
- Proxy physiological endpoint rather than a validated clinical deterioration endpoint
- Limited clinical variables
- No external validation
- Correlated summary features may affect individual coefficient estimates
- Performance estimates remain uncertain because of the small sample size
- Results should not be interpreted as evidence of clinical utility

---

## Next Steps

Future versions of ATLAS will explore:

- larger MIMIC-IV cohorts
- richer temporal and trend-based features
- clinically validated deterioration endpoints
- calibration and decision-threshold analysis
- additional interpretable baselines and more advanced models
- external or temporal validation

The priority will remain clinical validity and leakage prevention before model complexity.

---

## Data

ATLAS uses the MIMIC-IV demo dataset.

The clinical data are not included in this repository. Users should obtain the appropriate MIMIC-IV demo files separately and place them under a local data/mimic-demo/ directory.

---

## Tech Stack

- Python
- pandas
- NumPy
- scikit-learn
- matplotlib
- JupyterLab / Jupyter Notebook

---

## Author

Majed Hamad, MD  
Medical doctor transitioning into Clinical AI and clinical decision-support research.

Focus: interpretable machine learning, ICU deterioration, temporal clinical data, and clinically meaningful decision-support systems.

---

## Project Status

ATLAS v0.4 — active development

The current version establishes a temporally valid and patient-grouped baseline that can serve as the foundation for larger datasets, richer endpoints, and more advanced clinical AI methods.
