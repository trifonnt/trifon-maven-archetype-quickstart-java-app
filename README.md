* Clone repository
```shell
$ git clone https://github.com/trifonnt/trifon-maven-archetype-quickstart-java-app
```

* Build
```shell
$ cd trifon-maven-archetype-quickstart-java-app
$ mvn install
```

* Install new Archetype into local Maven repository
```shell
$ mvn install:install-file -Dfile=target/trifon-archetype-quickstart-java-app-0.0.1.jar -DgroupId=name.trifon -DartifactId=trifon-maven-archetype-quickstart-java-app -Dversion=0.0.1 -Dpackaging=jar
```

* Use new Archetype to create sample project based on the new archetype
```shell
$ mvn archetype:generate 
  -DarchetypeGroupId=name.trifon                                   \
  -DarchetypeArtifactId=trifon-maven-archetype-quickstart-java-app \ 
  -DarchetypeVersion=0.0.1                                         \
  -DgroupId=name.trifon.sample                                     \
  -DartifactId=sample-java-01                                      \
  -Dversion=0.0.1-SNAPSHOT                                         \
  -Dpackage=name.trifon.sample.java                                \
  -DlearnlibVersion=0.9-SNAPSHOT    # optional
```

```shell
$ mvn archetype:generate -DarchetypeGroupId=name.trifon -DarchetypeArtifactId=trifon-maven-archetype-quickstart-java-app -DarchetypeVersion=0.0.1 -DgroupId=name.trifon.sample -DartifactId=sample-java-01 -Dversion=0.0.1-SNAPSHOT -Dpackage=name.trifon.sample.java
```
