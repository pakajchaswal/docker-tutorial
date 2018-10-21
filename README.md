# docker-tutorial

Docker intro (for the sake of it), in my words :

Docker is to application's(anything that's deployable, runnable) what JVM is to java. Another three lines in an attempt to 
understand docker better:

You can have multiple instances of an application running on a single machine:

1. Have multiple deployables of an application e.g. multiple tomcats listening to different ports.
2. Have application run on multiple VM's(virtual machines, 
   this means multiple operating systems running on a single machine using hypervisr), this way you can run multiple 
   tomcats listening to same port.
3. Compartmantalize application in a Docker container, and run multiple instances of docker (ofcourse different ports).

Now from above 3 points, to a layman the question appears(it appeared to me as well sometime back), how 1 and 3 are any 
different? Believe me its a good question, as understanding docker is all about answering this question.

The difference between 1 and 3.
1. Containerize once and use anywhere. It a big hassel maintaining the deployed application version, software versions, 
   dependencies version across different environments(DEV, QA, UAT, PT, PROD), with docker you can build a release once and 
   play it in any environment and be rest assured that all the working componets have their version synced.

2. When you containerize via docker you can customize or control the resouces your application is going to use i.e memory, CPU.
   Docker also ensures that each application only uses resources that have been assigned to them. A particular application 
   won’t use all of your available resources, which would normally lead to performance degradation or complete downtime for 
   other applications.

3. With Docker, you can use different versions of same software(e.g. java) because docker is the runtime environment for 
   application, different applictions have different runtime environments which can vary without affecting others.
