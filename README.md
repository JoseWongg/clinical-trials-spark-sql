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
├── data/
│   └── clinical_trials.csv         # Dataset
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
- Dataset


## Dataset

This project uses a **clinical trials dataset** (CSV export, 196 MB).  

- The full dataset is included in this repository via [Git LFS](https://git-lfs.com/).  
- When you clone the repository, GitHub automatically manages downloading the large file.  

### Using the dataset in Databricks
1. In Databricks, go to **Data → Create → Add Data → Upload File**.  
2. Upload `data/clinical_trials.csv` from this repository.  
3. Set the target path (e.g., `/FileStore/clinical_trials.csv`).  
4. Load into Spark:  
```
   python
   df = spark.read.option("header", "true").csv("/FileStore/clinical_trials.csv")
   df.show(5)
```

## How to Use
### Option 1: Quick View  
Open the **HTML file** in any web browser to explore the notebook and results.

### Option 2: Run in Databricks  
1. Log in to your Databricks workspace.  
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
