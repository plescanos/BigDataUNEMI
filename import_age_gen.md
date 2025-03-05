```[cloudera@quickstart ~]$ sqoop --options-file import_age_gen.txt
Warning: /usr/lib/sqoop/../accumulo does not exist! Accumulo imports will fail.
Please set $ACCUMULO_HOME to the root of your Accumulo installation.
25/03/04 17:03:35 INFO sqoop.Sqoop: Running Sqoop version: 1.4.6-cdh5.12.0
25/03/04 17:03:35 WARN tool.BaseSqoopTool: Setting your password on the command-line is insecure. Consider using -P instead.
25/03/04 17:03:36 INFO manager.MySQLManager: Preparing to use a MySQL streaming resultset.
25/03/04 17:03:36 INFO tool.CodeGenTool: Beginning code generation
25/03/04 17:03:38 INFO manager.SqlManager: Executing SQL statement: SELECT edad, genero FROM usuarios WHERE  (1 = 0) 
25/03/04 17:03:38 INFO manager.SqlManager: Executing SQL statement: SELECT edad, genero FROM usuarios WHERE  (1 = 0) 
25/03/04 17:03:38 INFO manager.SqlManager: Executing SQL statement: SELECT edad, genero FROM usuarios WHERE  (1 = 0) 
25/03/04 17:03:38 INFO orm.CompilationManager: HADOOP_MAPRED_HOME is /usr/lib/hadoop-mapreduce
Note: /tmp/sqoop-cloudera/compile/dcb544972f54446ebbf5cce39d76559b/QueryResult.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
25/03/04 17:03:46 INFO orm.CompilationManager: Writing jar file: /tmp/sqoop-cloudera/compile/dcb544972f54446ebbf5cce39d76559b/QueryResult.jar
25/03/04 17:03:46 INFO mapreduce.ImportJobBase: Beginning query import.
25/03/04 17:03:46 INFO Configuration.deprecation: mapred.job.tracker is deprecated. Instead, use mapreduce.jobtracker.address
25/03/04 17:03:48 INFO Configuration.deprecation: mapred.jar is deprecated. Instead, use mapreduce.job.jar
25/03/04 17:03:51 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
25/03/04 17:03:52 INFO client.RMProxy: Connecting to ResourceManager at /0.0.0.0:8032
25/03/04 17:03:58 INFO db.DBInputFormat: Using read commited transaction isolation
25/03/04 17:03:58 INFO mapreduce.JobSubmitter: number of splits:1
25/03/04 17:03:59 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1741125613244_0004
25/03/04 17:04:01 INFO impl.YarnClientImpl: Submitted application application_1741125613244_0004
25/03/04 17:04:01 INFO mapreduce.Job: The url to track the job: http://quickstart.cloudera:8088/proxy/application_1741125613244_0004/
25/03/04 17:04:01 INFO mapreduce.Job: Running job: job_1741125613244_0004
25/03/04 17:04:27 INFO mapreduce.Job: Job job_1741125613244_0004 running in uber mode : false
25/03/04 17:04:27 INFO mapreduce.Job:  map 0% reduce 0%
25/03/04 17:04:48 INFO mapreduce.Job:  map 100% reduce 0%
25/03/04 17:04:49 INFO mapreduce.Job: Job job_1741125613244_0004 completed successfully
25/03/04 17:04:50 INFO mapreduce.Job: Counters: 30
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=151273
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=87
		HDFS: Number of bytes written=4714
		HDFS: Number of read operations=4
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=2
	Job Counters 
		Launched map tasks=1
		Other local map tasks=1
		Total time spent by all maps in occupied slots (ms)=17589
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=17589
		Total vcore-milliseconds taken by all map tasks=17589
		Total megabyte-milliseconds taken by all map tasks=18011136
	Map-Reduce Framework
		Map input records=943
		Map output records=943
		Input split bytes=87
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=415
		CPU time spent (ms)=5680
		Physical memory (bytes) snapshot=226246656
		Virtual memory (bytes) snapshot=1597276160
		Total committed heap usage (bytes)=221249536
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=4714
25/03/04 17:04:50 INFO mapreduce.ImportJobBase: Transferred 4.6035 KB in 58.7516 seconds (80.2362 bytes/sec)
25/03/04 17:04:50 INFO mapreduce.ImportJobBase: Retrieved 943 records.


```
