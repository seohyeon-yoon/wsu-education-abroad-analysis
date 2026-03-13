# WSU Education Abroad Program Analysis (2008–2025)

Exploratory data analysis of 17 years of Washington State University Education Abroad participation records, examining enrollment trends, program composition, geographic distribution, and equity gaps across colleges and majors.

---

## Project Overview

This project analyzes institutional records from WSU's Education Abroad office spanning 2008 to 2025. The goal is not only to describe participation patterns over time, but to surface actionable questions for program planning, access, and diversification.

**Key questions explored:**
- How has participation changed over time, including the COVID-19 disruption and recovery?
- Which program types, majors, and destinations dominate — and which are underrepresented?
- Where do equity gaps exist across colleges, majors, and geographic regions?

---

## Dataset

| Field | Details |
|---|---|
| Source | WSU Education Abroad office records |
| Time period | 2008–2025 (academic years) |
| Records | ~11,000+ participant entries |
| Key variables | Program type, academic year, major, college, destination country/city, student GPA |

**Note:** Data is not publicly available due to institutional data policy. Analysis outputs and methodology are documented in the notebook.

---

## Methods & Tools

- **Python** (Pandas, Matplotlib) — data cleaning, aggregation, visualization
- **Data cleaning:** Standardized column names, built academic year bins, imputed missing GPA values using global mean, and developed a rule-based major name lookup to map 300+ raw major strings to official WSU program names
- **Analysis:** Descriptive statistics, cross-tabulations, time-series trend analysis, HHI (Herfindahl-Hirschman Index) for regional concentration, equity gap analysis comparing observed vs. expected regional participation by major

---

## Key Findings

### Participation Over Time
- Participation grew steadily from 2008, peaking around **2018–2019** (~800 students/year)
- The **COVID-19 pandemic** caused a collapse in 2021 (36 students), with strong recovery in 2022–2023 (535 → 807)
- Post-pandemic recovery has been anchored by **Faculty-Led and Provider programs** rather than traditional exchanges

### Program Type
- **Faculty-Led** (5,101) and **Provider** (4,149) programs dominate overall participation
- Exchange and NAP/ITR/Direct programs remain a small share across all periods

### Geographic Distribution
- **Italy and Spain** account for the two largest destination volumes (~1,660 and ~1,540 students respectively)
- The program is heavily **Eurocentric**: Europe accounts for 64% of all destinations (2020–2025), while Asia, Latin America, and North America each make up only ~9–10%
- Regional concentration has **increased over time** — the HHI index rose from 0.33 (2008–2013) to 0.44 (2020–2025), indicating less diversity, not more

### Major & Destination Patterns
- Business Administration, Communication, and Hospitality Business Management are the most represented majors
- Italy is a hub for Hospitality and Design/Textiles majors; Spain shows broader major diversity
- Psychology students are underrepresented in Asia; Hospitality and Apparel/Textiles students are underrepresented in Latin America and North America relative to expected shares

### Equity Gaps
- Several majors send **zero students** to certain regions that would be academically relevant (e.g., Accounting → Latin America, Psychology → Asia)
- The Eurocentric concentration contradicts WSU Education Abroad's stated mission of creating **equitable global opportunities for all identities**

---

## Policy Suggestions

Based on the equity gap analysis:
1. **Targeted scholarships** for programs in Asia, Latin America, and Africa
2. **Expand partnerships** beyond Europe, particularly for majors with clear regional alignment
3. **Track destination diversity** by major over time and set measurable diversification goals
4. **Market non-European programs** around their unique academic and cultural value propositions

---

## Repository Structure

```
├── README.md
├── analysis/
│   └── EducationAbroadDataAnalysisProject.ipynb   # Full annotated notebook
└── report/
    └── Education_Abroad_Data_Analysis_Report_Summary.pdf  # Summary report
```

---

## How to View the Analysis

- **On GitHub:** Click into `analysis/EducationAbroadDataAnalysisProject.ipynb` — GitHub renders notebooks directly in the browser, showing code, charts, and narrative together
- **Locally:** Clone the repo and open the `.ipynb` file in Jupyter Notebook or JupyterLab

---

*Analyst: Seohyeon Yoon | August 2025*
