##1.0 Introduction
###1.1 Project Purpose
The purpose of this technical document is to provide documentation to the prospective NPHL developer’s technical team to help understand the architecture and structure of the RHTPT system.
###1.2 System Overview
The system was built using laravel framework version 5.3 which is a Model View Controller framework.  This approach helped in developing of dynamic web systems. The front end was built with a combination of HTML 5 and Vuejs.   The system database uses Mysql database queries and tables to perform CRUD operations with the assist of VueJs API Requests. 
###1.2.1 System Characteristics

* Operates in real-time and  linked to month-end reporting.
* Supports a large number of concurrent users.
* Highly resilient or fault tolerant.
* Highly scaleable and easily maintainable in the future.


###1.3 HTML5, VueJs and Controller Structure

HTML and VueJs are used in the front end to render data and carry out API call requests from the front end to the backend via the web route to the controller.  The project structure revolves around three folders the view folder that is found in the resource folder which contains the views of the different pages. The second folder is the controller’s java script files that are found in the public/controllers folders. Finally the controllers for the different views which are found in the http/controllers folders.
### 1.4 Setup and Configurations
###1.4.1 Requirements
    • Supported database. Currently only MySQL has been tested. 
    • PHP version 5.6.21
    • Composer - Dependency manager for PHP    
