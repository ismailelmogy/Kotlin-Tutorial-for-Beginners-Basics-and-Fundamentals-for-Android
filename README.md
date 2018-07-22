# Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android

In this documentation we will going with the basics of kotlin for Beginners .

### First Step to start coding by Kotlin : Install JDK and Intellij IDEA.

 You can watch the video of installation from  [Here](https://www.youtube.com/watch?v=toesg2HLMSs&index=2&list=PLlxmoA0rQ-LwgK1JsnMsakYNACYGa1cjR)

**  Main method in java

``` java
public static void main(String[] args){

}
```
equals in Kotlin 

``` kotlin
fun main(args : Array <String>){

}
```
** Simple example :
```
fun main(args : Array<String>){
    println(" Hello World ")
}
```
> output : Hello World 

### Some points you should aware of them 

 - The compiler in kotlin convert .Kt file  into .class file
 
 - Unit stands for void in Kotlin
 
 - no semicolon ( ; ) in kotlin in the end of each statement
 
 - We don't need the concept of static , each function by default is static.

---------------------------------------------------------------------------------------------------------------------------------

### " Hello World " in Kotlin : How it works ?
 
    No Need of class

![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/No%20need%20of%20class%20in%20kotlin.png )

How Does it works?

- Java Demands class files.

- Kotlin needs JVM in runtime similar to java.

Does Kotlin creates a class internally?

  - Yes

    The kotlin compiler internally creates a class file which is loaded into memory for execution in runtime.
  --------------------------------------------------------------------------------------------------------------------------------
   ### Kotlin programming Series
    Quick overview of Basic Syntax
    - Functions 
    - Variables 
    - Class 
    - Constructor 
    - Comments
    
   * Inline Comment :
    
 ``` kotlin
    // This is a inline comment
 ``` 
    
   * MultiLine Comment : 
   
 ``` kotlin
   /**
   * This is comment in line 1
   * This is comment in line 2
   */
 ``` 
 
 * Declaring variables :
 ``` kotlin
    var myString = "Hello World"
    var myNumber = 10
    var myDecimal = 1.1
 ``` 
   *another way :* 
  ``` kotlin
      var myString :String    // Mutable String
      myString =  "Hello World"
      myString = " Another World "
  ``` 
  
 * Declaring constant variables :
 
   ``` kotlin
       val myAnotherStr = " My Constant String  Value" // Immutable String
   ``` 
   
  * Declaring new object of any class :
  ``` java
  
    Person personObj = new Person( ) //  code in Java
  ```
   equals in Kotlin
  
  ``` kotlin
  var personObj =  Person() // code in kotlin
 
  ``` 
  
   
