# _Lab Report 2_

## Part 1

![StringServer](StringServer.png)
* *StringServer.java* determines the functionality/behavior of the web server by handling the url paths
* It is supported by the *Server.java* file from Week 2 Lab

![Screenshot1](Screenshot1.png)
* Both the main method of StringServer class and the handleRequest method of the Handler class are called
* The value 4000 is passed to the main method of the StringServer class when the StringServer.java was ran in the terminal
  * The value 4000 is actually saved as a string (in the args array)
  * We have to parse it into an int then it can be used as the port number
* The URI/URL ***http:/localhost:4000/add-message?s=greetings*** is then passed to the handleRequest method
* Then *greetings* in the path's query is concatenated into a string variable/field within the Handler class named *display*
* The newline escape character ("\n") is then concatenated to the *display* variable
* The *display* variable then becomes "greetings\n" and is displayed

![Screenshot2](Screenshot2.png)
* The handleRequest method is called
* The URL path ***http:/localhost:4000/add-message?s=testing%202nd%20line*** is passed to the handleRequest method 
* In url paths, spaces are designated by *$20*, so "testing 2nd line" is the string that is concatenated to the *display* variable
* The newline escape character is also concatenated again so any new addition will be on a new line
* The *display* variable then becomes "greetings\ntesting 2nd line\n" and is displayed to the screen

## Part 2

```java
@Test
public void testReverseInPlace2(){
  int[] input = {1, 2, 3};
  ArrayExamples.reverseInPlace(input);
  assertArrayEquals(new int[]{3, 2, 1}, input);
}
```
- The above code is a JUnit test that has a failure-inducing input

```java
@Test
public void testReverseInPlace(){
  int[] inupt = {3};
  ArrayExamples.reverseInPlace(input);
  assertArrayEquals(new int[]{3}, input);
}
```
- The above code is a JUnit test that doesn't induce a failure

![Symptom1](Symptom1.png)
- 


![Symptom2](Symptom2.png)

