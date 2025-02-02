# A Java/Maven/JUnit HelloWorld example

A „Hello World!” sample written in Java using Maven for the build, that showcases a few very simple tests.

This example demonstrates:

* A simple calculator application with tests
* Unit tests written with [JUnit 5](https://junit.org/junit5/)
* A Maven build that puts it all together

## Running the tests

* To run the unit tests, call `mvn test`

## Conventions

This example follows the following basic conventions:

|                              | unit test                                                           | integration test                                                    |
|------------------------------|---------------------------------------------------------------------|---------------------------------------------------------------------|
| **resides in:**              | `src/test/java/*Test.java`                                          | `src/test/java/*IT.java`                                            |
| **executes in Maven phase:** | test                                                                | verify                                                              |
| **handled by Maven plugin:** | [surefire](http://maven.apache.org/surefire/maven-surefire-plugin/) | [failsafe](http://maven.apache.org/surefire/maven-failsafe-plugin/) |
