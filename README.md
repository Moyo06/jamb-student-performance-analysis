# What Relates to JAMB Scores? An Exploratory Analysis of 5,000 Students

An exploratory data analysis (EDA) project investigating how study habits, school characteristics, socioeconomic status, and other student factors relate to JAMB scores in a dataset labelled **“Jamb result - 2024.”**

## Research questions

- Are weekly study hours associated with JAMB scores?
- How do scores compare for students with and without extra tutorials?
- Do average scores differ by school type?
- How do scores vary across socioeconomic groups?
- Are urban and rural students' scores different?
- Which numeric variables have the strongest correlations with JAMB scores?

## Current findings

The following figures are reported by the exploratory notebook and should be interpreted as descriptive results for the dataset analysed:

| Analysis | Reported result |
|---|---|
| Study hours | Moderate positive correlation with score (**r = 0.42**) |
| Extra tutorials | Mean score of **177.0** with tutorials vs **170.6** without |
| School type | Mean score of **181.2** for private-school students vs **171.7** for public-school students |
| Socioeconomic status | Mean scores: **164.8** (Low), **174.1** (Medium), **190.7** (High) |
| School location | Mean scores of **175.2** (Urban) and **172.5** (Rural) |
| Other numeric associations | Teacher quality (**r = 0.30**), attendance (**r = 0.28**), assignments completed (**r = 0.28**) |

These patterns do **not** establish causation. Differences may reflect other factors, including access to learning resources, study conditions, school selection, and family circumstances. Group overlap and statistical uncertainty should be examined before drawing stronger conclusions.

## Tools

- Python
- pandas
- Matplotlib
- Seaborn
- VS Code

## Repository structure

```text
jamb-performance-portfolio/
├── data/
│   └── README.md
├── notebooks/
│   └── jamb_student_performance_analysis.ipynb
├── reports/
│   └── figures/
├── .gitignore
├── requirements.txt
└── README.md
```


## Data quality and limitations

- The notebook reports **891 missing values** in `Parent_Education_Level` out of 5,000 records.
- The current analysis fills those missing values with the mode (`Secondary`). This can overstate the prevalence of that category; consider an `Unknown` category and a sensitivity check.
- Verify duplicate records, valid score ranges, category consistency, and missingness patterns.
- Correlation is not causation.
- Group means alone do not show whether differences are statistically meaningful. Consider confidence intervals and suitable statistical tests.
- Confirm the dataset's provenance, collection method, definitions, and representativeness before generalizing to JAMB candidates in Nigeria.


## Author

**Moyosore Iyanda**  
B.Sc. Data Science student, Pan-Atlantic University

This project is an educational exploratory analysis. Findings are limited to the dataset and methods used.
