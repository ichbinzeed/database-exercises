# Humai Bootcamp Data Science Portfolio

<p align="center">
	<img src="der_humai.png" alt="Entity Relationship Diagram from SQL practice" width="880"/>
</p>

<p align="center">
	<b>Hands-on exercises from my Humai Data Scientist Bootcamp.</b><br/>
	I am building practical skills to work in a real data team.
</p>

<p align="center">
	<img src="https://img.shields.io/badge/Open%20to%20Work-Junior%20Data%20Roles-1C8C5E" alt="Open to work"/>
	<img src="https://img.shields.io/badge/English-B1%20(learning%20to%20B2)-0057B8" alt="English level"/>
	<img src="https://img.shields.io/badge/Python-Data%20Analysis-3776AB?logo=python&logoColor=white" alt="Python"/>
	<img src="https://img.shields.io/badge/SQL-PostgreSQL%20%7C%20MongoDB-1F6FEB" alt="SQL"/>
	<img src="https://img.shields.io/badge/Ibis-DuckDB%20%2B%20PostgreSQL-F59E0B" alt="Ibis + DuckDB + PostgreSQL"/>
	<img src="https://img.shields.io/badge/Advanced%20SQL-Window%20Functions%20%7C%20CUBE-DC2626" alt="Advanced SQL"/>
	<img src="https://img.shields.io/badge/Code%20Quality-pylint%20%7C%20type%20hints-0A7EA4" alt="Code quality"/>
	<img src="https://img.shields.io/badge/MongoDB-Atlas%20%7C%20PyMongo-00A35C?logo=mongodb&logoColor=white" alt="MongoDB Atlas"/>
</p>

## Advanced SQL + Ibis Spotlight

<p>
  <a href="Avanzadas.ipynb"><img src="https://img.shields.io/badge/Notebook-Avanzadas.ipynb-1D4ED8" alt="Avanzadas notebook"/></a>
  <img src="https://img.shields.io/badge/Database-PostgreSQL-336791?logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/Engine-Ibis%20on%20DuckDB-92400E" alt="Ibis on DuckDB"/>
  <img src="https://img.shields.io/badge/Methods-CTE%20%7C%20Windows%20%7C%20CUBE%20%7C%20Grouping%20Sets-0F766E" alt="Methods"/>
</p>

| What I learned in advanced exercises                        | Why this is useful at work                            |
| ----------------------------------------------------------- | ----------------------------------------------------- |
| CTE and multi-step SQL logic                                | Breaks complex analysis into clear steps              |
| Window functions (`ROW_NUMBER`, `SUM OVER`, moving average) | Builds ranked reports and time trends                 |
| `CUBE` and `GROUPING SETS`                                  | Creates executive summaries with totals and subtotals |
| SQL to Pandas translation                                   | Checks result consistency across tools                |
| Ibis expressions                                            | Writes backend-agnostic analytics code                |
| DuckDB engine reading PostgreSQL                            | Fast local analysis without copying full data         |

<details>
  <summary><b>Advanced workflow I can now do</b></summary>

1. Connect to PostgreSQL and validate schema/tables.
2. Build a business query in SQL with CTE + windows.
3. Rebuild the same logic in Pandas and Ibis for validation.
4. Compare outputs and explain differences.
5. Deliver a final, ordered table for decision makers.
</details>

## MongoDB Exercises Spotlight

<p>
  <a href="MongoEx.ipynb"><img src="https://img.shields.io/badge/Notebook-MongoEx.ipynb-2B6CB0" alt="MongoEx notebook"/></a>
  <img src="https://img.shields.io/badge/Connection-Atlas%20with%20.env-0F766E" alt="Atlas connection"/>
  <img src="https://img.shields.io/badge/Operations-CRUD%20%7C%20Filters%20%7C%20Aggregation-7C3AED" alt="Mongo operations"/>
  <img src="https://img.shields.io/badge/Updates-Idempotent%20logic-CA8A04" alt="Idempotent updates"/>
</p>

| What I practiced                   | Real result                                        |
| ---------------------------------- | -------------------------------------------------- |
| Atlas cloud connection from `.env` | Connected and validated with `ping`                |
| CRUD with PyMongo                  | Inserted, updated, deleted, counted documents      |
| Business filters                   | Queries by age, product count, and product name    |
| Advanced update logic              | Fixed `$size` query using `$expr` + `$size`        |
| Safe re-execution                  | Used `$addToSet` to avoid duplicate "Bolso Gratis" |
| Data quality check                 | Aggregation to detect duplicated values in arrays  |

<details>
  <summary><b>MongoDB challenge solved</b></summary>

I found and fixed two common MongoDB issues:

1. Invalid filter with `$size` + `$gte`.
2. Duplicate values after running the same update many times.

Final solution:

- Use `$expr` when comparing array size with operators.
- Use `$addToSet` for idempotent updates.
- Use aggregation to verify no duplicates remain.
</details>

## Why Recruiters Like This Repo

| You can quickly see            | Evidence in this repository                                     |
| ------------------------------ | --------------------------------------------------------------- |
| Real practice, not only theory | Many notebooks and exercises solved end-to-end                  |
| Technical range                | Python, SQL, data wrangling, visualization, API basics          |
| Work habits                    | Git branches, clear commits, quality checks, reproducible setup |

## Core Skills

- Data analysis with Pandas: cleaning, grouping, joins, pivot tables, indexing.
- SQL problem solving: filters, joins, aggregates, date logic, business questions.
- Advanced SQL analytics: CTE, window functions, moving averages, CUBE, grouping sets.
- Data quality mindset: validation, consistency checks, and clean outputs.
- Ibis framework: expression-based analytics with DuckDB engine and PostgreSQL source.
- Python quality practices: pylint, type hints, logging, and simple tests.
- Project workflow: Poetry environments, branch strategy, and merge flow.

## Repository Map

| Folder                | Focus                                                  |
| --------------------- | ------------------------------------------------------ |
| Ciencia de datos      | Wrangling, visualization, pivot/indexing, data quality |
| Desarrollo con Python | CLI, typing, pylint, docs, poetry, logging             |
| Python Avanzado       | OOP, testing, CI basics, concurrency, FastAPI intro    |
| SQL and SQL NEW       | SQL I/II exercises, async tasks, MongoDB intro         |

## Selected Outcomes

- Built SQL datasets and answered business questions with clean queries.
- Solved advanced analytical questions with ranking, cumulative sums, and centered moving averages.
- Connected Ibis (DuckDB engine) to PostgreSQL and queried tables directly from the database.
- Implemented CUBE-style reporting for totals/subtotals and translated it to Pandas/Ibis.
- Created and documented a full ER diagram for relational tables.
- Connected and worked with MongoDB Atlas using secure credentials from `.env`.
- Implemented idempotent MongoDB updates to avoid duplicated array values.
- Improved code readability and maintainability with quality tools.
- Practiced team-like Git flow: branch, push, review, and merge.

## Value for Hiring Teams

<p align="center">
	<img src="https://img.shields.io/badge/Business%20Questions-Translated%20to%20SQL%20logic-0E7490" alt="Business to SQL"/>
	<img src="https://img.shields.io/badge/Validation-SQL%20vs%20Pandas%20vs%20Ibis-7C2D12" alt="Cross validation"/>
	<img src="https://img.shields.io/badge/Delivery-Clean%20tables%20for%20stakeholders-166534" alt="Delivery"/>
</p>

This portfolio shows that I can:

- turn unclear business needs into clear analytical steps,
- write reproducible queries and notebooks,
- validate results with multiple tools,
- and communicate outcomes in a simple way.

## Quick Git Help

For real workflow commands and fixes, check:

- [GIT_CHEATSHEET.md](GIT_CHEATSHEET.md)

## Contact

**Gustavo Nicolas Castellon**

- GitHub: [ichbinzeed](https://github.com/ichbinzeed)
- LinkedIn: [gustavo-nicolas-castellon](https://www.linkedin.com/in/ichbinzeed)
