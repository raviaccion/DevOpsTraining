# DevOps-WebApp project integrated with CI model 
# Added more lines of code
-------------------------------
DevOps-WebApp for maven web app projects

## By: Devops

# Pre-requesites:
---------------
-- Install Java
-- Install maven
  -- $sudo apt-get update on Ubuntu Linux Machine 
  -- $sudo apt-get install maven on Ubuntu Linux Machine
  -- $mvn -version
--Install tomcat8 webserver with Ubuntu Linux version below 18.0
  -- $apt-get install tomcat8
--Install tomcat9 webserver with Ubuntu Linux version 20.0
  --$apt-get install tomcat9

To create a simple java project using maven, you need to open command prompt and run the archetype:generate command of mvn tool:
----------------------------------------------------------------------------------------------------------------------------------
 mvn archetype:generate -DgroupId=com.javatpoint -DartifactId=CloudenabledWebApp -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false
 
 It will generate following code in the command prompt::
 ----------------------------------------------------------
 1) Automatically Generated pom.xml file
 2) Automatically Generated index.jsp file
 3) Automatically Generated web.xml file
 
  How to Build the maven project or how to package maven project ?:
 ===============================================================
 mvn package  
 
 Deploy and Run the Maven Web Project
 =======================================
 Deploy the project on the server and access it by the following url:
 http://<host-name>:<portnumber>/projectname, for example: http://localhost:8080/DevOps-Training
 
 For Tomcat 8: - By copying the generated war file onto /var/lib/tomcat8/webapp and restart the tomcat8 service
 
 For Tomcat 9: - By copying the generated war file onto /var/lib/tomcat9/webapp and restart the tomcat9 service
 
For adding feature copy below lines and update index.html on line 33 

<form action="http://www.html.am/html-codes/textboxes/submitted.cfm">
<textarea name="myTextBox" cols="50" rows="5" style="background-color:#FCF5D8;color:#AD8C08;">
Enter some text...
</textarea>
<br />
<input type="submit" />
</form>
