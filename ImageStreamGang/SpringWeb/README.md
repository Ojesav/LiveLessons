[Sanjeev, can you please explain what dependencies are needed to run
this program.  For example, does Maven (mvn) need to be installed and
available in the shell?  Likewise, does Postman have to be installed?
We should explain how to install these tools!

[Sanjeev:] Maven is needed for building the project. Yes, if we want to invoke this in the shell, mvn is needed.
However, this could also be invoked from any IDE.
Instead of Postman, we can also use Curl utility to make HTTP requests.

Also, do you have experience with Intellij?  It would be nice if we
could set up this project using Intellij and Gradle.]
[Sanjeev:] I don't have experience working with IntelliJ. But IntelliJ seems to have a very good support for building/running SpringBoot applications. Below link can be helpful
https://www.javadevjournal.com/spring-boot/spring-boot-application-intellij/
The following are the steps required to build and run this example.

1. Change directory to the ImageStreamGang/SpringWeb folder and run
   the following command from the shell:

   % mvn spring-boot:run

   This starts the Tomcat webserver by default on port 8080 and also
   starts the WebCrawlerApplication.

   This application can also be run from within the IDE by selecting
   run on WebCrawlerApplication.

2. Below are the end points to access the application

   . http://localhost:8080/run (Post Query. Use Postman to invoke or use any Http/Java client)
   . http://localhost:8080/timingresults (Get query to fetch timing results)