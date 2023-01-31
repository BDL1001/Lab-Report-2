# _Lab Report 2_

## StringServer

![StringServer](StringServer.png)
* *StringServer.java* determines the functionality/behavior of the web server by handling the url paths
* It is supported by the *Server.java* file from Week 2 Lab

![Screenshot1](Screenshot1.png)
* Both the main method of StringServer class and the handleRequest method of the Handler class are called
* The value 4000 is passed to the main method of the StringServer class
  * The value 4000 is actually saved as a string (in the args array)
  * We have to parse it into an int then it can be used as the port number
* The URI/URL (http:/localhost:4000/add-message?s=first) is then passed to the handleRequest method
* Then *first* is saved/concatenated into a string variable/field within the Handler class named *display*
* The *display* variable 

![Screenshot2](Screenshot2.png)
* 

## What I Learned

Week 2 lab was 
