
```
[cloudera@quickstart ~]$ sqoop --options-file import_like_home.txt
Warning: /usr/lib/sqoop/../accumulo does not exist! Accumulo imports will fail.
Please set $ACCUMULO_HOME to the root of your Accumulo installation.
25/03/04 15:23:57 INFO sqoop.Sqoop: Running Sqoop version: 1.4.6-cdh5.12.0
25/03/04 15:23:57 WARN tool.BaseSqoopTool: Setting your password on the command-line is insecure. Consider using -P instead.
25/03/04 15:23:58 INFO manager.MySQLManager: Preparing to use a MySQL streaming resultset.
25/03/04 15:23:58 INFO tool.CodeGenTool: Beginning code generation
25/03/04 15:24:00 INFO manager.SqlManager: Executing SQL statement: SELECT * FROM peliculas WHERE titulo LIKE "%home%" AND  (1 = 0) 
25/03/04 15:24:00 INFO manager.SqlManager: Executing SQL statement: SELECT * FROM peliculas WHERE titulo LIKE "%home%" AND  (1 = 0) 
25/03/04 15:24:00 INFO manager.SqlManager: Executing SQL statement: SELECT * FROM peliculas WHERE titulo LIKE "%home%" AND  (1 = 0) 
25/03/04 15:24:00 INFO orm.CompilationManager: HADOOP_MAPRED_HOME is /usr/lib/hadoop-mapreduce
Note: /tmp/sqoop-cloudera/compile/212c25711938a12d722a69df8100743c/QueryResult.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
25/03/04 15:24:08 INFO orm.CompilationManager: Writing jar file: /tmp/sqoop-cloudera/compile/212c25711938a12d722a69df8100743c/QueryResult.jar
25/03/04 15:24:08 INFO mapreduce.ImportJobBase: Beginning query import.
25/03/04 15:24:08 INFO Configuration.deprecation: mapred.job.tracker is deprecated. Instead, use mapreduce.jobtracker.address
25/03/04 15:24:10 INFO Configuration.deprecation: mapred.jar is deprecated. Instead, use mapreduce.job.jar
25/03/04 15:24:10 INFO Configuration.deprecation: mapred.output.value.class is deprecated. Instead, use mapreduce.job.output.value.class
25/03/04 15:24:13 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
25/03/04 15:24:14 INFO client.RMProxy: Connecting to ResourceManager at /0.0.0.0:8032
25/03/04 15:24:21 INFO db.DBInputFormat: Using read commited transaction isolation
25/03/04 15:24:21 INFO db.DataDrivenDBInputFormat: BoundingValsQuery: SELECT MIN(id_pelicula), MAX(id_pelicula) FROM (SELECT * FROM peliculas WHERE titulo LIKE "%home%" AND  (1 = 1) ) AS t1
25/03/04 15:24:21 INFO db.IntegerSplitter: Split size: 820; Num splits: 2 from: 35 to: 1676
25/03/04 15:24:21 INFO mapreduce.JobSubmitter: number of splits:2
25/03/04 15:24:22 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1741125613244_0001
25/03/04 15:24:24 INFO impl.YarnClientImpl: Submitted application application_1741125613244_0001
25/03/04 15:24:24 INFO mapreduce.Job: The url to track the job: http://quickstart.cloudera:8088/proxy/application_1741125613244_0001/
25/03/04 15:24:24 INFO mapreduce.Job: Running job: job_1741125613244_0001
25/03/04 15:25:01 INFO mapreduce.Job: Job job_1741125613244_0001 running in uber mode : false
25/03/04 15:25:01 INFO mapreduce.Job:  map 0% reduce 0%
25/03/04 15:25:24 INFO mapreduce.Job:  map 100% reduce 0%
25/03/04 15:25:26 INFO mapreduce.Job: Job job_1741125613244_0001 completed successfully
25/03/04 15:25:27 INFO mapreduce.Job: Counters: 30
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=303472
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=233
		HDFS: Number of bytes written=840
		HDFS: Number of read operations=8
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=4
	Job Counters 
		Launched map tasks=2
		Other local map tasks=2
		Total time spent by all maps in occupied slots (ms)=38647
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=38647
		Total vcore-milliseconds taken by all map tasks=38647
		Total megabyte-milliseconds taken by all map tasks=39574528
	Map-Reduce Framework
		Map input records=11
		Map output records=11
		Input split bytes=233
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=287
		CPU time spent (ms)=12490
		Physical memory (bytes) snapshot=456908800
		Virtual memory (bytes) snapshot=3189809152
		Total committed heap usage (bytes)=442499072
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=840
25/03/04 15:25:27 INFO mapreduce.ImportJobBase: Transferred 840 bytes in 73.4514 seconds (11.4361 bytes/sec)
25/03/04 15:25:27 INFO mapreduce.ImportJobBase: Retrieved 11 records.

```
