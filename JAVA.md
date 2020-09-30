# JAVA Day 1
## Date: 21st August 2019   UNIT 1

## Introduction
* Java was initiated by ```James Gosling, Mike Sheridan and patrick Naughton``` at ```sun Microsystems``` in ```1991```
* initially named as ```Oak```
* Originally designed for interactive TV
* Before jdk 1.6 , java was not pure object oriented programming because it used variables not objects that is using primitive ```data types``` instead of project
    ```e.g,. int a;```
* Though from ```jdk 1.6``` or ```java 6``` , it started using ```wrapper ``` classes to become ```pure object oriented programming```
* <u> wrapper classes  </u>  these are used to make objects of primitive data types
    ```e.g., Integer a=new Integer(5);```

## Features of JAVA
1. Simple
    * Syntax similar to C++
    * no use of pointers
    * no need to remove unreferenced pointers

2. OOP's
    * Pure Object oriented language because we are not able to execute a single line of statement in java without using class and objects ```(Interview special)```

3. Platform Independent
    * Once a program is compiled then it can run anywhere and in any system
    * not produce machine specific code
    * software based platform independence
    * Software run on top of other platform
    * It has 2 components:
        1. Runtime environment
        2. Application Programming Interface
    
    #### Why JAVA is platform independentant?
    * Inside ```.exe``` file the code is translated to OS internal commands in C++
    * For example , a ```print``` statement replaces with ```display``` function to print something on ```windows``` console  in C++
    * In Java , after compiling the file created is ```.class``` and not ```.exe``` 
    * The ```.class``` file contains ```byte code``` and is read by ```interpreter``` at run time
    * JAVA program runs inside JVM
    * Uses run time environment of its own

5. Robust
6. Portable
7. High Performance
8. Multi Threading 
9. Dynamic
10. Interpreted 

* Class Loader seperate local file system form network imported files
* byte code verifier to check the code frament for illegal code

## Concepts of OOP's

### Class
* Collection of member variables and member functions
* blueprint to construct object
* By default all members are public in JAVA
* User defined data type
* It has access specifiers private, public, protected
* class is a logical representation
* Things defined inside class are the properties of the objects
* Example
```java
class Lamp
{ // instance variable
private boolean isOn;
//method
public void turnOn(){isOn}}
```

### Object
* instance of a class
* Object is a real world entity
* Need object to access class members
```java
class Lamp
{
    public static void main(String[] args)
    { 
        Lamp l1 = new Lamp(); // create l1 object of Lamp CLass
        Lamp l2 = new Lamp(); // create l2 object of Lamp Class
    }
}
// Object is ```new Lamp```
// l1 is a referenced variable of specified class
```

### Abstraction
* show only essential details
* focus on what class can do and what it must do
* Done in java using interface
* e.g., Email send system
* A phenomena by which we just show essential details to the user and hiding the rest

### Encapsulation
* Wrapping up of data together into a single unit class
* hiding data
* focus on how to achieve the functionality
* Done in java using access modifiers
* e.g., CSE department
* binding the accessibility of some variable inside a class


## Inheritance
* Inheritance is the process by which we can use existing code
* Inheritance is the property by which object of one class can acquire the property of other class
* <u> Base Class or Super Class</u> the class which has main properties
* <u> Derived Class or Sub class </u> inherits the existing properties of a class
* Reusability of code


### Types Of Inheritance
* Multiple inheritance of classes is not allowed in ```JAVA``` because of ```Diamond Problem``` and it has a solution of ```Virtual Classes```
* virtual classes requires pointers but there are no pointers in java
1. Single Level Inheritance
    ``` 
    A
    |
    B
    ```
2. Multi Level Inheritance
    ```
    A
    |
    B
    |
    C
    ```
3. Multiple Level Inheritance (#### Not present in JAVA)
    ```
    B           C
    |___________|
          |
          A
    ```
4. Hierarichal Inheritance
    ```
            A
        ____|____  
        B       C
    ```

## Polymorphism
* One name many forms
* It depends on the instance of objects
* It can be achieved using ```method overloading```
* It is of 2 types
    1. Static Polymorphism ( compile )  -> method overloading, constructor overloading  
    2. Dynamic Polymorphism ( run time ) -> method overriding
    
```java
int getdata (int,int)  //1   
void getdata(int,int)  //2
int getdata(float,float)  //3
void getdata(int,float)   //4
int getdata(float,int)   //5

/* 
1 & 2 are not overloading
1 & 3 are function overloading
1 & 4 are function over loading
1 & 5 are function over loading
*/
```
* 3 rules to find overloading(polymorphism)
    1. ignore the data type declaration ( int, void, char etc)
    2. Name of methods should be same 
    3. no of arguments or types of arguments or order of argument should be different
    

## Java Virtual Machine
* ```JVM``` is the component due to which ```java``` is very ```powerful```
* It is a combination of ```java interpreter and operating system```
* It requires compiled file ```.class``` 
* Communicates between ```.class``` file and OS
* Decodes the ```.class``` file
* JVM is platform dependent and because of JVM java programs are platform independant
* ```JAVA SOFTWARE``` is platform dependant but not its ```programs```


## JDK(Java Development Kit) and JRE(Java Runtime Environment)
* JRE is a collection of ```JVM + Java Libraries```
* Collection of ```JRE + Java Development Tool Kit``` is ```JDK```
* The ```.class``` file contains encoded instruction for the java interpreter and are known as java byte code


## Data Types
* Data types are of two types
    1. Primitive -> defined in language by default
    2. Non Primitive -> user defined data structure
* Primitive Data Types
    1. Numeric 
        * Integer (Int, Float or Double)   
        * Character (char)
    2. Boolean
* Non Primitive
    array,stack,queue
* Types of Size
    32 - bit System
    1. (1) byte
    2. (2) short
    3. (4) int
    4. (8) long
    5. (2) char
    6. (4) float
    7. (8) double
   
    64 - bit system
    1. (8) float
    2. (16) double
    3. (1) boolean  ```till jdk 1.3```
    4. (1 byte) boolean  ```after 1.3 jdk```
* Short is important and char is also used in short

# DATE: 27 August 2019

* ## ```  Narrowing of Data Type is not Allowed JAVA ```
## What is narrowing of Data Type?
* b < S < I < L < F < D   these are data types
* this narrowing is not allowed in java

## Why we can store more data in ```char``` as compared to ```short```
* In short or integer type data type , the storage size is 15 bit due to presence of signed bit 
* In char data type , the storage size is 16 bit as there is no signbit
* 2 byte = 16 bit

## Variable
* Name of a memory location
* Each variable has a datatype
* 4 rules to define a variable are:
    1. the variable name should not start with a numeric digit
    2. variable name should not contain any whitespace
    3. variable name should not contain any ```language keywords``` or ```primitive words```
    4. We can not use special character except ```_```

## Types of variables in JAVA
* There are 3 types of variable
    1. Local Variable
    2. Instance Variable
    3. Static Variable
* <u> Local Variable </u> ~>  Variable defined inside a method and accessed inside that method only
* <u> Instance Variable </u> ~> Value is object specific , value not shared with other instances , Declared inside class but outside the body of method
* <u> Static Variable </u> ~> Declared with static keywords , Shared among all instances , Memory allocated once at compile time, Should be initialized first that is each object will be able to change value of class variables and values will be modified for each object

```java
class Demo 
{
    int a = 50; // instance variable
    static int b = 100; // static variable
    void func()
    {
        int x = 90; //local variable
    }
}
```

## Array
* Collection of homogenous items stored under one name
* size is fixed
* it can be used as a object
* Syntax
```java
// pre declaration of array
int[] a1 = new int[5];  // type name[] = new type[size]

// post declaration of array
int a1[] = {1,2,3,4,5}; // array as referenced variable = size

int []a, b, c[];  // pre declaration gets associated with all variables till semi-column in its right side
// here a is 1d array , b is 1 d array and c is 2d array
```
* no of columns can be variate in JAVA
* To find the length or size of array that is no of elements in array, we use the function ```variable-name.length```
* For 2D array, ```variable-name.length``` will return no of rows and ```variable-name[i].length``` will return no of elements in ```ith ``` row
* For 3D array, ```variable-name.length``` will return no of 2D array in 3D array
```java
int [][]a[]= new int[6][4][2]  // 3D array
/*
| [ [ ] ] | [ [ ] ] | [ [ ] ] |
*/

``` 

### <u> Variable Length of Array </u>
    ```
    |0|1|2|3|4
    |0|1|
    |0|1|2|
    |0|2|3|4|5|6|
    |0|
    ```


## Variable Declaration
* 2D Array
```java
int a[][] = new int[5][4];
int []a[];
int [][]a , b[]; // 3d array
```

# Date: 29th August 2019

## Expression
* built using values,variables, operators and method calls
* (a*2) is an expression and b+ (a*2); is a statement
* Expression is a clause, and the statement is the complete sentence since it forms the complete unit of execution
* expression produces intermediate result

## Types of expression:
* produce a value
* assign a variable
* those that have no result but have a side effect because an expression can include a wide range of elements such as method invocations or increment operators that modify the state.

## Operators
* symbols that operates on one or more arguments to produce results
* Arguments here are operands
    ```
    result = a+b
    ```

## Types of operators
1. Assignment operator
    * lvalue = rvalue -> rvalue is assigned to lvalue
2. Arithmatic operator
3. Relational Operator
    * ```==``` and ```!=``` are object reference operators
4. Logical Operator ```AND (&&)  OR(||)   NOT(!)```
5. Logical Operator bit level
    ```
    AND &
    OR |
    XOR ^
    NOT ~
    ```
    ```java
    int a= 10; // 00001010 = 10
    int b = 12; // 00001100 = 12
   ```
   * logical bit wise opeator checks first condition before proceding further
   * logical operator checks all conditions before taking any conditions
   * Number is represented into 32 bit(Theoretically)
   ```
   result = a & b
   * result is negative then the answer will be 2's complement
   ```
6. Shift Operators
    * Shift Operators(bit level)
    * Shift Left  ```<<``` Fill with zeros
    * Shift Right ```>>``` Based on Sign
        * if number is positive then it will be filled with ```0```
        * if number is negative then it will be filled with ```1```
    * Shift Right ```>>>``` Fill with zeros
    ```
    a = 0011
    a << 2 
    0011 ~> 001100

    a >> 2
    0011 ~> 0000

    b = -4
    b >> 2
    111111111111111111111111100 ~> 11111111111111111
    0100 ~> 0001
    -4 ~> -1 (twos complement)

    a >>> 2
    0011 ~> 0000
    3 ~> 0
    ```

## Control Structures
* Block of program to change the execution of program based on logic and values
* 3 types of control structures are:
1. Conditionals
    1. IF
    ```java
    if (condition)
    {
        //codes
    }
    //codes after if
    ```
    2. if else
    ```java
    if (condition) {

    }
    else if {

    }
    ```
    3. nested if else
    4. switch
    ```java
    switch (condition)
    {
        case 1 : //code
        case 2 : //code
    }
    ```

2. loop
    1. For
    ```java
    for(initialization;testExpression;update)
    {
        //code inside for loop's body   
        // to run it for infinite just testExpression == True
    }
    ```

    2. While loop
    ```java
    int i = 0;
    while(condition)
    {
        statement
        condition update
    }
    ```
    3. Do While
        * It executes atleast once

3. Jump Statements
* unconditionally transfer the program control to another part of program
    1. Continue
    2. Break
    3. Return ~> it immediately quit the current method and return to the calling method

## Basic Syntax
```java
class class-name-user-defined{
    // access-specifier method-static void main(String[] args)
    public static void main(String[] args){
        ... ..      ...
        n=3;
        result = square(n);
        ... .. ...
    }
    private static int square(int i){
        // return statement
    }
    
}
// static method ~> we dont need any object to call the function/method
// String[] is a variable length array which stores the input from cmd
// args is just a variable name which can be user-changeable
```
* file name should be similar to class name but its not compulsory
* at compile time we need ```file-name.java```
* at run time we need ```class-name.class```

                <-----------------The End of Unit 1---------------------->

# Date 3rd September 2019
* To run any code
    1. Save the file with code
    2. Open cmd and run ```javac file-name.java```
    3. it will create a ```.class``` file
    4. to execute ```java file-name```
* Default package always associated with java code is ```java.lang```
* Any word starting with ```Capital Letter``` is a ```Class```
* All methods are iitiated with ```small letters```
* To take input we use class ```java.util.*```
    ```java
        Scanner sc=new Scanner(System.in); // object of the same class
        System.out.print("enter the value of a: ");
        a = sc.nextInt();  // Camel Notation used in java
        // nextInt works same as scanf of C 
    ```
* ```random``` class produces ```17 decimal place``` digit
* Static method can only call other Static methods

## For Each Loop
* Syntax
```
for(data-type variable:iterable-structure)

for(int i:a[])
    further code
```

# Date 4th September 2019


## String
* <u> String </u>  ~> An array of characters is called String
* ```String``` is also a ```class``` in java which can be used by making objects
    ```
    String s = 'Deepak';
    ```
* String objects are immutable
* While creating the first object of any String always ```2 objects``` are created
* The two objects created are ```Heap``` and ```Constant```
* when creating further objects of similar String, the compiler checks the constant object for availablity , and if available then link to its reference else create another ```Heap```
* The Heap object is used to process or compute the String with other commands and Constant for Similar String checking

## Shallow Comparsion
* It is a functionality of java where Strings are compared with each other based on their referecnce variable and not on their actual value
* To compare two strings we use the function ```string-variable-name.equals(another-string-variable-name)```
* To compare two strings without ```CaseSensitive``` we use function ```String1.equalsIgnoreCase(String-2)```
* To convert String to ```Lower Case``` use the function ```toLowerCase()```
* To convert String to ```Upper Case``` use the function ```toUpperCase()```
* To find the charater in a string with ```index``` position use the function ```string-name.charAt(index-position)```
* Constructor can be made ```private``` using ```Single Turn Pattern```


# Date : 5th September 2019

## Inheritance
* To inherit one class in another , we use the function ```extends```
* All the classes being inherited by a ```Derived``` class are written seperated by ```,```
    ```java
    // created a base class
    class Super  // Java has a inbuild keyword super 
    {
        int a = 0;
        public void show()
        {
            System.out.println("A="+a);
        }
    }

    // created a derived class
    class Sub extends Super 
    {
        int b = 0;
        public void display()
        {
            System.out.println("B="+b);
        }
    }
    ```
* if we do not define a specific ```constructor``` in a class then ```compiler``` creates a constructor for the same ```class``` so that a user is able to make ```object``` of the ```class```

* We have three types of constructor
    1. Default ~> to initialise the variable with default data types
    2. Parameterised Constructor ~> Initialse the variables of the class defined by user at run time
    3. Copy Constructor ~> Previously existing objects are used to create new objects
* Constructor of Super Class can not be called in the derived class just by using its name
* To call the constructor ```Base``` class inside the ```Derived``` class we use the function ```super();```
* If we are using ```super``` keyword then it must be the ```FIRST``` executable keyword in the ```Sub``` or ```Derived``` class created by the ```user```
* If you define same variable as ```argument to a function``` and to be assigned, we can use keyword to differentiate the varaiables
    ```java
    class Sub extends Super 
    {
        int b = 9;
        public Sub(int b)
        {
            super(); // it calls the constructor of the Base Class
            this.b=b;
        }
    }
    ```

# Date : 6th September 2019

## Overloading
* Same name with different names or arguments

## Overriding
* Same name with same number and name of arguments

```java
class Super
{
    int a;
    public Super(int a) // constructor
    {
        this.a = a;  // instance variable
    }
    public void show()
    {
        System.out.println("A=" + a);
    }
}
class Sub extends Super
{
    int b;
    public Sub(int b)
    {
        Super(b*2);
        this.b = b;
    }
    public void display()
    {
        System.out.println("B="+b);
    }
}
class Day4Demo
{
    public static void main(String args[])
    {
        Sub obj = new Sub(10);
        obj.display();
    }
}
```
* ```this``` it differentiates instance variable with arguments
* In Inheriatnce(overriding) , the top variable(variable of base class) can store the Sub/Derived class object or variable where as Sub/Derived class can not do so
```java
Sub obj = new Super(10); // not possible
// where as
Super obj = new Sub(20); // is possible
```

## Method Overloading
```java
class Add
{
    int a , b;
    float c;
    public void getAB(int a,int b,float c)
    {
        this.a = a;
        this.b = b;
        this.c = c;
    }
    public void Sum(int a , int b)
    {
        System.out.println("Sum ="+(a+c));
    }
    public void Sum(int a, float c)
    {
        System.out.println("Sum = " + (a+c));
    }
}
class DayOverriding
{
    public static void main(String args[])
    {
        Add obj = new Add();
        obj.Sum(2,3);    
        obj.Sum(2,2.5); // By default double
    }
    // Sum =5
    // Sum = 4.5
}
```
---
# Date: 17th September 2019
# Unit 2 Types of Java Classes

## Content
1. Abstract Class
2. Static Class
3. Inner Class
4. Package
5. Interface
6. Wrapper Class,Access Control
7. Super,this,final keywords

## Abstract Class
* A class which is declared with the abstract keyword is known as an abstract class in Java. It can have abstract and non-abstract methods
* <b>Abstract</b> is a process of hiding the implementation
* It shows only essential things to user and hides the internal details
* Ways to achieve abstaction
    1. Abstract Class (0 to 100%)  ~> depends on developer
    2. Interface ( only 100%)
* Implementation
    1. must be declared with ```abstract``` keyword
    2. may have abstract method and non abstract method
    3. must have ```Atleast One``` abstract method and vice~versa
    4. it need to be ```extended``` means need to implement inherited
        * the abstract class will be the super class and need to be inherited in some class
    5. it cannot be ```instantiated```, means we can not create object of abstract class

## Abstract Method
* a method without definition is known as abstract method
* it must be declared with abstract keyword
* It must be override in sub class otherwise subclass will become abstract
* Syntax: ```abstract void function-name();```

```java
//abstract return_type Method_Name(ARGS)

abstract void fun(int,int);

abstract class Demo{
    int a,b;
    abstract void fun(int,int);
    void getdata(){
        a=10;
        b=20;
    }
}
```

## Interface
* Interface is a process to achieve abstraction
* interface is the just a blueprint of a class
* it has ```static``` and ```final``` variable ~> value will be constant for all objects
* it has only ```abstract``` method
* interface always be implemented
* it cannot be instantiated just like the abstract class
* It is not a class itself but tells the structure of the class
* Interface must be ```implemented``` where as class must be ```extended``` for ```abstraction```
* interface is a collection of abstract methods and constants
* Can not create ```object``` of ```interface```
* All methods declare in an interface are public abstract by default
* Till ```JDK 1.7``` , Non abstract methods are not allowed in interface
* From ```JDK 1.8```, we can define ```non-abstract methods``` inside ```interface``` as well
* Everything defined inside interface is public by default

```java
// A function with definition but do nothing can be stated as
void func-name()
{

}
```

```java
class A{
    //declaration and definition
}
interface A{
    //declaration only
    // all methods will be abstract
    // 
}
```
```java
interface name_interface{
    //declare variables
    //declare methods
}
interface Animal()
{
    int legs=4;
    void fun();
}
```

## Relation between Class and Interface
* Class extends Class
* Class implements Interface
* Interface extends Interface

## Multiple Inheritance in java by interfcae
```
        (interface)         (interface)
                |                 |
implements      |_________________|          
                        |
                      (Class)

        (interface)         (interface)
                |                   |
                |___________________| (extends)
                        |
                     (Class)
```

## Difference    
<img src="Images/ClassVsInterface.png"></img>

# Date 19th September 2019

## Package
* A java package is a group of similar types of classes , interfaces and sub-packages
* Package in java can be categorized in two form, built-in package and user-defined package
* ```Abstroict window Toolkit``` is ```AWT```
* There are many buil in packages such as java,lang,awt.javax,swing,net,io,util,sql etc

## Syntax for using Package
```java
package Name_Package;
import.....;
class......{
    statement...
}
// package must be the first line inside the source code file 
```
* Name_Package is the full path of directory separated by ```.```
* E.g., ```Desktop.Ju-Notes.JavaCode```

## Syntax for compile the package program
```
javac -d directory javafilename
javac -d . Demo.java  # example 1
```
* Package is used for classes in which main class function is not included

## Access Control
* It is of 2 types
1. Access Modifiers ~> Defines the accessibility limitations
    * Default
    * Private
    * Protected
    * Public
2. Non-Access Modifiers ~> it defines the functionality but not the accessibility
    * Static
    * Abstract
    * Final
    * Synchronized
* Modifiers provide some kind of feature or limitation to an data structure like class or object or methods

<table>
<tr>
<td>
Access MOdifier
</td>
<td>
within class
</td>
<td>
within package
</td>
<td>
outside package by subclass only
</td>
<td>
outside package
</td>
</tr>

<tr>
<td>
Private
</td>
<td>
Y
</td>
<td>
N
</td>
<td>
N
</td>
<td>
N
</td>
</tr>

<tr>
<td>
Default
</td>
<td>
Y
</td>
<td>
Y
</td>
<td>
N
</td>
<td>
N
</td>
</tr>

<tr>
<td>
Protected
</td>
<td>
Y
</td>
<td>
Y
</td>
<td>
Y
</td>
<td>
N
</td>
</tr>

<tr>
<td>
Public
</td>
<td>
Y
</td>
<td>
Y
</td>
<td>
Y
</td>
<td>
Y
</td>
</tr>
</table>


## Java Inner Classes
* Java ```inner class``` or ```nested class``` is a class which is declared inside the class or interface
* We use inner classes to ```logically group``` classes and interfaces in one place so that it can be more readable and maintainable, that is keeping data which is dependable upon each other can kept together
* It can access all the members of ```outer class``` including ```private data members and methods```
* It is a part of nested class
* Non static nested classes are known as inner classes

## Advantages of Inner Classes
* It can access all the members (data members and methods) of outer class including private

## Types of nested class
1. Non static nested class
    * Member inner class ~> normal inner class
    * Anonymous class ~> name is defined by compiler at the runtime, a class without name
    * Local Inner class ~> class which is defined inside a method
2. Static class
    * Static nested class

### Anonumous Class
* Name is decided by compiler
* Used in Artificial Programs
```java
// Anonymous inner class
abstract class Demo{
    public void show();
}
class testDemo{
    Demo p=new Demo(){ // Anonymous class... name will be decided by compiler at run time
        public void show(){
            S.o.p("Hello Demo");
        }
    };
    p.show();
}//end test demo

// another example
Demo1 d = new Demo1(
    new TestDemo(){    // starting of syntax of anonymous class
    void data()
    {
        ...
    }
}
);
// TestDemo is abstract class
```

## Local Inner Class
```java
class Demo{
    public void display(){
        class inner{
            public void show(){
                SOP("Local inner ");
            }
        
        }//local class ends
        inner obj=new inner()l
        obj.show();
    }//display ends here
}
```

## Static Inner Class
* can access static data members of outer class including private only
```java
class outer{
    static int a = 10;
    int b = 20; // not accessible
    static class inner{
        public void show(){
            s.o.p("value od a="+a);
        }//show ends
    }//inner class ends
}//outer class ends
```

## Final
* it can be applied to variable, method and class
* if we make a variable as final, then it become the constant. That means values of that variable can't be changed
* If we make a method as final then it can't be overridden . That means overriding of final methods are not allowed
* If we make a class as final then it can't be inherited

## Super
* The super keyword in Java is a reference variable which is used to refer ommediate parent class object
* super can be used to refer immediate parent class instance variable
* super can be used to invoke immediate parent class method
* super is used to invoke constructor of ```Super``` or ```base``` class

## This
* this can be used to refer current class instance variable
* this can be used to invoke ```current``` class method (implicitly)
* this() can be used to invoke current class constructor
* this can be passed as an argument in the method call

```java
class Demo{
    Demo(int a){
        x = a;
    }
    Demo(int a, int b){
        y=b;
        this(a)
    }
    Demo(int a, int b,int c){
        z = c;
        this(a,b)
    }
}
```
---

# Date : 9th October 2019
# Unit 3 Exception Handling

## Types of Errors:
1. Compile Time Error -> Some kind of ```Syntax error```
2. Run Time Error -> Not run due to ```environment error``` 
3. Logical Error -> Compiled and run but Error in some code input due to which we are not getting desired output

* ```Exception``` are the cause by which our programs get terminated or giving some wrong output
* If we get such error at ```compile time``` then Exception is known as ```Compile time``` exception in our program
* If we get  such error at ```execution time``` of the program then such errors are known as ```Run time``` exceptions

## Types of Exception
* ```Check``` and ```Uncheck``` exceptions are with respective to the ```compilers``` point of view
1. Compile Time Exception
    * These are also known as ```checked exceptions```
    * Examples
        * I/O Exceptions
        * SQL Exceptions

2. Run Time Exception
    * These are also known as ```unchecked exceptions```
    * Examples
        * Arithmatic Exception (due to some calculation mistake)
        * Array Index Out of Bound Exception

## Handling Exception
* There are two ways to handle ```exception```
    1. ```Throw```
        * All exceptions will be handled by compiler only
        * Program always gets successfully compiled
        ```java
        Class ABC{
            P.S.V.M(String args[]) throw {
                ......
                ...... // Exception occur
                ......
            }
        }
        ```
        * Does not compile when error occurs due to package missing issues
        * We can define the particular ```name of package``` for which error may occur
        e.g., ```IOException```
        * or just define the main class ```Exception```

    2. ```Try , Catch , FInally```
        ```java
        try {
            //Exception Code... the line of code in which we are expecting some exception to be generated
        }
        catch (Exception e) {
            // corrective measure of exception occurring in upper block that is in try block
        }
        finally {
            // it is executed always whether we are having error or not
        }
        
        ```
        * If we are defining ```try``` block then atleast one ```catch``` block is necessary to be defined
        * finally block is not necessary to be defined , its upto the developer
        * It is of 3 types:
            1. Try_catch with single catch
            2. Try_catch woth multiple catch
            3. Try_catch with nested try_catch
        
## User Defined Exception
* Generating a self customized exception and terminating the program as per our need


# UNIT 4 Input/Output Stream
* I/O stream can be implemented by two ways:
    1. Sequence of bytes
    2. Sequence of characters 
* ```File handling is performed using IO Stream```
* Stream can be defined as flow of data
* To work with any Stream, follow the steps:
    1. Import the specific stream package
    2. Create the object of concern I/O Stream
    3. Determine The input (make source using CLA or at compile time) and output points for work to be performed
* Object is supermost class of Java,for both pre-defined and user-defined classes
* Every Stream should be closed ```.close()``` before exiting the program

## Stream
* A stream is a sequence of data and is composed of bytes
* Default Stream: System.out,System.in,System.err, all are connected to console only


## Byte Stream
* Each class has an Input and Output Stream
* Available Classes are  of 7 types:
    1. Input (SYstem.in)
    2. Output (System.out)
    3. Filter Stream
    4. Buffered Stream ~> Tends to save the inputs to input stream and output to output stream which makes it faster at the moment of execution
    5. Data Stream ~> Used in networking tasks , A socket is generated between 2 systems trying to communicate with each other
        ``` |A|~~~> (Socket)~~~>|B|```
    6. Print Stream
    7. File stream ~> Specifically used for ```File Handling```
* to send some errors we can use ```System.err```

## Character Stream
* Reader and Writer
* It is again of 4 types
    1. Input Stream Reader
    2. Output Stream Writer
    3. Buffered Stream Reader/Writer
    4. File Reader/Writer

## Input Streamm class
* Java.io is an abstract class for all input stream
* Basic ```read()``` method read a single unsigned byte of data and returns the integer value of the unsigned byte
* ```read()``` returns ```-1``` at the EOF
* Every input stream should be closed before exiting the program

## Reading Multiple Bytes
* I/O is slow in comparison to memory access, limiting the number of reads and writes is essential
* The basic read() method only reads in a byte at a time
* The following two overloading read() methods read in multiple bytes into an array of bytes
    1. public int read(byte b[])
    2. public int read(byte b[], int offset=2)

## Reading from File Input Streams
* It obtains input bytes from a file.It is used for reading byte oriented Data
* To print certain character after reading using ```Input Stream``` then it will be required to change into character using ```char()``` method.
* To typecast a certain variable the syntax is like ```(char)variable_name```
* during file handling,when ```file.read()``` reaches ```EOF``` it returns ```-1```
* ```fil.read()``` ~> it does the work of fetching character as well as iteration of next byte/character

```java
import java.io.*;
class FileInputStreamDemo{
    public static void main(String args[]){ //CLA - command line arguments
        try {
            //Create a file input stream
            FileInputStream fis= new FileInputStream("Path" args[0]);
            //read 12 byte from file
            int i;
            while(i=fis.read() != -1) // at EOF byte is -1 which indicates the end of file
            {
                System.out.println(i);
            }//close file output
            fis.close()
        }catch(Exception e){ System.out.println("Exception:"+e)}
    }
}
```
* An example of Buffered Input Stream, it will increase the Execution Speed of the Program
```java
import java.io.*;
class FileInputStreamDemo{
    public static void main(String args[]){ //CLA - command line arguments
        try {
            //Create a file input stream
            FileInputStream fis= new FileInputStream("Path" args[0]);
            //read 12 byte from file
            BufferedInputStream bis = new BufferedInputStream(fis);
            int i;
            while(i=bis.read() != -1) // at EOF byte is -1 which indicates the end of file
            {
                System.out.println(i);
            }//close file output
            bis.close()
            fis.close()
        }catch(Exception e){ System.out.println("Exception:"+e)}
    }
}
```
## Output Stream Class Methods
* public void write(int)throws IO Exception ~> is used to write a byte to the current output stream
* public void write(byte[])throws IOException ~> is used to write an array of byte to current output stream
* public void flush()throws IOException ~> flush or remove the current output stream
* public void close()throws IOException ~> close the current output stream

* FileOutputStream~> it is an output stream used for writing data to a file
```java
public class FileOutputStream extends OutputStream
```
* Methods in FileOutputStream are:
    1. protected void finalize()
    2. void write(byte[] ary)
    3. void write(byte[] ary,int off,int len)
    4. void write(int b)
    and many more
```java
import java.io.FileOutputStream;
public class FileOutputStreamExample{
    public static void main(String args[]){
        try{
            FileOutputStream fout = new FileOutputStream("path of file");
            // to connect it with a buffer
            //BufferedOutputStream bout = new BufferedOutputStream(fout);
            fout.write(97); // instead we will use bout.write(97); and bout.flush();
            // flush() is used to forcefully write if some error occurs due to network issues
            fout.close(); 
            System.out.println("Success");
        }
        catch(Exception e){
            System.out.println(e);
        }
    }
}
```
```java
import java.io.FileOutputStream;
public class FileOutputStreamExample{
    public static void main(String args[]){
        try{
            FileOutputStream fout = new FileOutputStream("path of file");
            String s = "Pykid";
            byte b[] = s.getBytes();  //converting string into byte array
            fout.write(b);
            fout.close();
            System.out.println("Success");
        }
        catch(Exception e){
            System.out.println(e);
        }
    }
}
```
## Object Serialization and De-Serialization
(Will be taught later)

# Date: 6th November 2019
# Unit 5 Multi Threading

## Content
* Thread Life Cycle
* Multi Threading Advantage and issue
* Threading Synchronization
* Introduction to AWT Programming(Abstract Windowing Toolkit used for designing GUI)
* Layout, COmponenet and Event Handling
* Applet PRogramming
* Swing Component(All components in AWT and swing are same)

## Notes
* AWT components(Presentation and not working) are dependable on OS Platform where as Swing isn't
* Naming Difference in AWT and Swing is there ( JLabel(Swing) ~> Label (AWT) )
* Layout ~> Decision Taking as to where the component is to be added
* Component ~> Everything visible in a GUI is a component
* Container ~> It contains components. e.g., Frame/Window
* Panel ~> Used when we have some limitation, in panel components are added and Panel is used as an component is Frame
* Event Handling ~> Controls the working of our GUI either click or drag or type everything
* Applet is an java program that is implemented in HTML Code(will be studied later)
* A process needs to perform ```Context Switching``` to communicate with other processes which is not required with threads
* Each process has an seperate address in memory
* If in a program no threads are defined then it means it has ```1 internal thread``` running in it

## MultiThreading
* Thread is a ```smallest unit of process``` or lightweight sub-process
* ```Multi threading``` is a process of executing multiple threads simultaneously
* Multiprocessing and Multi Tasking is used to achieve multitasking
* Threads used a ```shared memory area``` that is the same ```address space```
* It is mostly used in Games and animation

## Advantage of MultiThreading
* It doesn't block the user because threads are independent and you can perform multiple operations at same time
* saves time as many operations can be performed together
* Threads are ```Independent``` , so it doesn't affect other threads if an exception occurs in a single thread

## Thread Class and Methods
* start() ~> To start a thread
* run() ~> to do an action of thread
* getName() ~> gives name of thread
* setName() ~> changes name of thread
* getId ~> return id of thread
* isAlive() ~> tests if thread is alive
* yield() ~> pause current running thread temporarily and allow other threads to run

## Life Cycle of Thread
* There are four states of a thread life cycle
    1. New ~> Thread is just created
    2. Runnable ~> Thread is ready to execute (after start() method is called )
    3. Running ~> Thread is executing (after run() method is called)
    4. Terminated ~> Thread is completed or aborted


# Date 19/11/2019

## AWT
* Java AWT(Abstract Window Toolkit) is an API to develop GUI or Window-based applications in java
* Java AWT components are platform-dependent
* WT is heavyweight i.e, its components are using the resources of OS
* The java.awt package provides classes for AWT api such as TextField , Label,TextArea,RadioButton, CheckBox , CHoice ,List etc

## Container
* The Container is a component in AWT that can contain another components like buttons, textfields etc. The classes that extends COntainer class are known as container such as Frame , Dialog and Panel
* Panel is never visible unless a component is added to it and The panel is fixed to a specific layout
* Useful Methods of COntainer Class are:
    1. public void add(Component c) ~> Inserts a component on this component
    2. public void setSize(int width,int height) ~> sets the size(width, Height) of the component
    3. public void setLayout(LayoutManager m) ~> defines the layout manager for the component
    4. public void setVisible(boolean status ) ~> changes the visibility of the component,by default false
* By default layout is Flow Layout

```java
import java.awt.*;
class DemoAWT extends Frame{

    DemoAWT(){
        Button b=new Button("Click me");
        b.setBounds(x1,y1,x2,y2); //setting button position
        add(b); //adding button into frame
        setSize(300,300); //frame size is 300x300;
        setLayout(null); //no layout manager
        setVisible(true); // now frame will be visible, by default not visible
    }
    public static vod main(String args[]){
        DemoAWT obj=new DemoAWT();
    }
}
```

## Event Handling
* Changing the state of an object is known as an event
* Event Classes ~> Listner Interface(Action Perform)
    1. ActionEvent ~> ActionListner
    2. MouseEvent ~> MouseListner and MouseMotionListner
    3. MouseWheelEvent ~> MouseWheelListner
    4. KeyEvent ~> KeyListner

* We can define the definition of a button with its declaration only by using ```anonymous class```


## Layout Manager
* The Layout Manager are used to arrange components in a particular manner.Layout Manager is an interface that is implemented by all the classes of layout manager
* BorderLayout ~> Used to arrange the components in five regions where each region may contain one component only.
    1. NORTH ~> public static final int NORTH
    2. SOUTH ~> public static final int SOUTH
    3. EAST ~> public static final int EAST
    4. WEST ~> public static final int WEST
    5. CENTER ~> public static final int CENTER
* If Single Component is added, it takes the space of all other regions as well


## Java Grid Layout
* The GridLayout is used to arrange the components in rectangular grid.One component is displayed in each rectangle
* Constructors of GridLayout CLass
    1. GridLayout() : creates a grid layout with one column per component in a row
    2. GridLayout(int rows, int columns) : creates a grid layout with the given rows and columns but no gaps between the components
    3. GridLayout(int rows,int columns,int hgap, int vgap) : creates a grid layout with the guven rows and columns alongwidth given horizontal and vertical gaps


## Applet
* Applet is a special type of program that is embedded in the webpage to generate the dynamic content.It runs inside the browser and works at a client side

### Advantages
1. It works at client side so less response time
2. Secured as it uses its own internal memory and data management systems to block any unauthorized data access. 
3. It can be executed by browser running under many platforms, inlcuding Linux,Windows , Mac OS etc

### Drawbacks
* Plugin is required at client browser to execute applet

## Card Layout
* Applied when components are required to be structured over one another
* Makes the above component disable or invisible making the below component active or visible

<br>

# CRT Classes
* Basic Questions related to Java that could be asked will be taught in java class

1. Difference between inner class and sub class?
    ```
    * inner classes are in the same file, whereas subclasses can be in another file, maybe in another package.
    * You cannot get an instance of an inner class without an instance of the class that contains it.
    * inner classes have the methods they want, whereas subclasses have the methods of their parent class. Subclasses can, of course,    define additional methods, but they'll always have those of their parent.
    ```
2. Access specifiers in Java are:
    ```
    1. Public
    2. Private
    3. Protected
    4. Default ~> Method can access only things from same package
    ```
3. Purpose of static method/keyword:
    It is shared for all the objects
4. Data encapsulation ?
    * A Class , wrapping up of data in one unit
    * Creation of objects inside class also possible

5. What is Singleton class?
    * when only one object is only possible to be made for a class
    * It is to be used to limit the resources
    * To design a singleton class:
        1. Make constructor as private.
        2. Write a static method that has return type object of this singleton class

6. Types of Loops in Java:
    1. For ~ For each is a variable concept of for loop
    2. while
    3. Do while

7. In for(;;) ~> this refers to infinte loop

8. if initialization or increment/decrement is outside loop and no condition is provided in for loop syntax then it will create error

9. Will bye be printed?
```java
for(i=0;i<=10;i++)
{
    System.out.print("Hello");
    i++;
    continue;
    system.out.print("bye"); // Not printed
}
```

10. Java has ```goto``` statement

11. Precision in float is 6 and for double is 

## Array List

```java
package exes;
import java.util.ArrayList;
import java.util.Iterator;

public class MyFirstGenerics
{
    public static void main(String args[])
    {
        ArrayList<String> names = new ArrayList<String>();
        // In order
        names.add("Piyush"); // append new element
        names.add("Rajneesh");
        names.add("Sneha");
        names.add("Piyush");
        names.set(1,"chetan"); // change element at position 1
        System.out.println(names); // print the list

        for(int i=0;i<names.size();i++)
        {
            System.out.println(names.get(i)); // print one by one
        }

        // To Copy one list into another
        ArrayList<string> copynames = new ArrayList(names);
        // Iterator Use
        Iterator itr = names.iterator();
        
        /* Iterator has 2 methods
        1. Has Next : Check whether next element is there or not (gives true or false)
        2. next: Element
        */

        while(itr.hasNext())
        {
            System.out.println(itr.next());
        }
    }
}
// javac -d . MyFirstGenerics.java this will create a exes file in current folder
```

## JDBC
* Java Database Connectivity
* standard API specification developed in order to move data from frontend to backend
* To remove platform dependency, JDBC was introduced after ODBC
* JDBC drivers are client-side
* To build JDBC application:
    1. Import Package ```import java.sql.*```
    2. Register the driver ~> initialize a driver
    3. Open a Connection ~> ```DriverManger.getConnection()```
    4. Execute a query
    5. Extract Data from result set ~> ```ResultSet.getXXX()```
    6. Clean up the environment
* Using Mysql
    1. Driver Class ```com.mysql.jdbc.Driver```
    2. Conection URL ```jdbc:mysql://localhost:3306/Database_Name```
    3. Username
    4. Password
* JDBC drivers are of 4 types:
    1. Type 1 JDBC-ODBC
    2. Type 2 
    3. Type 3 Native
    4. Type 4 

```java
import java.sql.*;

public class ConnectionDemo
{
    static final String JDBC_DRIVER = "org.mariadb.jdbc.Driver";
    static final String DB_URL = "jdbc:mariadb://localhost:3306/CRT";

    static final String USER = "user-name";
    static final String PASS = "password";

    public static void main(String[] args)
    {
        Connection conn = null;
        Statement stmt = null;
        try{
            Class.forName(JDBC_DRIVER);

            System.out.println("Connecting");
            conn = DriverManager.getConnection(DB_URL,USER,PASS);

            // Query
            stmt = conn.createStatement();
            String sql = "Select * from placed";

            ResultSet rs = stmt.executeQuery(sql);
            while(rs.next())
            {
                Variable_name = rs.getString("col name");
            }

        }
        except{

        }
    }
}
```
* Static Binding ~> The binding which can be resolved at compile time by compiler is known as static or early binding. The binding of static, private and final methods is compile-time. 
* When compiler is not able to resolve the call/binding at compile time, such binding is known as Dynamic or late Binding. Method Overriding is a perfect example of dynamic binding as in overriding both parent and child classes have same method and in this case the type of the object determines which method is to be executed. The type of object is determined at the run time so this is known as dynamic binding.