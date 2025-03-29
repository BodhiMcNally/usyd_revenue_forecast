# Forecasting Study Load at the University of Sydney  
**STAT3926/STAT4026: Statistical Consulting Project**  
📅 **Published:** May 20, 2024  
👨‍💻 **Authors:** 520432255, 510288769, 510456265  
🎯 **Client:** Susie Chee

---

## 📌 Project Summary

This project presents a forecasting model to estimate student enrolments (measured by EFTSL) at the University of Sydney, specifically in response to new 2024 government policies impacting international student enrolments. A faculty-level linear modelling approach was employed to estimate enrolment loads for budgeting purposes. Although the model was outperformed by the university’s existing forecast system, it shows potential for future application with a larger dataset and additional predictors.

---

## 🎯 Client’s Aims

- Estimate enrolment numbers **before the Census date** to confirm budget targets.
- Account for **fee types (CSP, DFEE, IFEE)**, **semesters**, and **COVID-19 impact**.
- Build separate models for each faculty.
- Forecast impact of **policy changes affecting international student behaviour**.

---

## 🧠 Methodology

### 📊 Data
- Historical EFTSL data from 2018–2023.
- 8 major faculties considered (e.g., Science, Business, Engineering).
- Fee types: CSP (domestic supported), DFEE (domestic full fee), IFEE (international).

### 🛠 Modelling
- Built 24 **linear regression models** (one per faculty × fee type).
- Predictors: **Year**, **Semester**, **COVID-19 impact**.
- Evaluation using **R², AIC/AICc, MAE**, and **diagnostic plots**.

### 📈 Evaluation
- R² values ranged from **~0.1 to 0.96**, depending on faculty/fee type.
- Mean Absolute Error (MAE) calculated against actual 2023 data and compared to existing forecasts.
- **Percentage change** trends also compared across forecast methods.

---

## 🔍 Key Insights

- CSP and IFEE categories had relatively **high model accuracy**.
- DFEE predictions were **less reliable** due to **limited data**.
- COVID-19 had **varying effects** across faculties.
- **Policy changes in 2024** could shift Semester 2 behaviour, limiting predictive accuracy.

---

## 💸 2024 Budget Forecast

| Faculty | Estimated EFTSL | Projected Income (AUD) |
|--------|------------------|------------------------|
| Business | 11,582 | $545.8M |
| Arts & Social Sciences | 14,949 | $571.1M |
| Engineering | 8,516 | $378.8M |
| Medicine & Health | 9,860 | $383.3M |
| Science | 8,033 | $312.0M |
| Conservatorium | 1,229 | $33.8M |
| Law | 2,054 | $74.5M |
| Architecture | 3,133 | $117.3M |
| **Total** | **59,356** | **$2.42B** |

> ✅ Forecast suggests the university is **on track to meet its 2024 budget.**

---

## ⚠️ Limitations

- Small dataset (6 years) → potential **overfitting** and unreliable extrapolation.
- **New enrolment behaviours** due to 2024 policy not captured in historical data.
- Does not account for **external drivers** like economic factors or marketing changes.

---

## 🧭 Future Work

- Integrate **more historical data** and refine predictors.
- Explore **non-linear** models or ensemble methods.
- Apply to **semester-specific forecasting** models with updated policy assumptions.

---
