# datatypes\_keywords

## **Variables and Keywords in C**

A variable in simple terms is a storage place which has some memory allocated to it. Basically, a variable used to store some form of data. Different types of variables require different amounts of memory, and have some specific set of operations which can be applied on them.

### Variable Declaration:

A typical variable declaration is of the form:

```text
  type variable\_name;

  or for multiple variables:

  type variable1\_name, variable2\_name, variable3\_name;
```

A variable name can consist of alphabets \(both upper and lower case\), numbers and the underscore '\_' character. However, the name must not start with a number.

### Difference b/w variable declaration and definition

Variable declaration refers to the part where a variable is first declared or introduced before its first use. Variable definition is the part where the variable is assigned a memory location and a value. Most of the times, variable declaration and definition are done together.

See the following C program for better clarification:

```text
        #include <stdio.h>
        int main()
        {
            // declaration and definition of variable 'a123'
            char a123 = 'a';

      // This is also both declaration and definition as 'b' is allocated
      // memory and assigned some garbage value.  
      float b; 

      // multiple declarations and definitions
      int _c, _d45, e;

      // Let us print a variable
      printf("%c \n", a123);

            return 0;
        }
```

**Output:**

```text
    a
```

#### Rules for defining variables

A variable can have alphabets, digits, and underscore.

A variable name can start with the alphabet, and underscore only. It can't start with a digit.

No whitespace is allowed within the variable name.

A variable name must not be any reserved word or keyword, e.g. int, goto , etc.

#### Types of Variables in C

**1. Local Variable**

A variable that is declared and used inside the function or block is called local variable.

It's scope is limited to function or block. It cannot be used outside the block.Local variables need

to be initialized before use.

Example –

```text
        #include <stdio.h>
        void function() {
          int x = 10; // local variable
        }

        int main()
        {
          function();
        }
```

In the above code x can be used only in the scope of function\(\) . Using it in main function will give error.

**2. Global Variable**

A variable that is declared outside the function or block is called a global variable.

It is declared at the starting of program. It is available to all the functions.

Example –

```text
         #include <stdio.h>

        int x = 20;//global variable
        void function1()
        {
          printf("%d\n" , x);
        }
        void function2()
        {
          printf("%d\n" , x);
        }
        int main() {

          function1();
          function2();
            return 0;
        }
```

**Output**

```text
    20

    20
```

In the above code both the functions can use global variable x as we already global variables are accessible by all the functions.

**3.Static Variable**

A variable that retains its value between multiple function calls is known as static variable.

It is declared with the static keyword.

Example-

```text
        #include <stdio.h>
        void function(){ 
        int x = 20;//local variable 
        static int y = 30;//static variable 
        x = x + 10; 
        y = y + 10; 
        printf("\n%d,%d",x,y); 
        } 
        int main() {

          function();
          function();
          function();
          return 0;
        }
```

**Output**

```text
        30,40

        30,50

        30,60
```

In the above example , local variable will always print same value whenever function will be called whereas static variable will print the incremented value in each function call.

## keywords in C

Keywords are specific reserved words in C each of which has a specific feature associated with it. Almost all of the words which help us use the functionality of the C language are included in the list of keywords.

There are a total of 44 keywords in C \(C89 – 32, C99 – 5, C11 – 7\):

![](../.gitbook/assets/keywords.png)

Most of these keywords have already been discussed in the various sub-sections of the C language, like Data Types, Storage Classes, Control Statements, Functions etc.

