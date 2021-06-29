# goto statement in C/C++

The goto statement is a jump statement which is sometimes also referred to as unconditional jump statement. The goto statement can be used to jump from anywhere to anywhere within a function.

**Syntax** :

syntax of goto statement.png

In the above syntax, the first line tells the compiler to go to or jump to the statement marked as a label. Here label is a user-defined identifier which indicates the target statement. The statement immediately followed after &#39;label:&#39; is the destination statement. The &#39;label:&#39; can also appear before the &#39;goto label;&#39; statement in the above syntax.

Flowchart\_goto\_statement.png

Below are some examples on how to use goto statement:

**Examples:**

- **Type 1** : In this case, we will see a situation similar to as shown in Syntax1 above. Suppose we need to write a program where we need to check if a number is even or not and print accordingly using the goto statement. Below program explains how to do this:

example\_1\_goto.png

**Output:**
output\_ex1\_goto.png

  - **Type 2:** : In this case, we will see a situation similar to as shown in Syntax1 above. Suppose we need to write a program which prints numbers from 1 to 10 using the goto statement. Below program explains how to do this.

example\_2\_goto.png

**Output:**
output\_ex2\_goto.png

**Disadvantages of using goto statement:**

- The use of goto statement is highly discouraged as it makes the program logic very complex.
- use of goto makes the task of analyzing and verifying the correctness of programs (particularly those involving loops) very difficult.
- Use of goto can be simply avoided using break and continue statements.