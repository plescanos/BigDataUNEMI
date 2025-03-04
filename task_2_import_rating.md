```[cloudera@quickstart ~]$ sqoop --options-file task_2_imp_rating.txt
Warning: /usr/lib/sqoop/../accumulo does not exist! Accumulo imports will fail.
Please set $ACCUMULO_HOME to the root of your Accumulo installation.
25/03/04 08:32:07 INFO sqoop.Sqoop: Running Sqoop version: 1.4.6-cdh5.12.0
25/03/04 08:32:07 WARN tool.BaseSqoopTool: Setting your password on the command-line is insecure. Consider using -P instead.
25/03/04 08:32:08 INFO manager.MySQLManager: Preparing to use a MySQL streaming resultset.
25/03/04 08:32:08 INFO tool.CodeGenTool: Beginning code generation
25/03/04 08:32:10 INFO manager.SqlManager: Executing SQL statement: SELECT t.* FROM `ratings` AS t LIMIT 1
25/03/04 08:32:10 INFO manager.SqlManager: Executing SQL statement: SELECT t.* FROM `ratings` AS t LIMIT 1
25/03/04 08:32:10 INFO orm.CompilationManager: HADOOP_MAPRED_HOME is /usr/lib/hadoop-mapreduce
Note: /tmp/sqoop-cloudera/compile/b1460ff95c55b3262c5e1e1416745bfa/ratings.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
25/03/04 08:32:19 INFO orm.CompilationManager: Writing jar file: /tmp/sqoop-cloudera/compile/b1460ff95c55b3262c5e1e1416745bfa/ratings.jar
25/03/04 08:32:19 WARN manager.MySQLManager: It looks like you are importing from mysql.
25/03/04 08:32:19 WARN manager.MySQLManager: This transfer can be faster! Use the --direct
25/03/04 08:32:19 WARN manager.MySQLManager: option to exercise a MySQL-specific fast path.
25/03/04 08:32:19 INFO manager.MySQLManager: Setting zero DATETIME behavior to convertToNull (mysql)
25/03/04 08:32:19 INFO mapreduce.ImportJobBase: Beginning import of ratings
25/03/04 08:32:19 INFO Configuration.deprecation: mapred.job.tracker is deprecated. Instead, use mapreduce.jobtracker.address
25/03/04 08:32:20 INFO Configuration.deprecation: mapred.jar is deprecated. Instead, use mapreduce.job.jar
25/03/04 08:32:20 INFO Configuration.deprecation: mapred.output.value.class is deprecated. Instead, use mapreduce.job.output.value.class
25/03/04 08:32:24 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
25/03/04 08:32:24 INFO client.RMProxy: Connecting to ResourceManager at /0.0.0.0:8032
25/03/04 08:32:31 INFO db.DBInputFormat: Using read commited transaction isolation
25/03/04 08:32:31 INFO db.DataDrivenDBInputFormat: BoundingValsQuery: SELECT MIN(`id_rating`), MAX(`id_rating`) FROM `ratings`
25/03/04 08:32:31 INFO db.IntegerSplitter: Split size: 33333; Num splits: 3 from: 1 to: 100000
25/03/04 08:32:31 INFO mapreduce.JobSubmitter: number of splits:3
25/03/04 08:32:32 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1741105356524_0001
25/03/04 08:32:34 INFO impl.YarnClientImpl: Submitted application application_1741105356524_0001
25/03/04 08:32:34 INFO mapreduce.Job: The url to track the job: http://quickstart.cloudera:8088/proxy/application_1741105356524_0001/
25/03/04 08:32:34 INFO mapreduce.Job: Running job: job_1741105356524_0001
25/03/04 08:33:08 INFO mapreduce.Job: Job job_1741105356524_0001 running in uber mode : false
25/03/04 08:33:08 INFO mapreduce.Job:  map 0% reduce 0%
25/03/04 08:33:36 INFO mapreduce.Job:  map 67% reduce 0%
25/03/04 08:33:39 INFO mapreduce.Job:  map 100% reduce 0%
25/03/04 08:33:40 INFO mapreduce.Job: Job job_1741105356524_0001 completed successfully
25/03/04 08:33:42 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=454923
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=358
		HDFS: Number of bytes written=2372758
		HDFS: Number of read operations=12
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=6
	Job Counters 
		Killed map tasks=1
		Launched map tasks=3
		Other local map tasks=3
		Total time spent by all maps in occupied slots (ms)=78197
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=78197
		Total vcore-milliseconds taken by all map tasks=78197
		Total megabyte-milliseconds taken by all map tasks=80073728
	Map-Reduce Framework
		Map input records=100000
		Map output records=100000
		Input split bytes=358
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=560
		CPU time spent (ms)=48950
		Physical memory (bytes) snapshot=767209472
		Virtual memory (bytes) snapshot=4804673536
		Total committed heap usage (bytes)=663748608
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=2372758
25/03/04 08:33:42 INFO mapreduce.ImportJobBase: Transferred 2.2628 MB in 78.1481 seconds (29.6507 KB/sec)
25/03/04 08:33:42 INFO mapreduce.ImportJobBase: Retrieved 100000 records.
```

