**Spotify ETL using Python and AWS**
--
**Objective:**
> Develop an ETL pipeline using Python and AWS services to obtain the song, artist and album details from the "Top 50 India" playlist on Spotify. This playlist is updated everyday and consists of 50 top songs of india.

###
###
**_Steps involved in the project_**
```
1. The pipeline involves extracting data from the Spotify API using Spotipy python module.
2. Loading data into amazon S3 using EventBridge cron.
3. Transforming the data in S3 bucket (raw_data) with S3 putobject as a trigger and loading it into another s3 bucket (processed).
4. Use AWS Glue Crawlers for cataloging and metadata management (create schema for data stored in processed folder).
5. Run queries and further analysis using AWS Athena on the processed data.
```
###
**_Tools Used_**
> Python, AWS services (CloudWatch, Lambda, S3, Glue and Athena)


Architecture Diagram :
---
![image](https://github.com/si-sa/spotify_aws_etl/assets/24570020/b76b4ff2-2422-4704-821f-2bbc4b411d18)
