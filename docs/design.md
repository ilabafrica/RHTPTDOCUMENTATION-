###2.1 Scope

This functional and technical requirements document will outline the functional, performance, security, notifications and other system architectures to the developers. This document outlines briefly the technical aspect of the RHTPT system.

###2.2 Functional Requirements

* Users Login: One of the core functions of this system is the user login. Different users with different roles will log into the dashboard with different sidebar menus. The administrator role will be able to see all the sidebar menu’s as compared to a Participant role who will only have the Proficiency Testing Sidebar menu and results sub menu only.

* User Permissions: Different users can be given different permissions within the system that will grant them certain privileges and also limit them to what they can do within the system. One of the permission within the system is create role which when enabled for a specific user role will allow them to create roles for different users.

* Results Algorithm: This is a results “marking Scheme” that compares the results entered by participants. The expected results are entered by the administrator for a specific round. Once the expected results are verified by the administrator it will be used as a reference by the algorithm to counter check the results entered by the participants. Once the algorithm counter checks the results of the participant it will either give an output of satisfactory or unsatisfactory.

* Configurations:  The system allows for different configurations such as SMS, Programs, shipping agents and Designations.  It enables the users to add their own preferred shipping agents, add programs create and send defaults/custom SMS to users.
 
###2.3 Non-Functional Requirements

* Performance: The system response time is reliable as the algorithm improves on the results throughput which reduces the time from when the results are submitted to when they are checked and verified. This makes the system highly reliable as the process is automated hence enabling it to process large amount of data concurrently.

* Availability: The system build quality and speed has been designed to produce the at most performance when handing any amount of data. The system performance ranges between 90-95% as it is less prone to errors.

* Reliability: The mean time between failures is estimated at 5 minutes every 24 hours or so meaning that the system may fail for 5 minutes after every 24 hours which is highly unlikely considering the extensive amount of tests the system has undergone during development.

* Maintainability: The modularization of the system enables it to fix errors in case of failures that may occur while the system is still being used. After the errors have been fixed the patch can be merged into the system and restore full services within the shortest time possible.

###2.4 Model View Controller (MVC) Approach.

MVC is a software architectural pattern for implementing user interfaces. The modules will be redesigned using this approach so as to achieve modularisation of the system components. This will allow easy maintenance and upgrading of the system.

###2.5 API Centric Development

API centric development allows the system to expose an interface to other systems for easy integration. This design will allow integration of other third party systems seamless and performance optimization. The APIs will also create a uniform point for integrating all other applications e.g. Mobile application or services run by the organization.

###2.6 Microservice Design pattern.

Based on the development approach we have chosen, a Microservice design pattern come in handy. The pattern allows components of the system to run as independent applications. This improves the security and performance of system. This approach ensures all the system components are decoupled. A Microservice design pattern made it easier for scalability and availability, this is achieved by not allowing some failing components of the system to tamper with other services since each service is independent. 
###2.7 Notification Service

The system has integrated a notification system so as to facilitate communication between the organization and its personnel. The service allows drafting of messages using predefined templates. This allows for flexibility and fast delivery of information to the clients in the field.
