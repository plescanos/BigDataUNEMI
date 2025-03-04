```
 [cloudera@quickstart ~]$ sqoop --options-file import_all.txt
Warning: /usr/lib/sqoop/../accumulo does not exist! Accumulo imports will fail.
Please set $ACCUMULO_HOME to the root of your Accumulo installation.
25/03/04 05:04:42 INFO sqoop.Sqoop: Running Sqoop version: 1.4.6-cdh5.12.0
25/03/04 05:04:43 WARN tool.BaseSqoopTool: Setting your password on the command-line is insecure. Consider using -P instead.
25/03/04 05:04:43 INFO manager.MySQLManager: Preparing to use a MySQL streaming resultset.
25/03/04 05:04:45 INFO tool.CodeGenTool: Beginning code generation
25/03/04 05:04:45 INFO manager.SqlManager: Executing SQL statement: SELECT t.* FROM `generos` AS t LIMIT 1
25/03/04 05:04:46 INFO manager.SqlManager: Executing SQL statement: SELECT t.* FROM `generos` AS t LIMIT 1
25/03/04 05:04:46 INFO orm.CompilationManager: HADOOP_MAPRED_HOME is /usr/lib/hadoop-mapreduce
Note: /tmp/sqoop-cloudera/compile/b69dbc14f99e1c817bf78a992670e57b/generos.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
25/03/04 05:04:54 INFO orm.CompilationManager: Writing jar file: /tmp/sqoop-cloudera/compile/b69dbc14f99e1c817bf78a992670e57b/generos.jar
25/03/04 05:04:54 WARN manager.MySQLManager: It looks like you are importing from mysql.
25/03/04 05:04:54 WARN manager.MySQLManager: This transfer can be faster! Use the --direct
25/03/04 05:04:54 WARN manager.MySQLManager: option to exercise a MySQL-specific fast path.
25/03/04 05:04:54 INFO manager.MySQLManager: Setting zero DATETIME behavior to convertToNull (mysql)
25/03/04 05:04:54 INFO mapreduce.ImportJobBase: Beginning import of generos
25/03/04 05:04:54 INFO Configuration.deprecation: mapred.job.tracker is deprecated. Instead, use mapreduce.jobtracker.address
25/03/04 05:04:55 INFO Configuration.deprecation: mapred.jar is deprecated. Instead, use mapreduce.job.jar
25/03/04 05:04:55 INFO Configuration.deprecation: mapred.output.value.class is deprecated. Instead, use mapreduce.job.output.value.class
25/03/04 05:04:59 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
25/03/04 05:04:59 INFO client.RMProxy: Connecting to ResourceManager at /0.0.0.0:8032
25/03/04 05:05:06 INFO db.DBInputFormat: Using read commited transaction isolation
25/03/04 05:05:06 INFO db.DataDrivenDBInputFormat: BoundingValsQuery: SELECT MIN(`id_genero`), MAX(`id_genero`) FROM `generos`
25/03/04 05:05:06 INFO db.IntegerSplitter: Split size: 4; Num splits: 4 from: 1 to: 18
25/03/04 05:05:07 INFO mapreduce.JobSubmitter: number of splits:4
25/03/04 05:05:07 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1741093063703_0001
25/03/04 05:05:10 INFO impl.YarnClientImpl: Submitted application application_1741093063703_0001
25/03/04 05:05:10 INFO mapreduce.Job: The url to track the job: http://quickstart.cloudera:8088/proxy/application_1741093063703_0001/
25/03/04 05:05:10 INFO mapreduce.Job: Running job: job_1741093063703_0001
25/03/04 05:05:46 INFO mapreduce.Job: Job job_1741093063703_0001 running in uber mode : false
25/03/04 05:05:46 INFO mapreduce.Job:  map 0% reduce 0%
25/03/04 05:06:14 INFO mapreduce.Job:  map 50% reduce 0%
25/03/04 05:06:16 INFO mapreduce.Job:  map 75% reduce 0%
25/03/04 05:06:18 INFO mapreduce.Job:  map 100% reduce 0%
25/03/04 05:06:19 INFO mapreduce.Job: Job job_1741093063703_0001 completed successfully
25/03/04 05:06:19 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=605272
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=454
		HDFS: Number of bytes written=814
		HDFS: Number of read operations=16
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=8
	Job Counters 
		Killed map tasks=1
		Launched map tasks=4
		Other local map tasks=4
		Total time spent by all maps in occupied slots (ms)=107773
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=107773
		Total vcore-milliseconds taken by all map tasks=107773
		Total megabyte-milliseconds taken by all map tasks=110359552
	Map-Reduce Framework
		Map input records=18
		Map output records=18
		Input split bytes=454
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=932
		CPU time spent (ms)=32050
		Physical memory (bytes) snapshot=925859840
		Virtual memory (bytes) snapshot=6379536384
		Total committed heap usage (bytes)=887095296
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=814
25/03/04 05:06:19 INFO mapreduce.ImportJobBase: Transferred 814 bytes in 80.656 seconds (10.0922 bytes/sec)
25/03/04 05:06:19 INFO mapreduce.ImportJobBase: Retrieved 18 records.
25/03/04 05:06:19 INFO tool.CodeGenTool: Beginning code generation
25/03/04 05:06:19 INFO manager.SqlManager: Executing SQL statement: SELECT t.* FROM `generos_peliculas` AS t LIMIT 1
25/03/04 05:06:20 INFO orm.CompilationManager: HADOOP_MAPRED_HOME is /usr/lib/hadoop-mapreduce
Note: /tmp/sqoop-cloudera/compile/b69dbc14f99e1c817bf78a992670e57b/generos_peliculas.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
25/03/04 05:06:21 INFO orm.CompilationManager: Writing jar file: /tmp/sqoop-cloudera/compile/b69dbc14f99e1c817bf78a992670e57b/generos_peliculas.jar
25/03/04 05:06:21 INFO mapreduce.ImportJobBase: Beginning import of generos_peliculas
25/03/04 05:06:21 INFO Configuration.deprecation: mapred.job.tracker is deprecated. Instead, use mapreduce.jobtracker.address
25/03/04 05:06:22 INFO client.RMProxy: Connecting to ResourceManager at /0.0.0.0:8032
25/03/04 05:06:26 INFO db.DBInputFormat: Using read commited transaction isolation
25/03/04 05:06:26 INFO db.DataDrivenDBInputFormat: BoundingValsQuery: SELECT MIN(`id`), MAX(`id`) FROM `generos_peliculas`
25/03/04 05:06:26 INFO db.IntegerSplitter: Split size: 722; Num splits: 4 from: 1 to: 2891
25/03/04 05:06:26 INFO mapreduce.JobSubmitter: number of splits:4
25/03/04 05:06:26 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1741093063703_0002
25/03/04 05:06:27 INFO impl.YarnClientImpl: Submitted application application_1741093063703_0002
25/03/04 05:06:27 INFO mapreduce.Job: The url to track the job: http://quickstart.cloudera:8088/proxy/application_1741093063703_0002/
25/03/04 05:06:27 INFO mapreduce.Job: Running job: job_1741093063703_0002
25/03/04 05:06:54 INFO mapreduce.Job: Job job_1741093063703_0002 running in uber mode : false
25/03/04 05:06:54 INFO mapreduce.Job:  map 0% reduce 0%
25/03/04 05:07:25 INFO mapreduce.Job:  map 50% reduce 0%
25/03/04 05:07:27 INFO mapreduce.Job:  map 75% reduce 0%
25/03/04 05:07:28 INFO mapreduce.Job:  map 100% reduce 0%
25/03/04 05:07:28 INFO mapreduce.Job: Job job_1741093063703_0002 completed successfully
25/03/04 05:07:28 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=605492
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=412
		HDFS: Number of bytes written=90813
		HDFS: Number of read operations=16
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=8
	Job Counters 
		Killed map tasks=1
		Launched map tasks=5
		Other local map tasks=5
		Total time spent by all maps in occupied slots (ms)=113553
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=113553
		Total vcore-milliseconds taken by all map tasks=113553
		Total megabyte-milliseconds taken by all map tasks=116278272
	Map-Reduce Framework
		Map input records=2891
		Map output records=2891
		Input split bytes=412
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=1943
		CPU time spent (ms)=37330
		Physical memory (bytes) snapshot=924246016
		Virtual memory (bytes) snapshot=6388994048
		Total committed heap usage (bytes)=887095296
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=90813
25/03/04 05:07:28 INFO mapreduce.ImportJobBase: Transferred 88.6846 KB in 66.7506 seconds (1.3286 KB/sec)
25/03/04 05:07:28 INFO mapreduce.ImportJobBase: Retrieved 2891 records.
25/03/04 05:07:28 INFO tool.CodeGenTool: Beginning code generation
25/03/04 05:07:28 INFO manager.SqlManager: Executing SQL statement: SELECT t.* FROM `ocupaciones` AS t LIMIT 1
25/03/04 05:07:28 INFO orm.CompilationManager: HADOOP_MAPRED_HOME is /usr/lib/hadoop-mapreduce
Note: /tmp/sqoop-cloudera/compile/b69dbc14f99e1c817bf78a992670e57b/ocupaciones.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
25/03/04 05:07:30 INFO orm.CompilationManager: Writing jar file: /tmp/sqoop-cloudera/compile/b69dbc14f99e1c817bf78a992670e57b/ocupaciones.jar
25/03/04 05:07:30 INFO mapreduce.ImportJobBase: Beginning import of ocupaciones
25/03/04 05:07:30 INFO Configuration.deprecation: mapred.job.tracker is deprecated. Instead, use mapreduce.jobtracker.address
25/03/04 05:07:30 INFO client.RMProxy: Connecting to ResourceManager at /0.0.0.0:8032
25/03/04 05:07:33 INFO db.DBInputFormat: Using read commited transaction isolation
25/03/04 05:07:33 INFO db.DataDrivenDBInputFormat: BoundingValsQuery: SELECT MIN(`id_ocupacion`), MAX(`id_ocupacion`) FROM `ocupaciones`
25/03/04 05:07:33 INFO db.IntegerSplitter: Split size: 5; Num splits: 4 from: 1 to: 21
25/03/04 05:07:33 INFO mapreduce.JobSubmitter: number of splits:4
25/03/04 05:07:33 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1741093063703_0003
25/03/04 05:07:34 INFO impl.YarnClientImpl: Submitted application application_1741093063703_0003
25/03/04 05:07:34 INFO mapreduce.Job: The url to track the job: http://quickstart.cloudera:8088/proxy/application_1741093063703_0003/
25/03/04 05:07:34 INFO mapreduce.Job: Running job: job_1741093063703_0003
25/03/04 05:08:01 INFO mapreduce.Job: Job job_1741093063703_0003 running in uber mode : false
25/03/04 05:08:01 INFO mapreduce.Job:  map 0% reduce 0%
25/03/04 05:08:31 INFO mapreduce.Job:  map 50% reduce 0%
25/03/04 05:08:32 INFO mapreduce.Job:  map 75% reduce 0%
25/03/04 05:08:35 INFO mapreduce.Job:  map 100% reduce 0%
25/03/04 05:08:36 INFO mapreduce.Job: Job job_1741093063703_0003 completed successfully
25/03/04 05:08:36 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=605384
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=478
		HDFS: Number of bytes written=958
		HDFS: Number of read operations=16
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=8
	Job Counters 
		Killed map tasks=1
		Launched map tasks=5
		Other local map tasks=5
		Total time spent by all maps in occupied slots (ms)=111782
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=111782
		Total vcore-milliseconds taken by all map tasks=111782
		Total megabyte-milliseconds taken by all map tasks=114464768
	Map-Reduce Framework
		Map input records=21
		Map output records=21
		Input split bytes=478
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=2027
		CPU time spent (ms)=31500
		Physical memory (bytes) snapshot=968851456
		Virtual memory (bytes) snapshot=6392532992
		Total committed heap usage (bytes)=884998144
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=958
25/03/04 05:08:36 INFO mapreduce.ImportJobBase: Transferred 958 bytes in 65.839 seconds (14.5507 bytes/sec)
25/03/04 05:08:36 INFO mapreduce.ImportJobBase: Retrieved 21 records.
25/03/04 05:08:36 INFO tool.CodeGenTool: Beginning code generation
25/03/04 05:08:36 INFO manager.SqlManager: Executing SQL statement: SELECT t.* FROM `peliculas` AS t LIMIT 1
25/03/04 05:08:36 INFO orm.CompilationManager: HADOOP_MAPRED_HOME is /usr/lib/hadoop-mapreduce
Note: /tmp/sqoop-cloudera/compile/b69dbc14f99e1c817bf78a992670e57b/peliculas.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
25/03/04 05:08:37 INFO orm.CompilationManager: Writing jar file: /tmp/sqoop-cloudera/compile/b69dbc14f99e1c817bf78a992670e57b/peliculas.jar
25/03/04 05:08:37 INFO mapreduce.ImportJobBase: Beginning import of peliculas
25/03/04 05:08:37 INFO Configuration.deprecation: mapred.job.tracker is deprecated. Instead, use mapreduce.jobtracker.address
25/03/04 05:08:38 INFO client.RMProxy: Connecting to ResourceManager at /0.0.0.0:8032
25/03/04 05:08:40 INFO db.DBInputFormat: Using read commited transaction isolation
25/03/04 05:08:40 INFO db.DataDrivenDBInputFormat: BoundingValsQuery: SELECT MIN(`id_pelicula`), MAX(`id_pelicula`) FROM `peliculas`
25/03/04 05:08:40 INFO db.IntegerSplitter: Split size: 420; Num splits: 4 from: 1 to: 1682
25/03/04 05:08:40 INFO mapreduce.JobSubmitter: number of splits:4
25/03/04 05:08:40 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1741093063703_0004
25/03/04 05:08:41 INFO impl.YarnClientImpl: Submitted application application_1741093063703_0004
25/03/04 05:08:41 INFO mapreduce.Job: The url to track the job: http://quickstart.cloudera:8088/proxy/application_1741093063703_0004/
25/03/04 05:08:41 INFO mapreduce.Job: Running job: job_1741093063703_0004
25/03/04 05:09:09 INFO mapreduce.Job: Job job_1741093063703_0004 running in uber mode : false
25/03/04 05:09:09 INFO mapreduce.Job:  map 0% reduce 0%
25/03/04 05:09:39 INFO mapreduce.Job:  map 25% reduce 0%
25/03/04 05:09:40 INFO mapreduce.Job:  map 50% reduce 0%
25/03/04 05:09:41 INFO mapreduce.Job:  map 75% reduce 0%
25/03/04 05:09:42 INFO mapreduce.Job:  map 100% reduce 0%
25/03/04 05:09:42 INFO mapreduce.Job: Job job_1741093063703_0004 completed successfully
25/03/04 05:09:42 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=605416
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=482
		HDFS: Number of bytes written=94447
		HDFS: Number of read operations=16
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=8
	Job Counters 
		Killed map tasks=1
		Launched map tasks=4
		Other local map tasks=4
		Total time spent by all maps in occupied slots (ms)=106733
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=106733
		Total vcore-milliseconds taken by all map tasks=106733
		Total megabyte-milliseconds taken by all map tasks=109294592
	Map-Reduce Framework
		Map input records=1682
		Map output records=1682
		Input split bytes=482
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=834
		CPU time spent (ms)=30090
		Physical memory (bytes) snapshot=952004608
		Virtual memory (bytes) snapshot=6388379648
		Total committed heap usage (bytes)=884998144
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=94447
25/03/04 05:09:42 INFO mapreduce.ImportJobBase: Transferred 92.2334 KB in 64.4476 seconds (1.4311 KB/sec)
25/03/04 05:09:42 INFO mapreduce.ImportJobBase: Retrieved 1682 records.
25/03/04 05:09:42 INFO tool.CodeGenTool: Beginning code generation
25/03/04 05:09:42 INFO manager.SqlManager: Executing SQL statement: SELECT t.* FROM `ratings` AS t LIMIT 1
25/03/04 05:09:42 INFO orm.CompilationManager: HADOOP_MAPRED_HOME is /usr/lib/hadoop-mapreduce
Note: /tmp/sqoop-cloudera/compile/b69dbc14f99e1c817bf78a992670e57b/ratings.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
25/03/04 05:09:45 INFO orm.CompilationManager: Writing jar file: /tmp/sqoop-cloudera/compile/b69dbc14f99e1c817bf78a992670e57b/ratings.jar
25/03/04 05:09:45 INFO mapreduce.ImportJobBase: Beginning import of ratings
25/03/04 05:09:45 INFO Configuration.deprecation: mapred.job.tracker is deprecated. Instead, use mapreduce.jobtracker.address
25/03/04 05:09:45 INFO client.RMProxy: Connecting to ResourceManager at /0.0.0.0:8032
25/03/04 05:09:49 INFO db.DBInputFormat: Using read commited transaction isolation
25/03/04 05:09:49 INFO db.DataDrivenDBInputFormat: BoundingValsQuery: SELECT MIN(`id_rating`), MAX(`id_rating`) FROM `ratings`
25/03/04 05:09:49 INFO db.IntegerSplitter: Split size: 24999; Num splits: 4 from: 1 to: 100000
25/03/04 05:09:49 INFO mapreduce.JobSubmitter: number of splits:4
25/03/04 05:09:49 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1741093063703_0005
25/03/04 05:09:49 INFO impl.YarnClientImpl: Submitted application application_1741093063703_0005
25/03/04 05:09:50 INFO mapreduce.Job: The url to track the job: http://quickstart.cloudera:8088/proxy/application_1741093063703_0005/
25/03/04 05:09:50 INFO mapreduce.Job: Running job: job_1741093063703_0005
25/03/04 05:10:16 INFO mapreduce.Job: Job job_1741093063703_0005 running in uber mode : false
25/03/04 05:10:16 INFO mapreduce.Job:  map 0% reduce 0%
25/03/04 05:10:51 INFO mapreduce.Job:  map 25% reduce 0%
25/03/04 05:10:52 INFO mapreduce.Job:  map 50% reduce 0%
25/03/04 05:10:53 INFO mapreduce.Job:  map 75% reduce 0%
25/03/04 05:10:55 INFO mapreduce.Job:  map 100% reduce 0%
25/03/04 05:10:56 INFO mapreduce.Job: Job job_1741093063703_0005 completed successfully
25/03/04 05:10:56 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=605452
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=478
		HDFS: Number of bytes written=4948992
		HDFS: Number of read operations=16
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=8
	Job Counters 
		Killed map tasks=1
		Launched map tasks=4
		Other local map tasks=4
		Total time spent by all maps in occupied slots (ms)=128526
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=128526
		Total vcore-milliseconds taken by all map tasks=128526
		Total megabyte-milliseconds taken by all map tasks=131610624
	Map-Reduce Framework
		Map input records=100000
		Map output records=100000
		Input split bytes=478
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=792
		CPU time spent (ms)=79620
		Physical memory (bytes) snapshot=1031049216
		Virtual memory (bytes) snapshot=6399217664
		Total committed heap usage (bytes)=884998144
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=4948992
25/03/04 05:10:56 INFO mapreduce.ImportJobBase: Transferred 4.7197 MB in 70.9131 seconds (68.1538 KB/sec)
25/03/04 05:10:56 INFO mapreduce.ImportJobBase: Retrieved 100000 records.
25/03/04 05:10:56 INFO tool.CodeGenTool: Beginning code generation
25/03/04 05:10:56 INFO manager.SqlManager: Executing SQL statement: SELECT t.* FROM `usuarios` AS t LIMIT 1
25/03/04 05:10:56 INFO orm.CompilationManager: HADOOP_MAPRED_HOME is /usr/lib/hadoop-mapreduce
Note: /tmp/sqoop-cloudera/compile/b69dbc14f99e1c817bf78a992670e57b/usuarios.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
25/03/04 05:10:58 INFO orm.CompilationManager: Writing jar file: /tmp/sqoop-cloudera/compile/b69dbc14f99e1c817bf78a992670e57b/usuarios.jar
25/03/04 05:10:58 INFO mapreduce.ImportJobBase: Beginning import of usuarios
25/03/04 05:10:58 INFO Configuration.deprecation: mapred.job.tracker is deprecated. Instead, use mapreduce.jobtracker.address
25/03/04 05:10:58 INFO client.RMProxy: Connecting to ResourceManager at /0.0.0.0:8032
25/03/04 05:11:01 INFO db.DBInputFormat: Using read commited transaction isolation
25/03/04 05:11:01 INFO db.DataDrivenDBInputFormat: BoundingValsQuery: SELECT MIN(`id_usuario`), MAX(`id_usuario`) FROM `usuarios`
25/03/04 05:11:01 INFO db.IntegerSplitter: Split size: 235; Num splits: 4 from: 1 to: 943
25/03/04 05:11:01 INFO mapreduce.JobSubmitter: number of splits:4
25/03/04 05:11:01 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1741093063703_0006
25/03/04 05:11:02 INFO impl.YarnClientImpl: Submitted application application_1741093063703_0006
25/03/04 05:11:02 INFO mapreduce.Job: The url to track the job: http://quickstart.cloudera:8088/proxy/application_1741093063703_0006/
25/03/04 05:11:02 INFO mapreduce.Job: Running job: job_1741093063703_0006
25/03/04 05:11:32 INFO mapreduce.Job: Job job_1741093063703_0006 running in uber mode : false
25/03/04 05:11:32 INFO mapreduce.Job:  map 0% reduce 0%
25/03/04 05:12:05 INFO mapreduce.Job:  map 50% reduce 0%
25/03/04 05:12:06 INFO mapreduce.Job:  map 75% reduce 0%
25/03/04 05:12:09 INFO mapreduce.Job:  map 100% reduce 0%
25/03/04 05:12:09 INFO mapreduce.Job: Job job_1741093063703_0006 completed successfully
25/03/04 05:12:09 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=605460
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=471
		HDFS: Number of bytes written=39259
		HDFS: Number of read operations=16
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=8
	Job Counters 
		Killed map tasks=1
		Launched map tasks=5
		Other local map tasks=5
		Total time spent by all maps in occupied slots (ms)=120045
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=120045
		Total vcore-milliseconds taken by all map tasks=120045
		Total megabyte-milliseconds taken by all map tasks=122926080
	Map-Reduce Framework
		Map input records=943
		Map output records=943
		Input split bytes=471
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=942
		CPU time spent (ms)=33940
		Physical memory (bytes) snapshot=920129536
		Virtual memory (bytes) snapshot=6392893440
		Total committed heap usage (bytes)=887095296
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=39259
25/03/04 05:12:09 INFO mapreduce.ImportJobBase: Transferred 38.3389 KB in 71.1442 seconds (551.8226 bytes/sec)
25/03/04 05:12:09 INFO mapreduce.ImportJobBase: Retrieved 943 records.

```
