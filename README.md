### 4.1_Spring_Framework_Basics_Level1


## Spring and Maven Exercise

This exercise is a first contact with Spring and Maven.

Access the page ->https://start.spring.io/, and generate a Spring boot project with the following characteristics:

#### PROJECT (dependency manager)

* Maven.

#### LANGUAGE

* Java.

#### SPRING BOOT

* The latest stable version.

#### PROJECT METADATA

* Group: cat.itacademy.s04.t01.n01

* Artifact: S04T01N01

* Name: S04T01N01

* Description: S04T01N01

* Package name: cat.itacademy.s04.t01.n01

#### PACKAGING

* Jar

#### JAVA

* Minimum version 11

* Dependencies: Spring Boot DevTools, Spring Web
  

Import it into Eclipse with the File > Import > Existing Maven Project option.

In the application.properties file, configure the server.port variable with the value 9000.

We will convert this application into a REST API:

Depending on the main package, create another subpackage called controller, and inside it, add the HelloWorldController class.

It should have two methods:
String hello
String hello2

These two methods will receive a String parameter called name, and will return the phrase:

“Hello, “ + name + “. You are running a Maven project”.

The first method will respond to a GET request, and should be configured to receive the parameter as a RequestParam. The "name" parameter will have the default value “UNKNOWN”.

It should respond to:

http://localhost:9000/HelloWorld
http://localhost:9000/HelloWorld?name=Myname

The second method will respond to a GET request, and should be configured to receive the parameter as a PathVariable. The "name" parameter will be optional.

It should respond to:

http://localhost:9000/HelloWorld2
http://localhost:9000/HelloWorld2/elmeunom

#### Practice Basic Maven Commands

Make sure Maven is installed and configured on your system. Open a terminal (from your IDE or from the command line on Windows, Mac, etc.) and navigate to your project directory. The goal is for you to become familiar with some important Maven commands:

* Compile the Project: mvn compile
* Package the Project: mvn package
* Clean the Project: mvn clean
* Run the Application: mvn spring-boot:run
