# lazy

- install local jar as maven dependency
```
mvn install:install-file -Dfile=../../kafka_dup/clients/build/libs/kafka-clients-2.2.0-SNAPSHOT.jar -DgroupId=org.apache.kafka -DartifactId=kafka-clients -Dversion=2.2.0-SNAPSHOT -Dpackaging=jar
```

- check presence of debug symbols in java classes 
```
javap -l class
```

Enable Java, Scala debug mode  - compiler options (e.g. in build.gradle):
```
-g
-g:notailcalls
```

