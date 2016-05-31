+01) Install new Archetype
$ mvn install


+02) Use new Archetype to create sample project based on the new archetype
$ mvn archetype:generate 
  -DarchetypeGroupId=name.trifon                                   \
  -DarchetypeArtifactId=trifon-maven-archetype-quickstart-java-app \ 
  -DarchetypeVersion=0.0.1                                         \
  -DgroupId=name.trifon.sample                                     \
  -DartifactId=sample-java-01                                      \
  -Dversion=0.0.1-SNAPSHOT                                         \
  -Dpackage=name.trifon.sample.java                                \
  -DlearnlibVersion=0.9-SNAPSHOT    # optional

$ mvn archetype:generate -DarchetypeGroupId=name.trifon -DarchetypeArtifactId=trifon-maven-archetype-quickstart-java-app -DarchetypeVersion=0.0.1 -DgroupId=name.trifon.sample -DartifactId=sample-java-01 -Dversion=0.0.1-SNAPSHOT -Dpackage=name.trifon.sample.java
