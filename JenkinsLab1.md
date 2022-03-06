# Jenkins lab 1

**01) What is Jenkins used for?**

Jenkins is a self-contained, open source automation server which can be used to automate all sorts of tasks related to building, testing, and delivering or deploying software.

**02) What is Jenkins agent? What is Jenkins executor (Build Executor)?**

Agent is a machine that connects to the jenkins controller and executes tasks directed by the controller , A Jenkins executor is one of the basic building blocks which allow a build to run on a node/agent (e.g. build server). Think of an executor as a single “process ID”, or as the basic unit of resource that Jenkins executes on your machine to run a build.

**03) Explain Jenkins master-slave architecture?**

The Jenkins master is the original node in the Jenkins installation. The Jenkins master administers the Jenkins slaves and orchestrates their work, including scheduling jobs on slaves and monitoring agents. Slaves may be connected to the Jenkins master using either local or cloud computers.

**04) Mention three security mechanisms used by Jenkins to authenticate users?**



1. Web UI

   ​	When you use the form on the login page, using the fields j_username and j_password

2. REST API

   ​  Using Basic with login / password

   ​	Using Basic with login / apiToken

3. Jenkins CLI jar

   ​	(deprecated) using remoting transport with login / logout command

   ​	(deprecated) username / password as parameters on each command

   ​	-auth argument with username:password or username:apiToken that will do something like HTTP calls

   ​	using SSH transport mode with your local keys





**05) Mention ways that a job can be run/scheduled in Jenkins?**

Using  cron expression.



**06) How can we restart the Jenkins server (Hint it's an endpoint we visit in the browser)?**

[http://127.0.0.1:8080/restart](http://127.0.0.1:8080/restart)



**07) Install Jenkins with docker image.**

<img src="https://i.imgur.com/MkM4Z78.png" alt="image-20220306080025954" style="zoom:100%;" />

**08) Install role-based authorization plugin.**

![image-20220306080852607](https://i.imgur.com/iLAmrrX.png)

**09) Create a new user.**

![image-20220306081150016](https://i.imgur.com/CAaTSDf.png)



**10) Create a read role and assign it to the new user**

![image-20220306081506782](https://i.imgur.com/wL2jIWK.png)



**11) Create a freestyle project and link it to the private git repo (inside it create a directory and create a file with "hello world").**

![image-20220306114334083](https://i.imgur.com/bec6Xvq.png)
