## Data Ingestion Workflow

1. constants (All hardcoded constants for the project)
2. configuration->mongo_db_connection.py (For DB connection)
3. data_access->usvisa_data.py (For data access and convert data to pandas data frame)
4. entity->config_entity.py-All data classes specific to each component
5. entity->artifact_entity.py-To store return values for each entity: Ex for Data ingestion it stores the train and test data path
6. components->data_ingestion.py->Get data from DB to Df store in feature store, split data into train and test and store them
7. Pipeline
8. Demo.py->call pipeline
10. Push after configuring Github with AWS
