## End to End Weather API Pipeline with Future Forecasting and logging functionality in Databricks and PySpark

The weather data for 5 cities are extracted every hour using OpenWeather API. The data for future hours are predicted using previous 4 hours and when the actual data arrives, the predicted data is replaced with actual data in the fact table.

Dimension tables
* Cities
* Date
* Time

Fact table
* Weather Data

Log table
* Every update to the fact or dimensional tables are added to the log table entry. The log table is implemented with the concept of decorator.

