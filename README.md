# jse-core.adligo.org
This is the repository for the most current version of java, currently jdk-20, Gradle 8.2.1;

To set this up download jdk-19 and jdk-20 from;
```
https://jdk.java.net/19/
https://jdk.java.net/20/
```
Note jdk19 is needed to run Gradle, which compiles and runs tests with jdk20.

Download and setup gradle
```
https://gradle.org/install/
```

You will need to point JAVA_HOME to jse 19 and Gradle at JDK 20 with an environment variable, i.e. with Windows on GitBash I have something like; 
```
export JDK19=/c/foo/bar/jdk-19
export JAVA_HOME=$JDK19
export GRADLE_HOME=/c/foo/bar/gradle
export PATH=$JDK19/bin:$PATH:$GRADLE_HOME/bin
export JDK20=/c/foo/bar/jdk-20
```

The latest Docker build Image is COMING SOON and was ... ;
```
adligo/jenkins-2023-04-30:v1
```
https://hub.docker.com/repository/docker/adligo/jenkins-2023-04-30/general




