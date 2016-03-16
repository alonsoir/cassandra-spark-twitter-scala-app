# cassandra-spark-twitter-scala-app

The purpose of is tiny project is to learn about how to interact with a Cassandra db using scala, in adittion to use Apache Spark and twitter.

The idea is to integrate the databricks reference app, which uses spark-streaming and machine learning techniques with the necessary code from Manuel Kiessling to interact with a cassandra instance.

The project is packed with sbt-pack, so in order to get running this project, download it to a local folder and run sbt and inside it, pack, that is all, sbt-pack will compile and pack in a uber jar all the necessary and it will create a unix command to run the code:

MacBook-Pro-Retina-de-Alonso:~ aironman$ cd Downloads/
MacBook-Pro-Retina-de-Alonso:Downloads aironman$ cd cassandra-spark-twitter-scala-app-master/
MacBook-Pro-Retina-de-Alonso:cassandra-spark-twitter-scala-app-master aironman$ sbt
[info] Loading project definition from /Users/aironman/Downloads/cassandra-spark-twitter-scala-app-master/project
[info] Updating {file:/Users/aironman/Downloads/cassandra-spark-twitter-scala-app-master/project/}cassandra-spark-twitter-scala-app-master-build...
[info] Resolving org.fusesource.jansi#jansi;1.4 ...
[info] Done updating.
[info] Set current project to spark-twitter-lang-classifier-using-cassandra (in build file:/Users/aironman/Downloads/cassandra-spark-twitter-scala-app-master/)
> pack
[info] Updating {file:/Users/aironman/Downloads/cassandra-spark-twitter-scala-app-master/}cassandra-spark-twitter-scala-app-master...
[info] Updating {file:/Users/aironman/Downloads/cassandra-spark-twitter-scala-app-master/}common...
[info] Resolving org.fusesource.jansi#jansi;1.4 ...
[info] Done updating.
[info] Resolving com.codahale.metrics#metrics-core;3.0.2 ...
[info] Packaging /Users/aironman/Downloads/cassandra-spark-twitter-scala-app-master/target/scala-2.10/spark-twitter-lang-classifier-using-cassandra_2.10-0.1-SNAPSHOT.jar ...
[info] Resolving com.chrisomeara#pillar_2.10;2.0.1 ...
[info] Done packaging.
[info] Resolving org.fusesource.jansi#jansi;1.4 ...
[info] Done updating.
[info] Updating {file:/Users/aironman/Downloads/cassandra-spark-twitter-scala-app-master/}main...
[info] Resolving com.google.guava#guava;16.0.1 ...
[info] Compiling 3 Scala sources and 1 Java source to /Users/aironman/Downloads/cassandra-spark-twitter-scala-app-master/common/target/scala-2.10/classes...
[info] Resolving org.fusesource.jansi#jansi;1.4 ...
[info] Done updating.
[info] Packaging /Users/aironman/Downloads/cassandra-spark-twitter-scala-app-master/common/target/scala-2.10/common_2.10-0.1.jar ...
[info] Compiling 5 Scala sources to /Users/aironman/Downloads/cassandra-spark-twitter-scala-app-master/main/target/scala-2.10/classes...
[info] Done packaging.
[warn] Multiple main classes detected.  Run 'show discoveredMainClasses' to see the list
[info] Packaging /Users/aironman/Downloads/cassandra-spark-twitter-scala-app-master/main/target/scala-2.10/main_2.10-0.1.jar ...
[info] Done packaging.
[info] Creating a distributable package in target/pack
[info] Copying libraries to target/pack/lib
blablabla...
[info] Generating target/pack/VERSION
[info] done.
[success] Total time: 10 s, completed 16-mar-2016 9:58:35
> exit
MacBook-Pro-Retina-de-Alonso:cassandra-spark-twitter-scala-app-master aironman$ target/pack/bin/collect
Usage: Collect$<outputDirectory> <numTweetsToCollect> <intervalInSeconds> <partitionsEachInterval>
MacBook-Pro-Retina-de-Alonso:cassandra-spark-twitter-scala-app-master aironman$ 

You can see that this new command needs four parameters
