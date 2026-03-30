# Chicago Urban Data Analysis

An end-to-end SQL-based analysis of Chicago's urban landscape, exploring the relationships between crime patterns, public school performance, and community-level socioeconomic hardship using three real-world datasets from the City of Chicago Data Portal.

---

## Project Notebooks

| Notebook | Focus |
|----------|-------|
| [`01_school_analysis.ipynb`](01_school_analysis.ipynb) | School performance: attendance, safety scores, and college enrollment across community areas |
| [`02_crime_census_analysis.ipynb`](02_crime_census_analysis.ipynb) | Crime patterns, poverty, and hardship — with cross-dataset analysis linking all three datasets |

---

## Key Questions Explored

- Which Chicago community areas have the lowest college enrollment, and how do they compare socioeconomically?
- Which schools have critically low attendance rates (below 70%), and where are they located?
- What types of crimes occur at school locations, and how safe are different school types?
- Which community areas are most crime-prone, and do they overlap with the highest poverty and hardship areas?
- Is there a measurable correlation between a community's hardship index and its crime rate?

---

## Datasets

| Dataset | Period | Source |
|---------|--------|--------|
| Chicago Public Schools Progress Report Cards | 2011–2012 | [Chicago Data Portal](https://data.cityofchicago.org/Education/Chicago-Public-Schools-Progress-Report-Cards-2011-/9xs2-f89t) |
| Socioeconomic Indicators (Census Data) | 2008–2012 | [Chicago Data Portal](https://data.cityofchicago.org/Health-Human-Services/Census-Data-Selected-socioeconomic-indicators-in-C/kn9c-c2s2) |
| Chicago Crime Data | 2001–present | [Chicago Data Portal](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-present/ijzp-q8t2) |

---

## Key Findings

- **Crime is geographically concentrated** — a small number of community areas account for a disproportionate share of all recorded crimes.
- **High hardship = high crime** — the most crime-prone community areas consistently overlap with those carrying the highest hardship index scores and poverty rates.
- **School safety gap** — High schools average lower safety scores than elementary schools, reflecting broader urban adolescent safety challenges.
- **Attendance crisis** — Several schools recorded average attendance below 70%, a strong indicator of systemic disengagement.
- **Enrollment inequality** — Community areas with low college enrollment tend to cluster in economically disadvantaged neighborhoods, highlighting a clear link between poverty and educational opportunity.

---

## Technologies Used

- **Python 3.8+**
- `sqlite3` — Local relational database
- `pandas` — Data ingestion and transformation
- `ipython-sql` — Inline SQL magic for Jupyter Notebooks
- `prettytable` — Formatted query output

---

## Getting Started

```bash
# Clone the repository
git clone https://github.com/your-username/chicago-urban-data-analysis.git
cd chicago-urban-data-analysis

# Install dependencies
pip install pandas ipython-sql prettytable

# Launch Jupyter
jupyter notebook
```

Open the notebooks in order. The `.db` files are included — no separate database setup required.

---

## SQL Concepts Demonstrated

- `WHERE`, `LIKE`, `DISTINCT` for filtering and pattern matching
- `COUNT`, `SUM`, `AVG`, `MAX`, `ROUND` for aggregation
- `GROUP BY`, `ORDER BY`, `LIMIT` for ranking and pagination
- `REPLACE()` and `CAST()` for string-to-numeric conversion
- Correlated subqueries for cross-table lookups
- `JOIN` and `LEFT JOIN` for multi-table analysis
- SQLite system catalog inspection (`sqlite_master`, `PRAGMA_TABLE_INFO`)
