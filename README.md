

# Example Java Library using Gradle: Part 1

The purpose of this project is to be a basic Java library that is built using Gradle, with the intention of adding to it common software utilities step by step.

The important step here, is how to run the build which includes any associated testing, other automation, and ultimatley builds the jar file:

```bash
$ ./gradlew clean build -i
> Configure project :lib
> Task :lib:clean
> Task :lib:compileJava
> Task :lib:processResources NO-SOURCE
> Task :lib:classes
> Task :lib:jar
> Task :lib:assemble
> Task :lib:compileTestJava
> Task :lib:processTestResources NO-SOURCE
> Task :lib:testClasses
> Task :lib:test
> Task :lib:check
> Task :lib:build

BUILD SUCCESSFUL in 919ms
5 actionable tasks: 5 executed
```



# FAQ

## How did I create this initial project?

```bash
~/workspaces/personal/example-java-gradle-lib-1 $ gradle init
Starting a Gradle Daemon, 1 incompatible Daemon could not be reused, use --status for details

Select type of project to generate:
  1: basic
  2: application
  3: library
  4: Gradle plugin
Enter selection (default: basic) [1..4] 3

Select implementation language:
  1: C++
  2: Groovy
  3: Java
  4: Kotlin
  5: Scala
  6: Swift
Enter selection (default: Java) [1..6] 3

Select build script DSL:
  1: Groovy
  2: Kotlin
Enter selection (default: Groovy) [1..2] 1

Generate build using new APIs and behavior (some features may change in the next minor release)? (default: no) [yes, no] 

Select test framework:
  1: JUnit 4
  2: TestNG
  3: Spock
  4: JUnit Jupiter
Enter selection (default: JUnit Jupiter) [1..4] 4

Project name (default: example-java-gradle-lib-1): 
Source package (default: example.java.gradle.lib): 

> Task :init
Get more help with your project: https://docs.gradle.org/7.6/samples/sample_building_java_libraries.html

BUILD SUCCESSFUL in 29s
2 actionable tasks: 2 executed
```

## How did I generate the Gradle Wrapper?

```bash
$ gradle wrapper
```

