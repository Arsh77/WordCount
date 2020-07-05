# WordCount
Prepared word count using java maven and hadoop

command to run jar:
hadoop jar <address of jar> <Class to run> <Class to run> <input file address> <address of output folder to be generated>

Steps to run:

1. Make a directory /user/input in hdfs:
  hdfs dfs -mkdir /user 
  hdfs dfs -mkdir /user/input

2. Add input file to hdfs /user/input folder:
  hdfs dfs -put ~/Document/hadoopInput/wordInput /user/input

3. Run jar:
  #for me the command was like this.
  hadoop jar ~/eclipse-workspace/wordcount/target/wordcount-0.0.1-SNAPSHOT.jar WordCount WordCount /user/input/wordInput.txt /user/output
