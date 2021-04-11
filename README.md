# WSUSDBCleaner
The performance of large WSUS deployments will degrade over time if the WSUS database isn't maintained properly. 
The T-SQL script in this article can be run by SQL Server administrators to reindex and defragment WSUS databases. 

# T-SQL script
  This script does basic maintenance tasks on SUSDB:
    1. Identifies indexes that are fragmented, and defragments them. For certain tables, a fill factor is set to improve insert performance.
    2. Updates potentially out-of-date table statistics.
#P.S: It shouldn't be used on WSUS 2.0 databases.
