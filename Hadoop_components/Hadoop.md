#   Stages in Data Analytics

*   Identify problem
*   Design data requirement
*   Pre-processing data
*   Performing Analytics
*   Visual data


#   Secondary NameNode

*   Metadata - contain all info about modification of data

*   Metadata are maintain by two files
    *   1) editlog.      
    *   2) fsImages

###   FSIMAGES:
*    Contain all modification done on cluster till namenode started
*   Stored in local disk

### EditLogs
*   Contain the recent changes on cluster
*   Stored in RAM

        Checkpointing is process of combining edit logs with fsimages

        Note -> Secondary name node has responsibility and has same copy of edit files and fsImages

        Combines boh files to make a new (FSIMAGE)


*   Check point occur in default 1 hour

