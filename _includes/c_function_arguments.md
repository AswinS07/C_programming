# calling functions in C


| Type | Description |
|------|-------------|
| Call by Value | The actual parameter is passed to a function |
|               | New memory area created for the passed parameters, can be used only within the function. |
|               | The actual parameters cannot be modified here. |
| Call by Reference | Instead of copying variable; an address is passed to function as parameters. |
|                   | Address operator(&) is used in the parameter of the called function. |
|                   | Changes in function reflect the change of the original variables. |

## Call by Value

### Example:

```c
  #include<stdio.h>         /* function declaration */
  int addition(int num1, int num2);
  int main() {
    int answer;         /* local variable definition */    
    int num1 = 10;
    int num2 = 5;

    answer = addition(num1,num2);         /* calling a function to get addition value */  

    printf("The addition of two numbers is: %d\n",answer);
    return 0;
  }

  int addition(int a,int b)             /* function returning the addition of two numbers */
  {
      return a + b;
  }
```

Program output:
```text
The addition of two numbers is: 15
```

## Call by Reference

### Example:

```c
  #include<stdio.h>

  /* function declaration */int addition(int *num1, int *num2);

  int main() {
      int answer;
      int num1 = 10;
      int num2 = 5;

      answer = addition(&num1,&num2);       /* calling a function to get addition value */    

      printf("The addition of two numbers is: %d\n",answer);
      return 0;
  }

  int addition(int *a,int *b)             /* function returning the addition of two numbers */
  {
      return *a + *b;
  }
```

Program output:
```text
The addition of two numbers is: 15
```

