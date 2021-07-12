# C PREPROCESSORS
The preprocessor is a program invoked by the compiler that modifies the source code before the actual composition takes place.

> To use any preprocessor directives, first we have to prefix them with pound symbol #

The following section lists all preprocessor directives:

| CATEGORY | DIRECTIVE | DESCRIPTION |
|----------|-----------|-------------|
| Marco substitution division | #include | File include |
| | #define | Marco define |
| | #undif | Marco undefine |
| | #ifdef | If marco defined |
| | #ifndef | If marco not defined |
| File inclusion division | #if, #elif, #else, #endif | if, Else, ifElse, Endif |
| Compiler control division | #line, #error, #pragma | Set line number, Abort compilation, Set compiler option |

## Examples

```c
#include <stdio.h>

/* #define macro_name character_sequence */
#define LIMIT 10

int main()
{
    int counter;
    for(counter =1; counter <=LIMIT; counter++)
    {
        printf("%d\n",counter);
    }
return 0;
}
```
In the above example for loop will run ten times.

```c
#include <stdio.h>
#include "header.h"
```
```c #include <stdio.h> ``` tell the compiler to add stdio.h file from System Libraries to the current source file, and ```c #include "header.h"``` tells the compiler to get header.h from the local directory.

```c
#undef  LIMIT
#define  LIMIT 20
```
