Gatling Performance Testing
============================================
![load](https://github.com/SChellapuram/gatling-java/assets/148459324/0e1859a4-634c-4d9c-93b2-d19ffe542abe)


Documentation
[refer Gatling website](https://gatling.io/docs/current/extensions/maven_plugin/) for usage. 

This project is written in Java and includes:

* [Maven Wrapper](https://maven.apache.org/wrapper/)
* Minimal `pom.xml` file
* Latest version of `io.gatling:gatling-maven-plugin`
* Sample [Simulation](https://gatling.io/docs/gatling/reference/current/general/concepts/#simulation) class,
  demonstrating various Gatling functionalities

## DPS API Services
```java
1. User Service 
2. Notification Service 
3. Training Service
4. Resource Service        
5. Organisation Service 
6. Asset Service 
```

## How to run 
1. Right-click on the 'Engine' class and select
```jshelllanguage
 Run Engine.Run()
```
2. Choose a simulation number and ENTER:
```java
[0] socialcarepassport.CreateNotificationSimulation
[1] socialcarepassport.GetBookedCoursesSimulation
[2] socialcarepassport.GetDownloadTrainingRecordSimulation
[3] socialcarepassport.GetEmployerListSimulation
[4] socialcarepassport.GetNotificationsByCurrentUser
[5] socialcarepassport.PostCreateCourseSimulation
[6] socialcarepassport.PostCreateUserSimulation
[7] socialcarepassport.UploadPhotoSimulation
```
3. Select run description (optional)
```java
Choose any description(example: Login Test) and ENTER
```
4. Gatling reports

```java
Find gatling reports under: '/target/gatling' or check console for the reports link
```
<img width="1428" alt="Screenshot 2024-01-03 at 19 48 11" src="https://github.com/SChellapuram/gatling-java/assets/148459324/dcbf2459-1572-41c9-9ec0-70f0ce6466ba">


### Useful terms

* **Scenario**: The summary of steps that the virtual users perform to simulate typical user behavior, e.g., log in to an socialcarepassport, View training records etc.
* **Simulation**: The definition of the load tests about how many virtual users will execute the Scenario in a given timeframe.
* **Session**: A state container assigned for each virtual user.
* **Recorder**: The Gatling UI to record a Scenario and output a Simulation.
* **Feeders**: A way to inject data for our virtual users from an external source like CSV files, JSON files, a JDBC data source, etc.
