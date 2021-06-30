C function is a self-contained block of statements that can be executed repeatedly whenever we need it.

Benefits of using the function in C

The function provides modularity.
The function provides reusable code.
In large programs, debugging and editing tasks is easy with the use of functions.
The program can be modularized into smaller parts.
Separate function independently can be developed according to the needs.

There are two types of functions in C

Built-in(Library) Functions
The system provided these functions and stored in the library. Therefore it is also called Library Functions.
e.g. scanf(), printf(), strcpy, strlwr, strcmp, strlen, strcat etc.
To use these functions, you just need to include the appropriate C header files.

User Defined Functions These functions are defined by the user at the time of writing the program.

Parts of Function

Function Prototype (function declaration)
Function Definition
Function Call

1. Function Prototype

#### Syntax:
dataType functionName (Parameter List)

#### Example:
int addition();

2. Function Definition

#### Syntax:
returnType functionName(Function arguments){
  //body of the function 
}

#### Example:
int addition()
{

}

Calling a function in C

Program to illustrate the Addition of Two Numbers using User Defined Function

#include<stdio.h>

/* function declaration */int addition();

int main()
{   
    /* local variable definition */    int answer;
    
    /* calling a function to get addition value */    answer = addition();

    printf("The addition of the two numbers is: %d\n",answer);
    return 0;
}

/* function returning the addition of two numbers */int addition()
{
    /* local variable definition */    int num1 = 10, num2 = 5;
    return num1+num2;
}

Program output

The addition of the two numbers is: 15

