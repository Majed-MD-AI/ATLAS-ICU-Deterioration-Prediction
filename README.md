## 🧠 ATLAS — Clinical AI for Early Patient Deterioration

ATLAS is a clinical AI prototype focused on early detection of patient deterioration in ICU settings.

This project is designed from a clinician's perspective, emphasizing:
- Interpretability over black-box performance  
- Clinical reasoning over pure metrics  
- Real-world applicability over idealized results  

Rather than optimizing for accuracy alone, ATLAS explores how machine learning can support meaningful clinical decision-making.

---

## 🚀 Current Version

ATLAS v0.3 — includes:
- Feature engineering from vital signs (HR, SBP, SpO2)
- Clinical trend-based features
- Identification and handling of data leakage
- Baseline logistic regression model

---

## 📊 Project Overview

This project explores how machine learning can be applied to detect early warning signs of patient deterioration in critical care settings.

The current version focuses on building a simple, interpretable baseline model using limited clinical features, while highlighting key challenges such as data leakage and small dataset limitations.

---

## 🏥 Clinical Perspective

In real-world ICU environments, early detection of deterioration can significantly impact patient outcomes.

This project reflects a simplified version of a larger vision:  
Building intelligent systems that assist clinicians in making faster, safer, and more informed decisions.

---

## ⚙️ Implementation

The workflow includes:
- Data preparation using pandas  
- Feature engineering from vital signs  
- Train-test split  
- Model training using logistic regression  
- Performance evaluation  

---

## 📈 Results

- Initial accuracy reached artificially high levels due to data leakage  
- After fixing leakage, performance dropped to more realistic levels (~0.7 accuracy)  
- Model behavior became more aligned with clinical expectations  

---

## ⚠️ Data Leakage (Critical Finding)

The initial model achieved extremely high accuracy (~1.0), which appeared unrealistic.

Upon investigation, it was found that the outcome variable was indirectly derived from one of the input features (shock index), leading to data leakage.

This highlighted the importance of proper outcome definition and strict separation between features and labels in clinical machine learning tasks.

---

## 💡 Key Insight

This was a critical learning point:

> Building clinical AI systems is not just about model performance.  
> It requires careful understanding of data, feature construction, and clinical reasoning.

This experience highlights the importance of validating assumptions and avoiding misleading results in healthcare applications.

---

## 🔄 Next Step

Replace the temporary leakage-based outcome with a real clinical endpoint (e.g., mortality or deterioration event), then retrain the ATLAS feature-based model.

---

## 🧪 Tech Stack

- Python  
- pandas  
- scikit-learn  
- Jupyter Notebook  

---

## ▶️ How to Run

1. Open the notebook  
2. Run all cells  

---

## 👤 Author

Majed Hamad  
Medical Doctor transitioning into Clinical AI  

Focused on building intelligent systems that bridge medicine and machine learning.

---

## 🔗 Project Status

ATLAS is currently under active development (v0.3).

This version focuses on building a clinically meaningful baseline system, with emphasis on interpretability, data limitations, and real-world applicability rather than pure performance.
