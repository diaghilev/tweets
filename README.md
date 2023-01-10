## 25 Custom Job Tweets a Day

### Introduction

The purpose of this project is to serve 25 job-related tweets a day with search parameters that are customizable by the user. 

[Image of interface]

### Project Files
- app
    - main.py - The main ETL script.
        - Fetches data from the Twitter API
        - Saves data to a JSONL file
        - Creates a dataset & table in BigQuery
        - Loads the data to BigQuery
    - tweets.jsonl - The JSONL file which stores tweets.
    - apikey.json - Stores Google Cloud credentials (not version controlled)
    - config.ini - Stores Twitter API credentials (not version controlled)

    - (To add: Any additional files such as dbt files, metabase.db , docker.yml etc.)

### Workflow

[Diagram of Workflow]

- **Ingestion** - Python script fetches data from the twitter API and saves to a JSONL file.
- **Transformation** - TBD (Either python or dbt. Format tweets for readability.)
- **Storage** - Python script creates a dataset & table in BigQuery and loads the data there.
- **Serving** - TBD 
- **Orchestration** - TBD
- **Deployment** - ?




