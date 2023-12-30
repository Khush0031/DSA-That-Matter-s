**`Lesson-02 :`**

**`Variables, Data Types and the first C++ program`**

**`List of Concepts Involved :`**

- C++ Variables. 
- C++ Identifiers.  
- C++ Data Types.
- C++ Output.
- How does the C++ program work.
- C++ user input.

A computer program/code consists of various components i.e -> `variables`,`data types`,`identifiers`,`keywords`, etc which helps us to build a successful program. 

Let us learn each one of them in detail and then move to our first program.

**`Topic 1: C++ Variables`**

- A variable is the title of a reserved region allocated in memory. In other words, it may be referred to as the    name of a memory location.
- Each variable should be given a unique name to indicate the storage area.
- A variable is a container that holds the value while the C++ program is executed. 
- A variable is assigned with a data type(we will learn about it after this).

**`Syntax for Declaring a Variable :`**

`DataType variableName = value;`

The variable\_name is the name of a variable. We can initialize the variable by specifying an equal sign and a value  (Initialization i.e. assigning an initial value, is optional).

**`Creating Variables Example:`**
```c++
DataType variableName = value; 
int age = 20;
```
**`Reserved Memory for Variable :`**  

**RAM**

In the example above, the variable can only hold integer values, as indicated by the int data type.
Here, we assigned a value to the variable during the declaration process. 
However, as stated before, it is optional. 
Variables can be declared and assigned separately.  
 **`Example :`**
```c++
int rate; 
rate = 40;
```

**`Change Values of Variables`**

Interestingly, a variable's value can also be changed in the programme. 
`As an example, int rate = 50;`
```c++
cout<<rate; // 50

rate = 60;

cout<<rate; // 60
```
Initially, the value of rate was 50 but it has changed to 60 after the last updation, rate=60.

**`Naming Conventions for variables in C++`**

Like us, all C++ components are identified with their names.  
There are a few points to remember while naming the variable. 
They are as follows -

- Variable names should not begin with a **Number**.  
`For Example :`  
```c++
 int 2var;   // 2var is an invalid variable.
 ```  

- Whitespaces are not permitted in variable names. 
`For example :`     
```c++
int cricket score;  // invalid variables.
```
There is a gap/whitespace between cricket and score.

- A C++ keyword (reserved word) cannot be used as a variable name. 
`For example`
```c++
 int float; /*is an invalid expression as float is  
 pre-defined as a keyword(we will learn about them) in C++.
 */
 ```
- As per the latest coding practices, for variable names with more than one word the first word has all lowercase letters and first letter of subsequent words capitalised. 
`For example`, *`cricketScore`*, *`codePracticeProgram`* etc. This type of format is called camel case
- While creating variables, it's preferable to give them `meaningful names like`- *`‘age’`*, *`‘earning’`*, *`‘value’`* etc. for instance, makes much more sense than variable names like *`a`*, *`e`*, and *`v`*.
- We use all lowercase letters when creating one-word variable name. It's preferable(and in practice) to use physics rather than PHYSICS or pHYSICS.

**`Topic 2: C++ Identifiers :`**

C++ identifier is a name given to a *`package`*, *`class`*, *`interface`*, *`method`*, or *`variable`*. All identifiers must have different names.

In C++, there are a few points to remember while dealing with identifiers :

- **`Rule 1 −`** All identifiers should begin with a letter (A to Z or a to z), $ and and must be unique.
- **`Rule 2 −`** After the first character/letter, identifiers can have any combination of characters.
- **`Rule 3 −`** A keyword cannot be used as an identifier.
- **`Rule 4 −`** The identifiers are case sensitive.
- **`Rule 5 –`** Whitespaces  are not permitted.

`Examples of legal identifiers : ` *`rank`*, *`$name`*, *`\_rate`*, *`\_\_2\_mark`*.

`Examples of illegal identifiers :` *`102pqr`*, *`-name`*.

These variables, identifiers etc. consume memory units. Before proceeding ahead, let us have a look at the memory unit concept too. Here, we will only focus on the relevant concept of memory.

**`Basic Memory units :`**

It refers to the amount of memory or storage used to measure data. Basic memory units are:

 **`1.Bit`**

A bit (`binary digit 0 or 1`) is the smallest unit of data that a computer can process and store.

Symbols `0` and `1` are known as bits. Here, `0` indicates the `passive state `of signal and `1` indicates the `active state `of signal.

At a time, a bit can store only one value i.e 0 or 1. To have a greater range of value, we combine multiple bits.

 **`2.Byte`**

A byte is a unit of memory/data that is equal to `8 bits`.

You may think of a byte as one letter. 
`For example`, the letter `'f'` is `one byte` or `eight bits`.

The bigger units are :

 **`3.Kilobyte`**

A Kilobyte is a unit of memory data equal to `1024 bytes`.

 **`4.Megabyte`**

A Megabyte is a unit of memory data equal to `1024 kilobytes`.

 **`5.Gigabyte`**

A Gigabyte is a unit of memory data equal to `1024 Megabytes`. 

**`Topic 3: C++ Data Types`**

Data types specify the different sizes and values that can be stored in the variable. 
Based on the data type of a variable, the operating system allocates memory and decides what can be stored in the reserved memory. 
Therefore, by assigning different data types to variables, we can store integers, decimals, or characters in these variables.

**`Data types in C++ are categorized in three groups :`**
 **`1.Built-in (Primary)`**.
 **`2.User-defined`**.
 **`3.Derived`**.

**`Data Types in C / C++ : `**

| Primary            | Derived        | User Defined  |
|---------------------|----------------|---------------|
| Integer             | Function       | Class         |
| Character           | Array          | Structure     |
| Boolean             | Pointer        | Union         |
| Floating Point      | Reference      | Enum          |
| Double Floating Point| Typedef        |               |
| Void                |                |               |
| Wide Character      |                |               |


`Here we will discuss primary data types only`.

 **`1.C++ int : `**
- The `int` keyword is used to indicate `integers`. 
- Its size is usually `4 bytes`. 
Meaning,  values can be stored from `-2147483648` to `2147483647`.
```c++
For example: 
int rate=40;
```
 **`2.C++ char : `**
- This data type is used to store a `single character`.
- Size of char  is `1 byte`.
- Characters in C++ are enclosed inside single quotes `' '`.
```c++
For example: 
char symbol='a'
```
**`3.C++ bool : `**     
- A boolean data type is declared with the `bool`keyword.
- The bool data type has one of two possible values: `true` or `false`.
```c++
- For example : 
 bool flag=false; //or
 bool flag=true;
 ```
 **`4.C++ float`** 
- Float is used to store `floating point numbers` (`decimals and exponentials`).
- The size of the float is `4 bytes`.
- In general, `7 decimal digits precision`.
```c++
- For example: 
 float rate=40.50;
 ```
 **`5.C++ double`**
- Double is used to store `floating-point numbers` (`decimals and exponentials`).
- The size of the double is `8 bytes`. 
Hence, double has two times the precision of float. 
- In general, `15 decimal digits precision`.
```c++
- For example: 
double rate=40.6543444;
```
 **`6.C++ void`**
- The void keyword means    `"nothing"` or `"no value"`.
- Void will be used in functions and pointers.
- Variables of the void type can’t be declared.

 **`7.C++ wchar\_t`**
- Wide character wchar\_t is similar to the char data type, except its size is 2 bytes instead of 1.

**`Note: C++ "String" Data Types : `**

- This data type is used to store a `sequence of characters` (`text`).
- This is `not a built-in data type`.
- String values must be surrounded by `double quotes`.
```c++
- For example
 string name= "Ramesh";
 ```

**`Topic 4: C++ Output/Display Program : `**

Now that we have learnt all the relevant concepts, let us go ahead and write our very first program!
```c++

// C++ program to display “Hello World in C++”: 
#include <iostream>
using namespace std;
int main()
{
    // prints hello world in C++
    cout << "Hello World in C++";

}

**Output: Hello World in C++**

**How Does this Programme Work?**
```
**`Understanding Every Line Of Program/Code.`**

- **`// C++ program to display “Hello World in C++” : `** This is a comment line. 
A comment is used for displaying additional information about the program. 
It does not contain any programming logic. 
When a comment is encountered by the compiler, that line or part of code is skipped by the compiler. 
Any line beginning with ‘//’ without quotes OR in between /\*…\*/ in C++ is a comment.

- In C++,  all lines that start with a `pound` or `hashtag(#)` sign are called `directives` and are processed by a `preprocessor` which is a program invoked by the compiler. 
The **`#include`** directive tells the C++ preprocessor to include contents of the file specified in input stream to the compiler and then continue with the rest of the original file. 
**`#include<iostream>`** tells the preprocessor to include the `iostream header file`(file that has some already pre-written code which we are importing to avoid reinventing the wheel) in the program and iostream is the header file which contains all the basic functions of the program like input/output etc.
- **`Using namespace std`** is used to define which input/output form is going to be used.
- **`int main()`**:This line is used to declare a function having the name `“main”` whose return type is integer. `Every C++ program’s execution begins with the main() function`, no matter where the function is located in the program. So,it’s necessary for every C++ program to have a main() function.
- **`cout<<“Hello World in C++”;`**:  This line instructs the compiler to `display the message “Hello World in C++” on the screen`.

**`Note 1 :`** In C++ every statement should be terminated with semicolon `(;)` for execution. 
**`Note 2 :`** In C++, we can use `endl` or `\n` to insert new lines in the output data stream.

**`Additional information :`**

Like `cout` we also use `printf()`function that comes from the `C language`. 
`C++ printf prototype` defined under `<cstdio> header file`

**`Example :`** 
```c++
#include <iostream>
using namespace std;
int main()
{
    // prints hello world in C++     
    printf("Hello World in C++");  
}
"Output: Hello World in C++" 
```
**`Example :`** 
```c++
cout<<"Physics"<<"Wallah";
"Output: PhysicsWallah"
cout<<"Physics"<<endl<<"Wallah";

"Output: Physics                     
          Wallah
"          
```
**`Topic 5: Taking input from the user : `**

We have already learnt that cout is used to output (print) values. Now let us explore the abilities of C++ which will allow us to get input from users. This can be done using `cin`.

`cin is a predefined object` that reads data from the user with the extraction operator `(>>)` (`like scanf is used in case of C language`).

`In the following example, the user can input a number, which is stored in the variable x. Then we will print the value of x :`

**`Example :`** 
```c++
int num; 
cout << "Enter any number "; // Type a number and press enter
cin >> num; // Get user input from the keyboard 
cout << "Entered number is: " << num; // Display the input value
```
**`Example :`**
```c++
 //The user is asked to enter two integers and their sum is displayed
#include <iostream>
using namespace std;
int main() {
int n1, n2, sum;
cout << "Enter two numbers: ";
cin >> n1 >> n2;
// sum of two numbers is stored in variable sum   
sum = n1 + n2;
// prints sum 
cout << sum <<endl;    
return 0;
}
```


