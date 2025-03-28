# LCAIM-Graph-case-study-data

This repository contains
- Neo4j case study database 'active.zip'. This is the original DB in Neo4j Community Edition version 3.5.25
- Neo4j case study database 'Neo.dump'. This is the DB updated to run in Neo4j Desktop version 1.6.1
- Unintegrated case study datasets 
- Python code for lifecycle analysis + raw data
- Sample queries

# Steps for installing and running the Neo4j graph database locally using Neo4j Desktop

- Download and install Neo4j Desktop from https://neo4j.com/download/ and install by following requirements.
- Run Neo4j Desktop 
- Create a project. Click the "+Add" button and add a File (3rd option in dropdown menu). Select "neo4j.dump" to add this file to the Project.
- When Neo4j.dump is added to the project you can select it. Click on the three horizontal dots and select "Create new DBMS from dump" from the dropdown to rebuild the DB. You can provide any name and password you wish (passwords have a minimum length of 8 characters).
- Once the DB is rebuilt, you can select it. A side window will open. Go to the second tab (Plugins) and select "APOC". Click "Install and restart" if the APOC procedures are not installed.
- After restarting Neo4j it will automatically open your project. You are now ready to run the database by selecting it and then clicking "Start".
- Once the DB is started, you have various options to open it. If you wish to run the queries, select the Database and open the Neo4j Browser by clicking "Open"
- You can also use other options like Neo4j Bloom for better visualisation of the datastructure.

# Steps for installing and running the Neo4j graph database locally using Neo4j Community Edition Server

- - Download Neo4j, free 'community edition' from https://neo4j.com/download-thanks/?edition=community&release=3.5.25&flavour=winzip (3.5.25)
- Unzip the folder to a location of your choice. The Neo4j server will launch from that location.
- Unzip 'active.zip'. Put the resulting database folder "graph.db" database file in YOUR_PATH/neo4j-community-3.5.25/data/databases 
- Put "Neo4j console start.bat" in the folder YOUR_PATH/neo4j-community-3.5.25
- Open the file using a text editor. change the line "cd YOUR_PATH/neo4j-community-3.5.25" to match your path. Save and close the file
- You can now run Neo4j by double clicking the .bat file.
- You can then try running some of the queries

# Steps for reproducing the life cycle cost analysis

- Download and unzip the 'Life Cycle Cost analysis script and input-output data.zip' folder
- Folder contains the following:
  - asset_register.xlsx = the input data for caluations for the case study, extracted from the unified graph database
  - user_input.xlsx = the analysis scope (including timeframe and some economic factors such as 'inflation rate')
  - LCCanalysis_output.xlsx = the resulting data which is returned to 'enrich' the graph database
- Open the 'LCC_demonstrator_V1.5.2_20.3.25.ipynb' Python script and follow the annotated data processing steps

If you encourter any issues, please don't hesitate to reach out to conor.shaw@ucdconnect.ie
