# LCAIM-Graph-case-study-data

This repository contains
- Neo4j case study database 'active.zip' 
- Unintegrated case study datasets 
- Python code for lifecycle analysis + raw data
- Sample queries
- .dump file for running the DB in Neo4j Desktop

# Steps for installing and running the Neo4j graph database locally

- Download and install Neo4j desktop, free 'community edition' from https://neo4j.com/download/ (2025.02.0)
- Unzip and import the 'active.zip' database file 
- Resore with neo4j.dump
- You can then try running some of the queries 

# Steps for reproducing the life cycle cost analysis

- Download and unzip the 'Life Cycle Cost analysis script and input-output data.zip' folder
- Folder contains the following:
  - asset_register.xlsx = the input data for caluations for the case study, extracted from the unified graph database
  - user_input.xlsx = the analysis scope (including timeframe and some economic factors such as 'inflation rate')
  - LCCanalysis_output.xlsx = the resulting data which is returned to the graph database
- Open the 'LCC_demonstrator_V1.5.2_20.3.25.ipynb' Python script and follow the annotated data processing steps

If you encourter any issues, please don't hesitate to reach out to conor.shaw@ucdconnect.ie
