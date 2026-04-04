# ATLAS — Clinical AI for Early Patient Deterioration

ATLAS is a clinical AI prototype designed to explore early detection of patient deterioration in critical care settings using interpretable machine learning and simple clinical features.

Rather than focusing solely on model performance, this project emphasizes clinical reasoning, data limitations, and real-world applicability of AI systems in healthcare.

---

## 🧠 Motivation

During clinical practice in emergency and ICU settings, early signs of patient deterioration are often present but not systematically utilized.

This project was built to explore how machine learning can assist in identifying these early warning signals and support clinical decision-making.

---

## ⚙️ Project Overview

This prototype uses a small subset of clinical data (MIMIC-IV demo) and focuses on:

- Vital signs (HR, SBP, SpO2, RR)
- Derived features (Shock Index, Oxygen-related indicators)
- Simple baseline models:
  - Logistic Regression
  - Random Forest

The goal is to simulate a clinical early warning system, not just a prediction model.

---

## 📊 Key Results & Observations

- Initial experiments produced artificially high performance (accuracy ≈ 1.0)
- Investigation revealed data leakage due to improper feature construction

⚠️ This was a critical turning point in the project.

After correcting for leakage:

- Model performance dropped to more realistic levels (~0.7 accuracy)
- Positive class detection remained limited due to severe class imbalance

---

## ⚠️ Limitations

This project intentionally highlights real-world challenges:

- Small dataset (MIMIC demo)
- Severe class imbalance
- Limited generalizability
- Simplified feature set

These limitations are part of the learning process, not just constraints.

---

## 🧪 Clinical Perspective

In real ICU environments, early detection of deterioration can significantly impact patient outcomes.

ATLAS reflects an early-stage attempt to bridge the gap between:

- Data availability  
- Clinical usability  
- Decision support systems  

---

## 🚀 Future Directions

This project is part of a broader vision to develop clinically integrated AI systems.

Next steps may include:

- Incorporating time-series modeling  
- Using larger real-world datasets  
- Improving feature engineering (labs, trends)  
- Designing actionable risk scoring systems  
- Moving toward real clinical deployment  

---

## 🛠️ Tech Stack

- Python  
- Pandas  
- Scikit-learn  
- Jupyter Notebook  

---

## ▶️ How to Run

1. Open the notebook:
2. 2. Run all cells

---

## 👨‍⚕️ Author

Majed Hamad  
Medical Doctor transitioning into Clinical AI  

Focused on building intelligent systems that bridge medicine and machine learning.

---

## 🔗 Project Status

ATLAS is currently under active development (v0.3).

This version focuses on building a clinically meaningful baseline system, with emphasis on interpretability, data limitations, and real-world applicability rather than pure performance.

