# Credentials Folder

## The purpose of this folder is to store all credentials needed to log into your server and databases. This is important for many reasons. But the two most important reasons is
    1. Grading , servers and databases will be logged into to check code and functionality of application. Not changes will be unless directed and coordinated with the team.
    2. Help. If a class TA or class CTO needs to help a team with an issue, this folder will help facilitate this giving the TA or CTO all needed info AND instructions for logging into your team's server. 


# Below is a list of items required. Missing items will causes points to be deducted from multiple milestone submissions.

1. Server URL or IP

	http://ec2-54-215-110-168.us-west-1.compute.amazonaws.com/
	
2. SSH username

	ubuntu
	
3. SSH password or key.

	Team03-Development.pem file is updated

    <br> If a ssh key is used please upload the key to the credentials folder.

4. Database URL or IP and port used.
    
    <br><strong> NOTE THIS DOES NOT MEAN YOUR DATABASE NEEDS A PUBLIC FACING PORT.</strong> But knowing the IP and port number will help with SSH tunneling into the database. The default port is more than sufficient for this class.

	Endpoint - database-1.cfucueuaq4qk.us-west-1.rds.amazonaws.com
	port - 3306
	

5. Database username
    admin
6. Database password
    12345678
7. Database name (basically the name that contains all your tables)
    database-1
8. Instructions on how to use the above information.
Connecting DB to workbench:

Input fields: 

Hostname: database-1.cfucueuaq4qk.us-west-1.rds.amazonaws.com
Port: 3306
username: admin
password: 12345678 (should prompt you to input this upon trying to connect)

Please do let me know if you are unable to connect to our db. I might have to add a rule in which allows your IP to access it. http://checkip.amazonaws.com/


Accessing EC2 server:
cd (change directory) on terminal / console to where you stored your downloaded .pem file (name should be Team03-Development.pem).

while in the proper directory run command:
ssh -i "Team03-Development.pem" ubuntu@http://ec2-54-215-110-168.us-west-1.compute.amazonaws.com/

    
username later on might vary depending if multiple users are implemented. 
general cmd would be ssh -i "Team03-Development.pem" http://ec2-54-215-110-168.us-west-1.compute.amazonaws.com/



# Most important things to Remember
## These values need to kept update to date throughout the semester. <br>
## <strong>Failure to do so will result it points be deducted from milestone submissions.</strong><br>
## You may store the most of the above in this README.md file. DO NOT Store the SSH key or any keys in this README.md file.
