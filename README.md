[PORTFOLIO_README_unificado.md](https://github.com/user-attachments/files/32870059/PORTFOLIO_README_unificado.md)

#<img width="1280" height="640" alt="repository-open-graph-template (1)" src="https://github.com/user-attachments/assets/d1994a25-bf22-4db0-815b-4d7b5d79a190" />


# Facundo Gastón Sasso

### Data & Research Analyst · Social & Urban Research

**Sociologist (UBA) working at the intersection of data analysis, social research and urban studies.**

I use quantitative and qualitative data to investigate how social inequalities are produced, distributed and experienced across urban space.

---

## About this portfolio

This repository brings together research projects developed from a common perspective:

> **Data analysis as a tool for understanding social and urban problems.**

The projects combine statistical analysis, spatial data, qualitative research and reproducible workflows. Rather than treating data analysis and sociological research as separate practices, I use programming and research methods together to move from empirical evidence to interpretable findings.

### Research interests

`Urban inequalities` · `Housing` · `Territory` · `Care` · `Mobility` · `Social networks` · `Housing markets` · `Qualitative research`

---

## Selected projects

| Project | Approach | Main question | Tools |
|---|---|---|---|
| 🏠 **Rental Prices and Income Inequality in Buenos Aires City** | Quantitative + spatial | Do rental prices follow the spatial distribution of income across Buenos Aires City's communes? | Python · Pandas · GeoPandas · Matplotlib · Seaborn · Plotly |
| 🏘️ **Villa Itatí — Modos de habitar, movilidades y sociabilidades** | Qualitative data analysis + urban research | How can everyday mobility, social networks and expectations of permanence be articulated in different ways of inhabiting Villa Itatí? | Python · Pandas · Matplotlib · Jupyter · qualitative coding |

---

# 01 · Rental Prices and Income Inequality in Buenos Aires City

### Quantitative & spatial analysis

**Research question**

> Do rental prices follow the spatial distribution of income across Buenos Aires City's communes?

This project examines the spatial association between **average family per-capita income** and **average rental prices** across Buenos Aires City's communes.

### Data

- **EAH 2023** — Buenos Aires City Household Survey
- **Rental prices 2018–2019** — historical rental-price data by commune
- **Commune geometries** — spatial data for Buenos Aires City

The temporal mismatch between the income and rental datasets is central to the interpretation. Therefore, the project studies **spatial association**, not current housing affordability.

### Analytical workflow

```text
Raw data
   ↓
Cleaning & filtering
   ↓
Aggregation by commune
   ↓
Descriptive statistics
   ↓
Pearson correlation
   ↓
Spatial data integration
   ↓
Maps & visualizations
   ↓
Interpretation
```

### Main result

The exploratory analysis found a **Pearson correlation of r = 0.87** between average family per-capita income and average rental prices across the communes for which rental data were available.

This indicates a strong positive spatial association in the observed data, while the temporal mismatch prevents interpreting the result as a contemporaneous measure of housing affordability.

### Skills demonstrated

`Python` `Pandas` `GeoPandas` `Matplotlib` `Seaborn` `Plotly` `EDA` `Pearson correlation` `data aggregation` `spatial analysis` `data visualization` `reproducible research`

**[→ Open project](./rental_income_caba_portfolio/)**

---

# 02 · Villa Itatí — Modos de habitar, movilidades y sociabilidades

### Qualitative data analysis applied to urban research

**Research question**

> How can everyday mobility, social networks and expectations of permanence be articulated in different ways of inhabiting Villa Itatí?

This project translates qualitative research material into a structured analytical dataset while preserving the conceptual categories developed through the original sociological research.

### Research context

- **Case:** Villa Itatí, Quilmes, Buenos Aires
- **Fieldwork:** 2024
- **Origin:** Sociology research at UBA
- **Analytical cases:** 8 selected interview cases
- **Method:** semi-structured interviews + qualitative coding + analytical grid

### From interviews to data

```text
Qualitative interviews
        ↓
Coding / analytical grid
        ↓
Conceptual categories
        ↓
Master dataset
        ↓
Python + Pandas
        ↓
EDA + cross-tabulation
        ↓
Visualization
        ↓
Sociological interpretation
```

The dataset organizes dimensions including:

- everyday mobility
- social networks and sociabilities
- expectations of permanence
- representations of self and neighborhood
- territorial representations
- states of mobility
- care as a transversal analytical dimension

### Analytical insight

The cases show different articulations between mobility, community ties, expectations and representations of the neighborhood.

Care and proximity networks can provide support and enable forms of action while existing alongside territorial fragmentation and institutional distance. The project therefore treats **ways of inhabiting as a multidimensional object**, rather than reducing them to residential location or physical mobility alone.

### Skills demonstrated

`Python` `Pandas` `NumPy` `Matplotlib` `Jupyter` `EDA` `categorical data` `cross-tabulation` `qualitative coding` `data modeling` `data provenance` `urban sociology` `research ethics`

**[→ Open project](./itati-modos-de-habitar/)**

---

# What connects both projects?

The two projects use different types of evidence, but follow a similar analytical logic:

```text
                 SOCIAL / URBAN PROBLEM
                           │
                           ▼
                    RESEARCH QUESTION
                           │
              ┌────────────┴────────────┐
              ▼                         ▼
       QUANTITATIVE DATA         QUALITATIVE DATA
              │                         │
              ▼                         ▼
       Cleaning & EDA            Coding & structuring
              │                         │
              ▼                         ▼
       Statistical / GIS          Categorical analysis
          analysis                       │
              │                         │
              └────────────┬────────────┘
                           ▼
                  VISUALIZATION
                           │
                           ▼
                 SOCIOLOGICAL ANALYSIS
                           │
                           ▼
                    INTERPRETABLE
                       FINDINGS
```

This is the core of my approach: **using data analysis not as an end in itself, but as part of a research process.**

---

## Technical toolkit

### Data analysis

`Python` · `Pandas` · `NumPy` · `Jupyter Notebook`

### Statistics & EDA

`Descriptive statistics` · `Pearson correlation` · `Cross-tabulation` · `Categorical data` · `Data cleaning` · `Aggregation`

### Spatial analysis

`GeoPandas` · `Spatial data integration` · `Choropleth mapping` · `Urban spatial analysis`

### Visualization

`Matplotlib` · `Seaborn` · `Plotly`

### Research methods

`Qualitative coding` · `Semi-structured interviews` · `Case study research` · `Operationalization` · `Data provenance` · `Research ethics`

---

## What I am building

My portfolio is focused on developing a profile as a:

### **Data & Research Analyst specialized in social and urban research**

with an emphasis on:

- translating research questions into analytical workflows
- working with structured and unstructured social data
- combining quantitative and qualitative evidence
- analyzing spatial inequalities
- building reproducible research pipelines
- communicating findings through clear visualizations
- documenting methodological decisions and limitations

---

## Repository structure

```text
PORTFOLIO/
│
├── README.md
│
├── rental_income_caba_portfolio/
│   ├── rental_income_caba.ipynb
│   ├── README.md
│   ├── requirements.txt
│   └── data/
│
└── itati-modos-de-habitar/
    ├── README.md
    ├── data/
    ├── notebooks/
    ├── outputs/
    ├── docs/
    ├── requirements.txt
    └── .gitignore
```

---

## Data ethics & research practice

Research involving people requires particular attention to data provenance, privacy and contextual interpretation.

The Villa Itatí project therefore does **not** publish raw interview transcripts, names, exact addresses or sensitive personal information. Public-facing datasets use anonymized identifiers and document which variables have and have not yet been incorporated into the analytical matrix.

The quantitative housing project likewise documents its main temporal limitation rather than presenting historical rental data as a current affordability measure.

For me, reproducibility includes not only code, but also **transparent documentation of what the data can and cannot support**.

---

## About me

**Facundo Gastón Sasso**  
Sociologist — Universidad de Buenos Aires (UBA)

Research interests: social research · urban studies · territorial inequalities · housing · care · mobility · data analysis

📍 Buenos Aires, Argentina

---

### Portfolio status

This repository is an evolving portfolio. New projects will expand the technical range toward SQL, dashboards, automation and additional spatial and statistical analysis while maintaining the same research-oriented approach.
