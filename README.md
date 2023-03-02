# SqoopIncrementalLoad
A real time example to perform Incremental load.


To create a Sqoop job that performs an incremental load for all tables from the "retail" database except "item" and "product" tables and saves them in ORC format to Hive table using last modified time as the check column, with no duplicates after each incremental load, updates rows in Hive tables if there are any changes in the source table, and reflects any inserts or deletions made in the source table in the Hive tables.


Note that the command imports data only for one table at a time. You can repeat the same command for each table you want to import. Additionally, you can automate this process using a script that runs the command for each table and schedules the script to run at a specific time interval using cron or another scheduling tool.
