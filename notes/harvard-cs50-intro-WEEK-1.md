 # 👨‍🏫 Harvard CS50 Foundations Notes 📓

⭐ This section will be for important notes as I go through the Harvard CS50's Foundations course.
## 🧑‍💻 KEY LESSONS🚀 WEEK 1 - Variables - Operators - Functions - Loops - Problem Set 1 - C -
## LECTURE / VERBAL ** https://manual.cs50.io/  **

*📘 Visual Studio Code for CS50** Coding playground — where the magic begins✨
---
## Visual Studio Code for CS50

- 🖥️ `vscode-cs50` – The text editor that is utilized for this course is Visual Studio Code, aka VS Code, affectionately referred to as [cs50.dev](https://cs50.dev/), which can be accessed via that same URL

## 🔁 From Source Code to Machine Code  
- 🧠 Machines only speak binary  
  Deep down, computers understand just ones and zeros — it's all 1s and 0s to them.  
- 📝 Humans write source code  
  We write code in languages like C because, let’s face it — binary is hard for us. Source code is a list of instructions that we can read and write.  
- 💥 Machine code produces a desired effect  
  That binary pattern creates actions, like lighting up a pixel or printing "Hello, world!"  
- 🧑‍💻 The compiler is our translator  
  A compiler takes our human-friendly C code and turns it into fast, efficient machine code.  
- 🛠️ Meet your C compiler  
  Today, you're getting introduced to a compiler that will help you build and run C programs — welcome to the translation business!
---
## 🔧 Inside the Compiler: Tools You’ll Use  
- 🧠 **The Compiler’s Structure**: The compiler can be divided into a number of regions — all designed to help you write, manage, and run your code with ease.  
- 🖥️ **IDE (Integrated Development Environment)**: On the left side is the file explorer, where you can find your files.
-  In the middle is the **text editor** where you write and edit your programs. At the bottom is the terminal window where you can interact with the system using commands.  
- 🖱️ Finally, **Terminal Window (CLI * command line interface)**: This is where you type commands to communicate directly with the computer in the cloud. It’s powerful, fast, and essential for developers.  
- 📁 **`cd`**: Use this to move between folders — like walking through different rooms in a house.  
- 📄 **`cp`**: Copy files or folders — like duplicating a document.  
- 📋 **`\ls`**: **The most commonly used command** — lists all the files in the current directory. 
- 🆕 **`\n`**: New line of coding. (\n \n wld be 2 line etc.)
- ⬅️ **`\r`**: Moves cursor to the Beginning of the line ( not new line ).
- 🗣️ **`\"`**: Double quotaion marks
- 🗣️ **`\'`**: Single quotaion marks
- 🔣 **`\\`**: backslash marks 
- 📁 **`mkdir`**: Create a brand-new folder — your own custom storage space.  
- 🔄 **`mv`**: Move or rename files — like picking up a file and placing it somewhere else or giving it a new name.  
- 🗑️ **`rm`**: remove files — use with care, there's no undo button!  
- 🗑️📁 **`rmdir`**: remove directory - Delete entire folders — again, double-check before hitting enter!
---
### 📋 Exploring the Terminal  
- 🖥️ **Preconfigured IDE**: Because this IDE is set up with all the necessary software, you should use it to complete all assignments for this course.
---
# 👋 Hello World

### 💻 Writing, Compiling, and Running Your First Program  
- 📄 **`code hello.c`**: Creates a new file and allows us to type instructions for this program 
- ⚙️ **`make hello`**: Compiles the file from out instructions in C and creates an executable file named `hello`. 
- ▶️ **`./hello`**: Runs your compiled program called hello — watch your code come to life!  

```bash
code hello.c
make hello
./hello
```
```c
// A program that says hello to the world

#include <stdio.h>

int main(void)
{
    printf("hello, world\n");
}
```
---
⚠️ Note that every single character serves a purpose. If you type it incorrectly, the program will not run. `printf` is a function that can output a line of text — notice the quotes, semicolon, and `\n`, which adds a new line after `hello, world`. Formatting is key ⚠️
---
# ⚙️ Compiling and Running Your Program  
- 🖥️ **`make hello`**: Switch back to the terminal and run this command to compile your code.
- Notice we *omit* `.c`
- — `make` is a compiler that will automatically look for `hello.c` file and turn it into an executable program called `hello`.  
- ✅ **No errors?** Great! That means your code compiled successfully — you’re ready to run it.  
- ❌ **Errors?** No worries — double-check your code to make sure it matches exactly. Even one typo can stop the process.  
- ▶️ **`./hello`**: Run your program with this command. 
- 📁 **File Explorer (left panel)**: Open it to see both a file called `hello.c` (your readable source code) and `hello` (the compiled, executable file that the computer runs).
- ⭐`./hello` is able to be read by the compiler: It’s where your code is stored.
- 👉 hello is an executable file that you can run but cannot be read by the compiler.
#
🧩 From Scratch to C
--- 
- 🧩 In Scratch, we utilized the say block to display any text on the screen. Indeed, in C, we have a function called printf that does exactly this.  
- 🔍 `code-observation` – Notice our code already invokes this function:  
  ```c
  printf("hello, world\n");
  ```
- 📥 `function-details` – Notice that the printf function is called. The argument passed to printf is hello, world\n. The statement of code is closed with a ;
- ❌ Errors in code are common. Modify your code as follows:   
  ```c
  // \n is missing
  #include <stdio.h>

  int main(void)
  {
      printf("hello, world");
  }
  ```
- ⚠️ Notice the \n is now gone?
- In your terminal window, run make hello. Typing ./hello in the terminal window.
- This \ character is called an **escape character** that tells the compiler that \n is a special instruction to create a line break.
---
# ⚠️ There are other escape characters you can use
---

```bash
\n  create a new line
\r  return to the start of a line
\"  print a double quote
\'  print a single quote
\\  print a backslash
```
---
# Restore your program to the following:
```bash
// A program that says hello to the world

#include <stdio.h>

int main(void)
{
    printf("hello, world\n");
}
```
 👉 Notice the semicolon and \n have been restored.
---
# ⭐⭐ Header Files and CS50 Manual Pages
- The statement at the start of the code **#include <stdio.h>** is a very special command that tells the **compiler** that you want to use the capabilities of a library called stdio.h, a **header file**. This allows you, among many other things, to utilize the printf function.
- A library is a collection of code and functions created by others in the past that we can utilize in our code.
You can read about all the capabilities of this library on the Manual Pages. The Manual Pages provide a means by which to better understand what various commands do and how they function.
It turns out that CS50 has its own library called cs50.h. There are numerous functions that are included that provide training wheels while you get started in C:
```c
get_char
get_double
get_float
get_int
get_long
get_string
```
# 👋 Hello, You
---
- Recall that in Scratch we could ask the user, “What’s your name?” and say “hello” with that name appended to it.
- In C, we can do the same. Modify your code as follows:
```c
// get_string and printf with incorrect placeholder

#include <stdio.h>

int main(void)
{
    string answer = get_string("What's your name? ");
    printf("hello, answer\n");
}
```
- The get_string function is used to get a string from the user. Then, the variable answer is passed to the printf function.
- Running make hello again in the terminal window, notice that numerous errors appear.
- Looking at the errors, string and get_string are not recognized by the compiler. We have to teach the compiler these features by adding a library called cs50.h. Also, we notice that answer is not provided as we intended. Modify your code as follows:
```c
// get_string and printf with %s

#include <cs50.h>
#include <stdio.h>

int main(void)
{
    string answer = get_string("What's your name? ");
    printf("hello, %s\n", answer);
}
```
- The get_string function is used to get a string from the user. Then, the variable answer is passed to the printf function. `%s` tells the printf function to prepare itself to receive a string.
- Now, running **make hello** again in the terminal window, you can run your program by typing `./hello`. The program now asks for your name and then says hello with your name attached, as intended.
answer is a special holding place we call a variable. answer is of type string and can hold any string within it. There are many data types, such as int, bool, char, and many others.
☑️ - `%s` is a placeholder called a ***format code*** that tells the `printf` function to prepare to receive a string. `answer` is the `string` being passed to `%s`.
---
# ⭐⭐ TYPES 
- `printf` allows for many format codes. Here is a non-comprehensive list of ones you may utilize in this course:
```c
%c
%f
%i
%li
%s
```
%s is used for string variables. %i is used for int or integer variables. You can find out more about this on the Manual Pages
- These format codes correspond to the many data types that are available within C:
```c
bool
char
float
int
long
string
...
```
# 👌 Conditionals 
---
- Another building block you utilized within Scratch was **conditionals.** For example, you might want to do one thing if x is greater than y.
- Further, you might want to do something else if that condition is not met.
  
⭐ In C, you can compare two values as follows:
```c
// Conditionals that are mutually exclusive

if (x < y)
{
    printf("x is less than y\n");
}
else
{
    printf("x is not less than y\n");
}
```
👉 Notice how if x < y, one outcome occurs. If x is not less than y, then another outcome occurs.
- Similarly, we can plan for three possible outcomes:
```c
// Conditional that isn't necessary

if (x < y)
{
    printf("x is less than y\n");
}
else if (x > y)
{
    printf("x is greater than y\n");
}
else if (x == y)
{
    printf("x is equal to y\n");
}
```
👉 Notice that not all these lines of code are required. How could we eliminate the unnecessary calculation above?
---
```c
// Compare integers

if (x < y)
{
    printf("x is less than y\n");
}
else if (x > y)
{
    printf("x is greater than y\n");
}
else
{
    printf("x is equal to y\n");
}
```
👉 Notice how the final statement is replaced with else.
---
# ☎️ Operators
---
**Operators** refer to the **_mathematical operations_** that are supported by your compiler. In C, these mathematical operators include:
Operator | Function
- `+` → Addition
- `-` → Subtraction
- `*` → Multiplication
- `/` → Division
- `%` → Remainder (Modulo)
  ⭐ Modulo, often represented by the symbol %, calculates the remainder of a division operation. For example, 7 modulo 3 (written as 7 % 3) equals 1, because 7 divided by 3 is 2 with a remainder of 1.
---
# 🔣 Variables
---
- In C, you can assign a value to an `int` variable as follows:
  ```c
  int counter = 0;
  ```
- This declares an integer variable named counter and initializes it to 0.
👉 Notice how a variable called counter of type int is assigned the value 0.
---
```c
- In C, you can assign a value to an `int` variable as follows:
  ```c
  int counter = 0;
  ```
- This declares an integer variable named `counter` and initializes it to `0`.
- C can also be programmed to add one to counter as follows:
  ```c
  counter = counter + 1;
  ```
⭕ Notice how 1 is added to the value of counter.
This can be also represented as:
  ```c
  counter += 1;
  ```
  - Equivalent to `counter = counter + 1`.
- It can be further simplified using the increment operator:
  ```c
  counter++;
  ```
⭕ Notice how the ++ is used to add 1.
   - `++` automatically increments `counter` by `1`.
    
- To subtract `1` from `counter`:
  ```c
  counter--;
  ```
  - Decrements `counter` by `1` (same as `counter = counter - 1`).
⭕ You can also subtract one from counter as follows:
 ```c
counter--;
```
⭕ Notice how 1 is removed from the value of counter.

---
## 🙉 compare.c
---
```bash
// Conditional, Boolean expression, relational operator

#include <cs50.h>
#include <stdio.h>

int main(void)
{
    // Prompt user for integers
    int x = get_int("What's x? ");
    int y = get_int("What's y? ");

    // Compare integers
    if (x < y)
    {
        printf("x is less than y\n");
    }
```
👉 Notice that we create two variables, an int or integer called x and another called y. 
-   The values of these are populated using the get_int function.
-   You can run your code by executing make compare in the terminal window, followed by ./compare. If you get     any error messages, check your code for errors.
-   Flow charts are a way by which you can examine how a computer program functions. Such charts can be used      to examine the efficiency of our code
-   Looking at a flow chart of the above code, we can notice numerous shortcomings
-   We can improve your program by coding as follows:
```bash
// Conditionals

#include <cs50.h>
#include <stdio.h>

int main(void)
{
    // Prompt user for integers
    int x = get_int("What's x? ");
    int y = get_int("What's y? ");

    // Compare integers
    if (x < y)
    {
        printf("x is less than y\n");
    }
    else if (x > y)
    {
        printf("x is greater than y\n");
    }
    else
    {
        printf("x is equal to y\n");
    }
}
```
👉 Notice that all potential outcomes are now accounted for.
- You can re-make and re-run your program and test it out.
- Examining this program on a flow chart, you can see the efficiency of our code design decisions.
---
👀 agree.c
---
- Considering another data type called a char, we can start a new program by typing code agree.c into the       terminal window.
- Where a string is a series of characters, a char is a single character.
---
```bash
// Comparing against lowercase char

#include <cs50.h>
#include <stdio.h>

int main(void)
{
    // Prompt user to agree
    char c = get_char("Do you agree? ");

    // Check whether agreed
    if (c == 'y')
    {
        printf("Agreed.\n");
    }
    else if (c == 'n')
    {
        printf("Not agreed.\n");
    }
}
```
👉  Notice that additional options are offered. However, this is not efficient code.
---
```bash
// Logical operators

#include <cs50.h>
#include <stdio.h>

int main(void)
{
    // Prompt user to agree
    char c = get_char("Do you agree? ");

    // Check whether agreed
    if (c == 'Y' || c == 'y')
    {
        printf("Agreed.\n");
    }
    else if (c == 'N' || c == 'n')
    {
        printf("Not agreed.\n");
    }
}
```
👉 Notice that || effectively means or.

## ➰ Loops and meow.c
---
- We can also utilize the loop building block from Scratch in our C programs.
- In your terminal window, type code meow.c and write code as follows:
```bash
// Opportunity for better design

#include <stdio.h>

int main(void)
{
    printf("meow\n");
    printf("meow\n");
    printf("meow\n");
}
```
---
- We can improve our program by modifying your code as follows:
  ---
```bash
// Better design

#include <stdio.h>

int main(void)
{
    int i = 3;
    while (i > 0)
    {
        printf("meow\n");
        i--;
    }
}
```
---
👉 Notice that we create an int called i and assign it the value 3. Then, we create a while loop that will run as long as i > 0. Then, the loop runs. Every time 1 is subtracted to i using the i-- statement.
- Generally, in computer science, we count from zero. Best to revise your code as follows:
```bash
// Better design

#include <stdio.h>

int main(void)
{
    int i = 0;
    while (i < 3)
    {
        printf("meow\n");
        i++;
    }
}
```
- Notice we now count from zero.
- Another tool in our toolbox for looping is a for loop.
- You can further improve the design of our meow.c program using a for loop.
- Modify your code as follows:
```bash
// Better design

#include <stdio.h>

int main(void)
{
    for (int i = 0; i < 3; i++)
    {
        printf("meow\n");
    }
}
```
- Notice that the for loop includes three arguments. The first argument int i = 0 starts our counter at zero. The second argument i < 3 is the condition that is being checked. Finally, the argument i++ tells the loop to increment by one each time the loop runs.
- We can even loop forever using the following code:
```bash
// Infinite loop

#include <cs50.h>
#include <stdio.h>

int main(void)
{
    while (true)
    {
        printf("meow\n");
    }
}
```
- Notice that true will always be the case. Therefore, the code will always run. You will lose control of your terminal window by running this code. You can break from an infinite loop by hitting control-C on your keyboard.
  ## Functions
---
- While we will provide much more guidance later, you can create your own function within C as follows:
```bash
void meow(void)
{
    printf("meow\n");
}
```
- The initial void means that the function does not return any values. The (void) means that no values are     being provided to the function.
- This function can be used in the main function as follows:
```bash
// Abstraction

#include <stdio.h>

void meow(void);

int main(void)
{
    for (int i = 0; i < 3; i++)
    {
        meow();
    }
}

// Meow once
void meow(void)
{
    printf("meow\n");
}
```
- Notice how the meow function is called with the meow() instruction.
- This is possible because the meow function is defined at the bottom of the code, and the prototype of the function is provided at the top of the code as void meow(void).
- Your meow function can be further modified to accept input:
```bash
// Abstraction with parameterization

#include <stdio.h>

void meow(int n);

int main(void)
{
    meow(3);
}

// Meow some number of times
void meow(int n)
{
    for (int i = 0; i < n; i++)
    {
        printf("meow\n");
    }
}
```
- Notice that the prototype has changed to void meow(int n) to show that meow accepts an int as its input.
- Additionally, we can get user input:
```bash
// User input

#include <cs50.h>
#include <stdio.h>

void meow(int n);

int main(void)
{
    int n;
    do
    {
        n = get_int("Number: ");
    }
    while (n < 1);
    meow(n);
}

// Meow some number of times
void meow(int n)
{
    for (int i = 0; i < n; i++)
    {
        printf("meow\n");
    }
}
```
- Notice that get_int is used to obtain a number from the user. n is passed to meow.
- We can even test to ensure that the input we get provided by the user is correct:
```bash
// Return value

#include <cs50.h>
#include <stdio.h>

int get_positive_int(void);
void meow(int n);

int main(void)
{
    int n = get_positive_int();
    meow(n);
}

// Get number of meows
int get_positive_int(void)
{
    int n;
    do
    {
        n = get_int("Number: ");
    }
    while (n < 1);
    return n;
}

// Meow some number of times
void meow(int n)
{
    for (int i = 0; i < n; i++)
    {
        printf("meow\n");
    }
}
```
- Notice that a new function called get_positive_int asks the user for an integer while n < 1.
- After obtaining a positive integer, this function will return n back to the main function.
---
# ⭐ Correctness, Design, Style
---
 - Code can be evaluated upon three axes
 - First, correctness refers to “Does the code run as intended?”
 - You can check the correctness of your code with check50.
 - Second, design refers to “How well is the code designed?”
 - You can evaluate the design of your code using design50.
 - Finally, style refers to “How aesthetically pleasing and consistent is the code?”
 - You can evaluate the style of your code with style50.
 # Mario
 ---
 - Everything we’ve discussed today has focused on various building blocks of your work as an emerging computer scientist.
 - The following will help you orient toward working on a problem set for this class in general: How does one approach a computer science-related problem?
 - Imagine we wanted to emulate the visual of the game Super Mario Bros. Considering the four question blocks pictured, how could we create code that roughly represents these four horizontal blocks?

<img width="960" height="540" alt="cs50Week1Mario1" src="https://github.com/user-attachments/assets/950dc12b-4483-4056-8eb5-496586e39401" />

In the terminal window, `type code mario.c` and code as follows:
```bash
// Prints a row of 4 question marks with a loop

#include <stdio.h>

int main(void)
{
    for (int i = 0; i < 4; i++)
    {
        printf("?");
    }
    printf("\n");
}
```
 - 🔁 Notice how four question marks are printed using a `for` loop
##
 - Just like printing horizontal question marks, we can apply the same logic to create **three vertical blocks**  
- Instead of printing all `?` on the same line, we'll print one per line

<img width="960" height="540" alt="cs50Week1three vertical blocks" src="https://github.com/user-attachments/assets/9fbd6450-6eec-49b6-86b2-fc426f04dd90" />
### Example Code
``` bash
// Prints a column of 3 bricks with a loop

#include <stdio.h>

int main(void)
{
    for (int i = 0; i < 3; i++)
    {
        printf("#\n");
    }
}
```
---
- 🔁 The `for` loop runs **3 times**, printing a single `?` followed by a new line (`\n`) each time  
- ⬆️ This gives the appearance of **vertical blocks**, like a column in a Mario level
- 
- What if we wanted to combine these ideas to create a three-by-three group of blocks?
-  We can use a loop that prints a single `#` followed by a newline each time  
- Below is the modified code:
---

<img width="960" height="540" alt="cs50Week1three-by-three group of blocks7" src="https://github.com/user-attachments/assets/8c4b2a15-e6eb-446f-b963-511cd216b627" />

We can follow the logic above, combining the same ideas. Modify your code as follows:
```bash
// Prints a 3-by-3 grid of bricks with nested loops

#include <stdio.h>

int main(void)
{
    for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 3; j++)
        {
            printf("#");
        }
        printf("\n");
    }
}
```
- Notice that one loop is inside another.
- The first loop defines what vertical row is being printed. For each row, three columns are printed.
- After each row, a new line is printed.

- What if we wanted to ensure that the number of blocks is constant, that is, unchangeable? Modify your code as follows:
```bash
// Prints a 3-by-3 grid of bricks with nested loops using a constant

#include <stdio.h>

int main(void)
{
    const int n = 3;
    for (int i = 0; i < n; i++)
    {
        for (int j = 0; j < n; j++)
        {
            printf("#");
        }
        printf("\n");
    }
}
```
- Notice how n is now a constant. It can never be changed.
---
# ✍️ Comments 
---
- All code you create for this course must include robust comments.  
- Typically, each comment is a few words or more, providing the reader an opportunity to understand what is happening in a specific block of code. Further, such comments serve as a reminder for you later when you need to revise your code.  
- Each comment begins with `//`
- Comments involve placing // into your code, followed by a comment.
- 🧠 This tells the compiler to **ignore the line** while making the code more understandable for humans  
- 🛠️ Good commenting improves **readability**, **maintainability**, and **collaboration** in programming
- As illustrated earlier in this lecture, we can abstract away functionality into functions. Consider the following code:
-  Modify your code as follows to integrate comments:
```bash
// Helper function

#include <stdio.h>

void print_row(int width);
  
int main(void)
{
    const int n = 3;

    // Print n rows
    for (int i = 0; i < n; i++)
    {
        print_row(n);
    }
}

void print_row(int width)
{
    for (int i = 0; i < width; i++)
    {
        printf("#");
    }
    printf("\n");
}
```
- 🔍 Notice how printing a row is now accomplished through a new function called `print_row`  
- 🧩 `print_row(int width)` handles printing a single row of `#` characters  
- 📦 This makes the `main` function cleaner and more focused on logic, not implementation  
- 🔑 This is a key step toward writing **modular, maintainable, and scalable** code
## 🧮 More About Operators – Building a Simple Calculator in C  
- 
You can implement a calculator in C. In your terminal, type code calculator.c and write code as follows:
```bash
// Addition with int

#include <cs50.h>
#include <stdio.h>

int main(void)
{
    // Prompt user for x
    int x = get_int("x: ");

    // Prompt user for y
    int y = get_int("y: ");

    // Add numbers
    int z = x + y;

    // Perform addition
    printf("%i\n", z);
}
```
- Notice how the `get_int` function is utilized to obtain an integer from the user twice.
- One integer is stored in the `int` variable called `x`
- Another is stored in the int variable called `y`
- The sum is stored in `z`
- Then, the `printf` function prints the value of `z`, designated by the `%i` symbol.
---
- # 🔣🔣 We can also double a number
```bash
// int

#include <cs50.h>
#include <stdio.h>

int main(void)
{
    int dollars = 1;
    while (true)
    {
        char c = get_char("Here's $%i. Double it and give to next person? ", dollars);
        if (c == 'y')
        {
            dollars *= 2;
        }
        else
        {
            break;
        }
    }
    printf("Here's $%i.\n", dollars);
}
```
- 👉 Running this program, some seeming errors appear in dollars. - Why is this?
🔁 This program starts with `$1` and keeps doubling it as long as the user types `y`  
- 💥 However, after a certain number of doublings, the value of `dollars` may appear to **behave incorrectly** or **reset unexpectedly**
- One of C’s shortcomings is the ease by which it manages memory. While C provides you immense control over how memory is utilized, programmers have to be very aware of the potential pitfalls of memory management. Can you add this inside a bullet, for this one we do not need a heading  
- Types refer to the possible data that can be stored within a variable. For example, a char is designed to accommodate a single character like a or 2.  
- Types are very important because each type has specific limits. For example, because of the limits in memory, _the highest value of an `int` can_ be **4294967295**.
- If you attempt to count an int higher, an _integer overflow_**** will result where an incorrect value will be stored in this variable.
  
- The number of bits limits how high and low we can count.  
- This can have catastrophic, real-world impacts.  
- We can correct this by using a data type called `long`.
```bash
// long

#include <cs50.h>
#include <stdio.h>

int main(void)
{
    long dollars = 1;
    while (true)
    {
        char c = get_char("Here's $%li. Double it and give to next person? ", dollars);
        if (c == 'y')
        {
            dollars *= 2;
        }
        else
        {
            break;
        }
    }
    printf("Here's $%li.\n", dollars);
}
```
---
👉 Notice how running this code will allow for very high dollar amounts.
---
## ➡️ Types with which you might interact during this course include:
- `` `bool` ``, a Boolean expression of either true or false  
- `` `char` ``, a single character like a or 2  
- `` `double` ``, a floating-point value with more digits than a float  
- `` `float` ``, a floating-point value, or a real number with a decimal value  
- `` `int` ``, integers up to a certain size, or number of bits  
- `` `long` ``, integers with more bits, so they can count higher than an int  
- `` `string` ``, a string of characters
---
# ✂️ Truncation 
---
## (cutting off part of a value, typically without rounding, resulting in a shortened or simplified version.)
- Removing decimal places from a floating-point number without rounding.
## For example:
- Truncating 3.789 results in 3 (all digits after the decimal are simply dropped).
- Shortening data, such as strings or files, by cutting off content beyond a certain point.
## For example:
- Truncating the string "HelloWorld" to 5 characters gives "Hello".
- Memory or variable overflow, where a value is too large to fit in a data type and gets cut off,              potentially leading to data loss or errors.
---
## Another issue that can arise when using data types includes truncation
### 🔍 Example: Integer Division with Truncation

```bash
// Division with ints, demonstrating truncation

#include <cs50.h>
#include <stdio.h>

int main(void)
{
    // Prompt user for x
    int x = get_int("x: ");

    // Prompt user for y
    int y = get_int("y: ");

    // Divide x by y
    printf("%i\n", x / y);
}
```
⭐ An integer divided by an integer will always result in an integer in C. Accordingly, the above code will often result in any digits after the decimal being thrown away.
- ➗ In C, dividing two `int` values results in an `int`  
- 📉 This means that any **decimal portion is truncated**, not rounded  
  - Example: `5 / 2` results in `2`, not `2.5`  
  - Example: `9 / 4` results in `2`, not `2.25`

### 🧠 Why This Matters

- Truncation can lead to **unexpected results** in calculations  
- It's especially important in applications where **precision is critical**, like finance, science, or engineering.
---
👌 This can be solved by using `float` or `double` for Division with Decimals.
To preserve decimal precision, cast one of the operands to a floating-point type:

```c
printf("%f\n", (float) x / y);
```

- 📌 This avoids truncation and gives you the full floating-point result  
- `%f` is the format specifier for `float` or `double` in `printf`

🚫 **Floating Point Imprecision – A New Kind of Problem**

- Using `float` can help avoid **truncation** from integer division  
- However, it introduces a new issue: **floating point imprecision**

### 🔍 Example: Division with `float`
```bash
// Floats

#include <cs50.h>
#include <stdio.h>

int main(void)
{
    // Prompt user for x
    float x = get_float("x: ");

    // Prompt user for y
    float y = get_float("y: ");

    // Divide x by y
    printf("%.50f\n", x / y);
}
```
- 🔎 Notice that using `%.50f` prints up to **50 decimal places**
- 💥 But the result may show **unexpected decimal values**, like:
  - `1.0 / 10.0` might print as `0.1000000014901161193677...` instead of `0.1`
### 📉 Why Floating Point Imprecision Happens
---
- Floating point imprecision illustrates that there are limits to how precise computers can calculate numbers.
- Computers store floating-point numbers using **binary fractions**  
- Some decimal numbers (like `0.1`) can't be represented exactly in binary  
- This leads to **tiny rounding errors** that accumulate over time
  **Patriot Missile Failure (1991)** – A rounding error caused a missile to fail, resulting in 28 deaths  
  - **Ariane 5 Rocket Explosion (1996)** – A floating point conversion error caused a $370 million loss
---
### ✅ Best Practices
---
As you are coding, pay special attention to the types of variables you are using to avoid problems within your code.
- Be cautious when choosing **data types** in C  
- Use `float` or `double` when you need decimal precision  
- Use `int` or `long` when fractional values aren’t needed  
- Always **think about the limits** of each type and how they affect your program
  
## 🎓 **Summing Up – Key Takeaways from This Lesson**
---
In this lesson, you learned how to apply the building blocks you learned in Scratch to the C programming language. You learned…
- how to apply programming concepts from **Scratch** to the **C programming language**  
- 💻 Created your **first program in C** and became familiar with the **command line**  
- 📦 Explored **predefined functions** that come natively with C  
- 🛠️ Used **variables**, **conditionals**, and **loops** to build logic into your programs  
- 🧩 Created your own **functions** to make code **cleaner**, **modular**, and **reusable**  
- 📊 Evaluated your code using three key criteria:
  - ✅ **Correctness** – Does it work as intended?
  - 🎨 **Design** – Is the code well-structured and efficient?
  - 🧼 **Style** – Is it readable and consistent?
- 📝 Integrated **comments** to document your code and improve clarity  
- 🔢 Worked with **data types** and **operators**, and explored the real-world consequences of type-related decisions like:
  - 🧨 **Integer overflow**
  - 🔍 **Floating point imprecision**
  - 🧱 **Memory management pitfalls**
