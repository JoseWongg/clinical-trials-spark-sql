# Clinical Trials Analysis with Spark SQL

Exploratory analysis of U.S. clinical trials data using **Apache Spark SQL**.  
The project demonstrates how to query and analyse large healthcare datasets in a distributed environment.  

It focuses on:
- Identifying the most frequent clinical trial types and medical conditions.  
- Calculating the average duration of completed trials.  
- Performing a trend analysis of diabetes-related completed trials over time, with supporting visualisation.  


## Repository Structure
```
clinical-trials-spark-sql/
├── notebooks/
│   ├── ClinicalTrials_SQL.html     # Databricks HTML export (open in browser)
│   └── ClinicalTrials_SQL.dbc      # Databricks archive (import into workspace)
├── docs/
│   └── project_context_clinical_trials.pdf        # Context
├── LICENSE
└── README.md
```

## Notebooks
This project is provided in two formats for convenience:
- **HTML (`.html`)** Open directly in your browser.  
- **Databricks Archive (`.dbc`)** Import into a Databricks workspace.   

## What’s Inside
- Spark SQL queries for:
  - Frequencies by study type and condition  
  - Average trial durations  
  - Yearly trend of completed trials related to diabetes (with visualisation)  
- Clean, well-documented SQL for readability and reproducibility.  
- A concise [project context document](docs/project_context_clinical_trials.pdf) summarising background, objectives, and business value.  


## How to Use
### Option 1: Quick View  
Open the **HTML file** in any web browser to explore the notebook and results.

### Option 2: Run in Databricks  
1. Log into your Databricks workspace.  
2. Import `notebooks/ClinicalTrials_SQL.dbc`.  
3. Run the cells to reproduce the analysis.  

### Clone this repo:  
   ```bash
   git clone https://github.com/JoseWongg/clinical-trials-spark-sql.git
   cd clinical-trials-spark-sql
   ```

## Authorship & Contact
Developed by **Jose Wong**  
j.wong@mail.com  
https://www.linkedin.com/in/jose-wongg  
https://github.com/JoseWongg  

## License
MIT — see the [LICENSE](LICENSE) file for details.
