# Bayesian Analysis of Hydroxyurea Treatment Effects on Cats with Erythrocytosis
 
---

## Overview
This project uses a **Bayesian hierarchical linear model** to evaluate how different doses of **hydroxyurea** affect the **packed cell volume (PCV)** in cats with erythrocytosis. The analysis also compares treatment responses between **domestic** and **non-domestic** breeds while controlling for disease type.

---

## Data Summary
Data were collected from **40 cats**, including:
- **Type:** 1 = Primary erythrocytosis, 0 = Secondary  
- **Breed:** A–E (A–C = domestic, D–E = non-domestic)  
- **Dose:** Hydroxyurea dosage over 3 months  
- **ΔPCV:** Change in packed cell volume after treatment  

---

## Methods
A **Bayesian hierarchical regression model** was implemented in **R** using **JAGS** to estimate posterior distributions.  
- Weakly informative priors and 3 MCMC chains (50k iterations post burn-in) were used.

---

## Key Results
- **Dose Effect (β₂):** Posterior mean = −0.397, 95% CI [−0.543, −0.253]  
  → Higher doses significantly reduce PCV.  
- **Breed Effect:** Domestic cats show greater PCV reduction than non-domestic cats.  
  Difference (domestic − non-domestic) = −2.12, 95% CI [−2.76, −1.44]  

---

## Conclusion
Hydroxyurea effectively lowers PCV in cats with erythrocytosis, with stronger effects at higher doses. Domestic breeds exhibit a significantly greater reduction compared to non-domestic breeds.

---
## 🗂 Repository Structure
```markdown
Bayesian-Hydroxyurea-Analysis/
├── DATA/                                                   # Folder Containing Model
│   ├── cat_model.txt                                       # Model used to run analysis        
├── .Rhistory
├── .README.md                                              # Presentation Slides Summarizing Project                 
├── STAT-4350-Final-Project.pdf                             # R Markdown file of report        
├── hydroxyurea_erythrocytosis_bayesian.Rmd                 # R Markdown File of Report
└── hydroxyurea_erythrocytosis_bayesian.pdf                 # Report 










## Structure





