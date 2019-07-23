The rhtpt system can be installed by going to this link   https://github.com/ilabafrica/rhtpt  or use this link to access it online http://rhtpt.or.ke. You can download the zip file or clone the repository to your machine.

    1. Extract this git repository to a local folder

            git clone git@github.com:ilabafrica/rhtpt.git 

    2. Change directory to the root folder of the application. Update composer then run it in order to install the application dependencies. You may need root permissions to update composer.
             
             Composerself-update
             composer install

    3. Update the application configuration files to suit your local settings:

        ◦ Set the "Application URL" in /app/config/app.php
        ◦ Create a database and set the database connection details in /app/config/database.php
        ◦ The organization name in /app/config/rhtpt.php

    4. Run the migrations to create the required database tables.
	    
	    php artisan migrate
    
    5. Load the basic seed data
	   php artisan db:seed

If #4 or #5 above fails, you may need to run the following command then repeat the two commands again.
composer dumpautoload

###1.6 Security and Privacy Considerations

This system stores personal health test result for users which they might not other people to know about. Hence the system has been structured to give access to authorized users to whom they can view the data. One of the users who are not allowed to view the results are the partners as their work is just to oversee and support the different counties which they are in and are not included in the Proficiency testing process. This is why the permission for the partners to view the results is not checked in the administrators menu. 

This system was built to provide and protect that will be gathered of the following years and provide an analysis of the number of test done, the number of participant who participated in the rounds with the aim to improve the proficiency testing process as compared to what was being done previously using the manual method.

###1.7 User Access Requirements

 In order for users to access this system they would require an internet connection as the system is web based and it is hosted on web based server that requires the client (user of the system) to make a request to the server through the web sites URL which will respond with the RHTPT login page.
The users can then use their username i.e email or their enrollment ID’s and passwords to log in to the system. For first time registration of participants into the system, they will be required to wait for an approval by their respective county or sub county coordinators to approve them. Once approved they will receive an SMS notification together with and email with their enrollment ID and confirmation of their registration into the system. 

###1.8 Security and Privacy rules

The following are some of the security and privacy rules implemented in the system. 
  
    • SMS sending is limited to the administrator only.
    • Expected results are entered by the administrator only for the coming round.
    • Results can be viewed by uses with access rights.
    • Filtering of participants and facilities is based on county region.
    • Depending on the users role they can either edit, create or view only.
