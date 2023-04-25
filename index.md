# Lab Report 2 

## Part 1: String Server

**String Server Code**
![Image](StringServer1.png)
![Image](StringServer2.png)

In the class `Handler` which implements `URL Handler` we have the method `handleRequest` which is used to add strings to the web server. `handleRequest` gets the path from the url and checks if it contains `/add-message`. If the url does indeed contain `/add-message` when the request `/add-message?s=<string>` is made the web server will upadte with the string that is after the equal sign. The class `StringServer` is also on this file, and this class is used to create the web server. 

**Web server page before `/add-message?s=<string>`:****
![Image](WebServer1.png)

**Web server page when `/add-message?s=Hello` is entered:** 
![Image](WebServer2.png)

**Web server page when `/add-message?s=How are you` is entered** 
![Image](WebServer3.png)

## Part 2: Bugs
In the class `ArrayExamples` the method method `reverseInPlace` has an error occur whenever it is used on an array that has two or more arrays.

**Failure-Inducing Input:**
```
@Test 
public void testReverseInPlace1() {
    int[] input1 = { 3 , 5, 7};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 7, 5, 3 }, input1);
    }
  ```
  
**Input that runs correctly**
```
@Test 
public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
    }
  ```
