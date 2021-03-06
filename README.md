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
 
 - No semicolon ( ; ) in kotlin in the end of each statement
 
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
  
  In Java we declare new object of any class By this way  : 
  ``` java
   Person personObj = new Person() // we consider that there is a class called Person
   
  ```
  But in Kotlin there is no keyword (new) like this example :
  
   ``` kotlin
   // code in kotlin 
  var personObj =  Person()  
  ``` 
  
   * String Interpolation : 

  In Java you use concatenation like this :
  ``` java
  System.out.println("The name of the person is " + personObj.name);
   
  ```
  But in Kotlin we use the concept called String Interpolation like this example :
  
  ``` kotlin
   fun main(args: Array<String>) {
    var personObj = Person() // Declare the object of the class
    personObj.name = "ismail elmogy"
    println("The name of the person is ${personObj.name}" )  // String Interpolation
    
}

class Person {
    var name = " "
}
  ``` 
 * REPL stands for : Read-Eval-Print-Loop
 
 You can use it inside IntelliJ from Tools --> Kotlin ---> Kotlin REPL
 
 ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/REPL.png)
  
  
  * Data Types:
  
  All are objects and no primitive data types in Kotlin.
  
  ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/Data%20Types%20in%20Kotlin.png)
  
 Some examples of declaring data types in Kotlin :
 
 ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/Declaring%20data%20types%20in%20kotlin.png)
 
 * Var vs Val :
 
 
 ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/Var%20vs%20Val.png)
 
 * Kotlin String Templates (Interpolation):
 
      instead of using concatenation in Kotlin , You can use Interpolation.
  
  example:
  
   ``` kotlin
        val name = "sam"
        val str = "Hello " + name
        println(str)
   ```
  
   You can make it better in Kotlin like this :
   
   ``` kotlin
        val name = "Sam"
        val str = "Hello $name"
        println("The statement is $str . The number of characters in the statement are ${str.length}")
   ```
  *another example :* 
  
   ``` kotlin
         val a = 10
         val b = 5
         print("The sum of $a and $b is ${a+b}")
   ```
   
   *another example of Interplation:*
   
  
   ``` kotlin
       fun main(args : Array<String>){
       var rect = Rectangle()
       rect.length = 10
       rect.breadth = 5

    println  ("The length of the rectangle is ${rect.length} and the breadth of the rectangle is ${rect.breadth}" +
            " The area of the rectangle is ${rect.length *rect.breadth}")

}

class Rectangle {
    var length : Int = 0
    var breadth : Int = 0
}

   ```

  * Ranges in Kotlin :
  
  ``` kotlin
  
    val r1 = 1..5
    // This range contains the number 1,2,3,4,5

    val r2 = 5 downTo 1
    // This range contains the number 5,4,3,2,1

    val r3 = 5 downTo 1 step 2
    // This range contains the number 5,3,1

    var r4 = 'a'..'z'
    // This range contains "a", "b","c",...,"z"

    var isPresent = 'c' in r4  
    print(isPresent) // output : true

    var countDown = 10.downTo(1)
    // This range contains the number 10,9,8,..,1

    var moveUp = 1.rangeTo(10)
    // This range contains the number 1,2,3,..,10
  ``` 
--------------------------------------------------------------------------------------------------------------------------------

* Control Statements in Kotlin :

- If as expression
     
     example :
     
     ```kotlin
      val a = 2
      val b = 5
      var maxValue : Int

      if(a > b)
         maxValue = a
      else
         maxValue = b
       print(maxValue)
     ```
     > output : 5
     
     same example by using if as expression :
     ```kotlin
      val a = 2
      val b = 5
      var maxValue : Int = if(a > b)
                    a
               else   
                    b
     println(maxValue)
    ```
     
 - When as expression
     
      example :
     
      ```kotlin
        val x = 5
        when(x){
          0,1 -> println(" x is 0 or 1 ")
          2 -> println(" x is 2 ")
         in 11 .. 20 -> println("x is in the range from 11 to 20")
          //  You can use !in 11..20 ! means not
         else ->   //  like the default value in Switch
         {
           println(" x value is unknown")
         }
           }
      ```
     
     
     *another example :*
     
     
     ```kotlin
    val x = 3
    var str : String  =  when(x){
        1 -> " x is 1"
        2 -> " x is 2"
        else -> {
            "x is unknown"
        }
       } 
     ```
    --------------------------------------------------------------------------------------------------------------------------------
    
*  Iterators [Loops]
    
   -  For Loop

   -  While Loop

   -  Do While Loop

   -  Break and Continue Statements
     
      ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/loops%20or%20iterators.png)
       
     * For Loop :
     
       ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/For%20Loop.png)
      
      example :
      
      ```kotlin
       for (i in 1..10){
       if( i % 2 == 0){
           print(i)
           print(" ")
       }
      }
      ```
      output :
      > 2
        4
        6
        8
        10
      
      * While Loop :
      
      ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/While%20Loop.png)
      
      ```kotlin
     var i :Int = 1
    while (i <= 10){
        if(i % 2 == 0){
            print(i)
            print(" ")
        }
        i++
       }
     }
    ```
    output :
      > 2
        4
        6
        8
        10
        
      * Do While Loop :  
      
        ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/Do%20While%20Loop.png)
        
        ```kotlin
        var i: Int = 1
        do {
        if (i % 2 == 0) {
            print(i)
            print(" ")
           }
         i++
          } while (i <= 10)
        ```
     output :
      > 2
        4
        6
        8
        10
        
       
     *  Break Statements :     
        
        ```kotlin
         for ( i in 1..10){
        print(i)
        print(" ")
        if (i == 5)
             break
        }
        ```
           
    output :
      > 1
        2
        3
        4
        5
     
     another example:
        
      ```kotlin
       for(i in 1..3){
          for(j in 1..3){
          println("$i  $j")
            if(i== 2 && j == 2)
             break
             }
           }
      ```
   
   output : 
   
   ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/break%20statement%20in%20nested%20for%20loop.png)
   
   another example:
        
    ```kotlin  
    myLoop@ for ( i in 1..3){
    for( j in 1..3){
         println("$i $j")
         if (i == 2 && j == 2)
             break@myLoop
          }
        }
    ```
           
      output : 
   
   ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/exit%20the%20%20outside%20for%20loop%20with%20break%20statement%20.png)
   
      *  Continue Statements :   
      
      ```kotlin
       for (i in 1..10){
      if(i == 5)
          continue
      println(i)
       }
      ```
        
      output : 
   
   ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/continue%20at%205%20from%201%20to%2010.png)
   
   another example:
        
    ```kotlin  
    for (i in 1..10){
      if(i % 2 == 0)
          continue
      println(i)
    }
    ```
           
      output : 
   
   ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/odd%20numbers%20with%20continue%20statement.png)
   
     another example:
        
    ```kotlin  
    outer@ for (i in 1..3){
    for (j in 1..3){
        if ( i == 2 && j == 2)
            continue@outer
        println(" $i $j")
    }
   }
    ```
           
      output : 
   
   ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/outer%20for%20with%20continue%20statement.png)
   
  
   -----------------------------------------------------------------------------------------------------------------------------
   
    *  Kotlin Functions :
    
    
  ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/Kotlin%20Functions%20Basics%20and%20syntax.png)
  
  example :
  
   ```kotlin  
    fun main(args: Array<String>) {
    var sum = add(5, 7)
    println(" Sum is $sum")
    }
     fun add(a: Int, b: Int): Int {
    return a + b
          }
   ```
  
  output :
  
  > Sum is 12 


   * Kotlin Functions as Expression :
   
   
   ```kotlin  
   fun main(args: Array<String>) {
    var maxValue = max(10, 6)
    println("The greater number is $maxValue")
      }

   fun max(a: Int, b: Int): Int =
        if (a > b)
            a
        else
            b
   ```
   
   output : 
   
   > The greater number is 10

-----------------------------------------------------------------------------------------------------------------------------
   
  *  Interoperability:

      -  You can call Java Functions from Kotlin and Kotlin Functions from Java .
      -  You ca n have Java and Kotlin files with same project .
      
    
    
     ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/How%20Java%20and%20kotlin%20code%20runs%20.png)
     
       
     ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/example%20of%20converting%20kotlin%20file%20after%20compilation%20.png)
     
     You can see a simple example of using java and kotlin together from  [Here](https://github.com/ismailelmogy/KotlinProgramming)
     

 *  Default Functions with Interoperability:
 
     
     ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/Kotlin%20Default%20Functions%20with%20Interoperability%20.png)
     
     
     ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/JVMOverloads%20for%20Interoperability.png)
     
     
     You can see a simple example of that in the second commit of this project from  [Here](https://github.com/ismailelmogy/KotlinProgramming)
     
     
 *  Named Parameters:
 
    - It's a pure kotlin feature. Not present in Java.
   
   ```kotlin  
     fun main(args: Array<String>) {
     findVolume(length = 10,breadth = 5 ,height = 20)
     }

  @JvmOverloads
  fun findVolume( breadth : Int , height : Int = 10,length : Int) {
    println("length  is  $length")
    println("breadth is $breadth")
    println("height is $height")
   
   }
   ```
   
      
   *  Extension Functions:
   
      ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/Extension%20Functions.png)
   
    
   ```kotlin  
   fun main(args : Array<String>){
    var student = Student ()
    println(" Pass status : " + student.hasPassed(57))
    println(" Scholarship Status : "  + student.isScholar(57))
   }

fun Student.isScholar (marks: Int) : Boolean{
    return marks > 95
  }

class Student{
    fun hasPassed(marks : Int) : Boolean{
        return  marks > 40
    }
   }
   ```
     
   
   output : 
   
   >  Pass status : true
   
   >  Scholarship Status : false
                
   another example:
   
   ```kotlin  
 fun main(args : Array<String>){
    val str1 : String = "Hello "
    val str2 : String = "World"
    var str3 : String = "Hey "
    println(str3.add(str1,str2))
    val x:Int = 6
    val y:Int = 10
    val greaterVal = x.greaterValue(y)
    println( greaterVal )
}

fun String.add(s1 : String , s2 : String): String{
    return this + s1 + s2;
}

fun Int.greaterValue(other : Int) : Int{
    if( this  > other)
        return this
    else
        return other
}
   ```
   
   output : 
   
   > Hey Hello World
   
   > 10
   
   
   * Infix Function:
   
     -  All infix functions are extension functions But all extension functions are not infix functions.
     -  Infix function just have one parameter.
   
   
   ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/Infix%20Functions.png)
   
     
   ```kotlin  
   fun main(args : Array<String>){
    val x:Int = 6
    val y:Int = 10
    val greaterVal = x greaterValue y     //   x.greaterValue(y)
    println( greaterVal )
  }
 
infix fun Int.greaterValue(other : Int) : Int {   // Infix Function and also Extension Function
    if( this  > other)
        return this
    else
        return other
   }
   ```
   
    output : 10
     
   * TailRec Functions [Recursive Functions] :
       
       
       ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/TailRec%20Functions.png)
      
 ```kotlin  
   fun main(args : Array<String>){
    println(getFibonacciNumber(8, BigInteger("0"),BigInteger("1")))
    // 0 1 1 2 3 5 8 13 21 34 ... series 
 }

 tailrec fun getFibonacciNumber(n : Int ,a :BigInteger , b : BigInteger): BigInteger{
    if ( n == 0)
        return b
    else
       return  getFibonacciNumber(n - 1 , a + b ,a)
   }
 ```
    output : 13
    
-----------------------------------------------------------------------------------------------------------------------------

* Object Oriented in Kotlin :

   -  Class Definition, init Block and Primary Constructor :
  
        ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/class%20definition_init%20block%20and%20primary%20constructor.png)
        
     example:
  ```kotlin
  fun main(args : Array<String>){
    var student = Student("Ismail Elmogy")
  }
  class Student(var name : String){
    init{
        println("Student has got a name as $name")
         }
    } 
   
  ```
  
      output : Student has got a name as Ismail Elmogy
      
    
    -  Secondary Constructor :
     
          - You can not use the secondary constructor without calling the primary constructor in it.
          - You can not define any property as a parameter of the secondary constructor.
          
          example:
  ```kotlin
  fun main(args : Array<String>){
    var student = Student("Ismail Elmogy",30)
    println(student.id)
    }
    class Student(var name : String){
    var id:Int = -1
    init{
        println("Student has got a name as $name")
    }
    constructor(name :String,id : Int) : this(name){
        this.id = id
    }
  ```
  
      output : Student has got a name as Ismail Elmogy
               30   
    
     - Inheritance in Kotlin :
     
            By default classes are : public and final. For Inheritance you need to make a class 'open'.
     
     
     ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/Inheritance.png)
   
        
     ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/Types%20of%20Inheritance.png)
   
   
   
   ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/Super%20Class%20Any.png)
   
   
   
    ![alt tag](https://github.com/ismailelmogy/Kotlin-Tutorial-for-Beginners-Basics-and-Fundamentals-for-Android/blob/master/Inheritance%20in%20kotlin.png)
   
   
     example:
     
  ```kotlin
   fun main(args : Array<String>){
     var dog = Dog()
      dog.breed = "labra"
      dog.color = "black"
      dog.eat()
      dog.bark()

      var cat = Cat()
      cat.age = 7
      cat.color = "brown"
      cat.meow()
      cat.eat()
      
      var animal = Animal()
      animal.color = "white"
      animal.eat()

  }

  open class Animal{
    var color : String = " "
    fun eat(){
        println("Eat")
    }
  }

  class Dog :Animal() {
    var breed : String = " "
    fun bark(){
        println("Bark")
    }
  }

  class Cat : Animal(){
    var age : Int = -1
    fun meow(){
        println("Meow")
    }
  }
  ```
     -  Overriding Properties and Methods during Inheritance
     
     example:
              
     ```kotlin
   fun main(args : Array<String>){
    var dog = Dog()
    dog.eat()
    println(dog.color)
    var cat = Cat()
    cat.eat()
    println(cat.color)
  }
  open class Animal{
    open  var color : String = "White"
    open fun eat(){
        println("Animal is Eating")
    }
  }

  class Dog :Animal() {
    var breed : String = " "
    override var color ="Black"
    fun bark(){
        println("Bark")
    }
    override fun eat(){
        super<Animal>.eat()    // Animal Eating
        println("Dog is eating")
    }
  }

  class Cat : Animal(){
    var age : Int = -1
    override var color = "Brown"
    fun meow(){
        println("Meow")
    }
    override fun eat(){
        println("Cat is eating")
    }
  }

     ```
          output: Animal Eating
                  Dog is eating
                  Black
                  Cat is eating
                  Brown
     


   -  Kotlin Inheritance with Primary and Secondary Constructors :
  
  
             
     ```kotlin

   fun main(args : Array<String>){
    var dog = Dog("Black","Pug")
    }

    open class Animal {
     //    init {
     //        println("From Animal Init: $color")
     //    }

    var color : String = " "
    constructor(color: String){
        this.color = color
        println("From Animal: $color")
    }
      }

      class Dog : Animal {
              var breed: String = ""
               //    init {
               //        println("From Dog Init: $color and $breed")
               //    }

    constructor(color: String , breed : String) : super(color){
        this.breed = breed
        println("From Dog: $color and $breed ")
    }
      }
     ```
   
   
   
