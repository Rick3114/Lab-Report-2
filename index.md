# Lab Report 2 

## Part 1: String Server

**String Server Code**
![Image](StringServer1.png)
![Image](StringServer2.png)

In the class `Handler` which implements `URL Handler` we have the method `handleRequest` which is used to add strings to the web server. `handleRequest` gets the path from the url and checks if it contains `/add-message`. If the url does indeed contain `/add-message` when the request `/add-message?s=<string>` is made the web server will upadte with the string that is after the equal sign. 
