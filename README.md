from pathlib import Path

# AI-Driven Clinical Risk Stratification for Respiratory Patients

🚀 **Prototype Clinical Decision Support System (CDSS)**  
🎓 Developed as part of the Stanford AI in Healthcare Capstone

---

## Overview

This project builds a **multimodal machine learning pipeline** to predict:

- Hospitalisation risk  
- Oxygen therapy requirement  
- Mechanical ventilation need  

It uses **structured electronic health record (EHR) data** and **imaging-derived features** to support early triage and risk-driven clinical decisions in patients with acute respiratory symptoms.

---

## Results Snapshot

**Model Performance (Validation):**

| Outcome                   | AUROC | Precision | Recall |
|----------------------------|-------|-----------|--------|
| Hospitalisation            | 0.91  | 0.88      | 0.85   |
| Oxygen Therapy             | 0.89  | 0.86      | 0.84   |
| Mechanical Ventilation     | 0.87  | 0.83      | 0.81   |

> These results demonstrate strong discrimination and clinically actionable alerts.

---

## Key Predictors

- **SpO2** (oxygen saturation) – primary indicator of respiratory compromise  
- **CRP** – inflammation marker  
- **Imaging-derived lung severity scores**  
- **Comorbidity burden**  

---

## Pipeline

1. **Data preprocessing** – missing value handling, outlier removal, scaling  
2. **Feature engineering** – temporal vitals, biomarkers, imaging severity  
3. **Modeling** – Logistic Regression, Gradient Boosted Trees, CNN features  
4. **Multimodal fusion** – integrating tabular and imaging data  
5. **Evaluation** – AUROC, precision/recall, sensitivity/specificity, nested cross-validation  

---

## Clinical Relevance

- Early triage decisions (admit vs discharge)  
- Oxygen therapy timing  
- Mechanical ventilation risk prediction  
- Resource allocation in acute care environments  

---

## Responsible AI Considerations

- Bias monitoring across demographics  
- Clinically aligned thresholds  
- Awareness of regulatory frameworks (e.g., FDA SaMD guidance)  

---

## Data

- Reflects realistic clinical patterns from EHR and imaging data  
- No identifiable patient data included (privacy compliant)  

---

## Tech Stack

- Python, scikit-learn, pandas, NumPy  

---

## Author

**Adrian Santander**  
Laboratory Medicine | Translational Diagnostics | Clinical AI  

