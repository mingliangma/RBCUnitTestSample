##Sample Project for Unit Test
The goal of this project is to illustrate to how write Unit Test in Scala with SBT. Integrated tests have been set up under a test task in each build system. To run the tests, invoke the build system and then launch test.


### Build
```$xslt
sbt clean assembly 
```

### Run
```$xslt
dse spark-submit --class com.datastax.spark.example.WriteRead target/scala-2.11/writeRead-assembly-0.1.jar
```

### Run Test
```$xslt
sbt test
```