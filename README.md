
## Project Name

To perform the API Automation using the Karate framework.

[![Maven Central](https://img.shields.io/maven-central/v/com.intuit.karate/karate-core.svg)](https://mvnrepository.com/artifact/com.intuit.karate/karate-core) [![Build Status](https://travis-ci.org/intuit/karate.svg?branch=master)](https://travis-ci.org/intuit/karate) [![GitHub release](https://img.shields.io/github/release/intuit/karate.svg)](https://github.com/intuit/karate/releases) [![Support Slack](https://img.shields.io/badge/support-slack-red.svg)](https://github.com/intuit/karate/wiki/Support) [![Twitter Follow](https://img.shields.io/twitter/follow/KarateDSL.svg?style=social&label=Follow)](https://twitter.com/KarateDSL)


The main motive of this project is to Automate the API's using karate framework. In this Example I have taken the mock API's from the http://dummy.restapiexample.com/ and Automated the CRUD operation.

![](header.png)

## Installation

Operating System:

```sh
Ubuntu 18.04
```
Editor:

```sh
Install Eclipse Photon (4.8) - https://www.eclipse.org/downloads/
```
JDK:

```sh
at least version 1.8.0_112
```

Maven dependencies:

```sh
<dependency>
  <groupId>com.intuit.karate</groupId>
  <artifactId>karate-apache</artifactId>
  <version>0.9.4</version>
  <scope>test</scope>
  </dependency>
<dependency>
  <groupId>com.intuit.karate</groupId>
  <artifactId>karate-junit4</artifactId>
  <version>0.9.4</version>
  <scope>test</scope>
</dependency>
```
## Directory Structure

```
src/test/java
    |
    +-- karate-config.js
    +-- logback-test.xml
    |
    \-- com/api
            |
            \-- feature
            |     |
            |     +-- AllFeatureFileRunner.java      
            |     |
            |     +-- CreateEmployeeRecord.feature
            |     |
            |     +-- DeleteEmployeeRecord.feature
            |     |
            |     +-- GetAllEmployeesRecord.feature
            |     |
            |     +-- GetResponseForIdZero.txt
            |     |
            |     +-- GetSingleEmployeeRecord.feature
            |     |
            |     +-- PostInvalidRequestData.json
            |     |
            |     +-- PostRequestValidData.json
            |     |
            |     +-- UpdateDetailsRequest.json
            |     |
            |     +-- UpdateEmployeeRecord.feature
            |
            \-- runner
                  |
                  +-- CreateEmployee.java
                  |
                  +-- DeleteEmployee.java
                  |
                  +-- GetAllEmployees.java
                  |
                  +-- GetSingleEmployee.java
                  |
                  +-- UpdateEmployeeDetails.java
  

```
## Usage example

1. *.feature - All feature files under feature folder contain the different scenarios which we can perform for the perticular request. As an Example consider the CreateEmployeeRecord.feature which contains the different scenarios by which we can test the api and all these scenarios can run automatically depending on the call given to them.
2. *.java - All java files under runner folder contain the individual caller for respective feature file
3. *.txt & *.json - All *.txt & *.json files contain the data of request or response of the API to manipulate the runtime behavior of the API by comparing it with the exact response which we get from the API after calling it.
4. AllFeatureFileRunner. java - Used to run all the feature files at once

## Report Generation

Report for the above execution gets generated in /target/surefire-reports where you can see the web based report of the execution of the feature file.


## Development setup

1. Install the JDK at least version 1.8.0_112.
2. Install eclipse Photon (4.8)
3. Create maven project in eclipse 
4. Add dependencies for karate in the POM.xml
5. You can create the feature file which contains the information about the operation which we were going to perform and to call that feature we need to create the java class.


## Meta

Your Name – [@Ajij_13](https://twitter.com/Ajij_13) – shaikhajij1234@gmail.com

[https://github.com/ajijshaikh/github-link](https://github.com/ajijshaikh/)

