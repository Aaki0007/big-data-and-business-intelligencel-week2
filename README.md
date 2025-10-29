# Session 2 — Big Data and Business Intelligence

This repository contains the materials for **Session 2** of *Big Data and Business Intelligence*.  
- Slides: see [`slides/`](./slides/) folder  
- Notebooks: see [`notebooks/`](./notebooks/) folder 
---

## Session Outline
#### Recap of Week 1
- Reviewed data lifecycles, data warehouses, and data lakes.  
- Discussed BI and KPIs as bridges between data and decision-making.  
- Worked with the *PeopleSuN* electrification dataset (Harvard Dataverse).  

#### Presentations
- Short student presentations (~4 min + Q&A).  
- Each student shared early findings from the *PeopleSuN* dataset.

#### Choosing a Dataset
- Reviewed where to find high-quality open data:
  - **Harvard Dataverse**, **Kaggle**, **Zindi**, **World Bank Open Data**, **OpenStreetMap**, **government portals**.
- Each student/team selected one dataset and described:
  - **Topic** (e.g., Energy, Health, Education, Mobility…)  
  - **Research Question** they aim to explore.

#### Designing KPIs
- Defined what makes a good KPI (measurable, relevant, interpretable).  
- Drafted 2–3 KPI formulas in plain language and Python notation.  
- Discussed real examples:
  - *US Population Dashboard*
  - *Superstore Sales Dashboard*
  - *Ireland Gender Pay Gap Dashboard*

#### Exploratory Data Analysis (EDA)
- Introduced EDA as the process of **getting to know your data**.  
- Covered:
  - Inspecting structure (`df.info()`, `df.head()`)  
  - Descriptive statistics (`df.describe()`, `value_counts()`)  
  - Missingness and duplicates awareness  
  - Univariate & bivariate visualization  
  - Correlation and time-trend exploration  
- Emphasized combining **quantitative** and **visual** exploration.

#### Hands-On Notebook
- Notebook covers:
  - Data loading and type inspection  
  - Descriptive summaries  
  - Missing value exploration  
  - Univariate and categorical plots  
  - Bivariate relationships  
  - Correlation matrix (continuous variables only)  
  - Regional summaries (average values by *zone*, *state*, etc.)  
  - Markdown reflections and KPI drafts  

#### Homework
- Perform an appropriate level of EDA on your **chosen dataset**.  
- Summarize insights and 2–3 KPI ideas in **a short 5-minute presentation** for Session 3.  


---
## 🚀 Environment Setup

Before starting, please **fork this repository** and create a fresh Python virtual environment.  
All required libraries are listed in `requirements.txt`.

> ⚠️ If you encounter errors during `pip install`, try removing the version pinning for the failing package(s) in `requirements.txt`.  
> On Apple M1/M2 systems you may also need to install additional system packages (the “M1 shizzle”).

---

### macOS / Linux (bash/zsh)

```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate

# Upgrade pip and install dependencies
pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (PowerShell)
```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
.venv\Scripts\Activate.ps1

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (Git Bash)
```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/Scripts/activate

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

You’re now ready to run the session notebooks!

Deactivate the environment when you’re done:
```bash
deactivate
```
