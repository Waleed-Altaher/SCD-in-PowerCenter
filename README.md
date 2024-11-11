# SCD-in-PowerCenter
This is a task for manually implement Slowly Changing Dimension concept in Informatica PowerCenter


## Mapping In Use: 
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://youtu.be/vt5fpE0bzSY)


## Transformations and Step-by-Step 

🔹 Source Qualifier (SQ): Extracts data from the source while filtering out unnecessary rows, ensuring only relevant data enters the ETL pipeline.

🔹 Lookup Transformation (LKP): Checks for existing records to identify if the incoming row is a new record or an update—essential for managing historical data accurately.

🔹 Router Transformation (RTR): Routes rows based on conditions (e.g., new vs. updated records) to handle inserts and updates separately, improving data flow efficiency.

🔹 Sequence Generator (SEQ): Generates unique keys for new records, crucial for maintaining primary keys in slowly changing dimensions.

🔹 Update Strategy (UPD): Specifies whether a record should be inserted or updated in the target, ensuring accurate versioning in SCD T2.

🔹 Expression Transformation (EXP): Used to perform calculations and modify data fields before loading—this helps format and standardize data based on requirements.
