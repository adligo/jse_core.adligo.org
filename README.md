# jse-core.adligo.org
This is the repository for the most current version of java, currently jdk-24, Gradle 8.14;

To set this up download jdk-24 from;
```
https://jdk.java.net/24/
```
Note jdk24 is needed to run Gradle, which compiles and runs tests with jdk24.

Download and setup gradle
```
https://gradle.org/install/
```

You will need to point JAVA_HOME to jse 24 and Gradle with an environment variables, i.e. with Windows on GitBash I have something like; 

```
# Note this JDK24 environment variable is picked up by gradle @ see
# gradle.propertes
# org.gradle.java.installations.fromEnv=JDK24
#
export JDK24=/c/foo/bar/jdk-24
export JAVA_HOME=$JDK24
export GRADLE_HOME=/c/foo/bar/gradle
```

Then simply run this to build and run the tests;

```
gradle build

```

If you would like the individual test all in the same folder (i.e. for a Jenkins build) run this;

```
./moveTextXmlFiles
```

The latest Docker build Image is COMING SOON and was ... ;

```
adligo/jenkins-2023-04-30:v1
```

https://hub.docker.com/repository/docker/adligo/jenkins-2023-04-30/general

Running Single Sub Projects can be achieved with

```
gradle :math_tests.adligo.org:build
```


