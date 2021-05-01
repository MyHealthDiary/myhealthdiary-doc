 Supporting Materials for the article "A Self-Management Diabetes Mellitus Application for Support Treatment by Using Smart Reminders and Low-Cost Fitness Bracelet"
 
The set of repositories is composed by:

- A [Documentation](https://github.com/MyHealthDiary/myhealthdiary-doc) repository containing requirements and documentation of the project.
- The [Front-End](https://github.com/MyHealthDiary/myhealthdiary-app) repository containing the code of the Flutter application. 
- The [Back-End](https://github.com/MyHealthDiary/myhealthdiary-server) repository containing the code of the Spring Boot webservices.

### A Self-Management Diabetes Mellitus Application for Support Treatment by Using Smart Reminders and Low Cost Fitness Bracelet

Chronic diseases, especially diabetes mellitus, are a huge public health burden. Consequently, new health care models are needed to share the responsibility for treatment between health care providers and the patients themselves. The concept of empowerment promotes active patient participation and control over their health. This can be achieved through education, self-government and collaborative decision-making. All these aspects can be covered by mobile health technologies, the so-called mobile health. These are mobile phones, patient monitoring devices, tablets, personal digital assistants, other wireless devices, and numerous applications.

This project has developed a mobile application that aims to solve many of the problems of diabetics using mobile health, including glycemic control, nutritional control, physical activity, high blood pressure, adherence to treatment, obesity.

The application has been tested and evaluated by the user. The application interface is very simple and intuitive for all ages.

Application development consisted of three stages.<br>
![](https://i.imgur.com/Z6vEOQW.png)

1. The first stage defines the requirements for the application. Answers the question "What features should an app include to effectively control Diabetes?" For this, a study of scientific works and existing applications was carried out, as well as a survey among patients. After that, all the data was analyzed to determine the functions for the design of the mobile application.
2. The second stage is the development of an application that works in real time with a fitness bracelet and a server. For development was using Dart as a programming language and the framework Flutter. We chose this because it makes it possible to develop a cross-platform system for iOS and Android apps. For the storage of data, we use PostgreSQL with a DaS model provided by ElephantSQL. BLE and GATT services were used for the fitness bracelet. The back-end part was developed using Spring Boot and hosted on Amazon Web Services.
3. The third stage includes testing and evaluating the system. Functional testing was performed using an Android device by one user who used the application for 1 week.


Architecture, environment and connection between parts of system a shown on the Figure. The system is composed by a front end part, with a mobile application and a back end part, with a web server. <br>
![](https://i.imgur.com/2bOhSsO.png)

The system consists of a server part, which performs the functions of collecting and processing information. All data that the user enters and wearable devices are stored in the server, after processing, the user is provided with feedback in the form of the latest health information on the main page, in the form of a graph and in the form of decision notifications.

The fitness bracelet, in turn, provides data on physical activity such as steps and exercises taken, as well as sleep and heart rate.

The rest of the data such as blood glucose level, pressure and weight are entered using the application by the user. There is also an automatic BMI calculation function. To enter carbohydrates, a database is used that contains 2 million types of food. The user can select food and gram and the database will find data about this food.

Reminder functions are provided for timely taking medications and checking blood glucose levels. There is a built-in notification function to notify if health indicators go out of the norm. This will help the user make timely decisions to improve health.

When all the reliable data on health and behavior during the treatment of the patient is collected, user can download the report to send to the doctor. <br>
![](https://i.imgur.com/0NPdW75.png)<br>
Flow and structure of application

Interface of application.<br>
![](https://i.imgur.com/duJi1jr.png)

