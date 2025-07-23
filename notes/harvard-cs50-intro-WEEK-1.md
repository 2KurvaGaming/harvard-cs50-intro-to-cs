 # 👨‍🏫 Harvard CS50 Foundations Notes 📓

⭐ This section will be for important notes as I go through the Harvard CS50's Foundations course.
## 🧑‍💻 KEY LESSONS🚀 WEEK 1 - Variables - Operators - Functions - Loops - Problem Set 1 - C -
## LECTURE / VERBAL ** https://manual.cs50.io/  **

**📘 Visual Studio Code for CS50** Coding playground — where the magic begins✨
---
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
- 🖥️ **IDE (Integrated Development Environment)**: On the left side is the file explorer, where you can find your files. In the middle is the text editor where you write and edit your programs. At the bottom is the terminal window where you can interact with the system using commands.  
- 🖱️ **Terminal Window (CLI)**: This is where you type commands to communicate directly with the computer in the cloud. It’s powerful, fast, and essential for developers.  
- 📁 **`cd`**: Use this to move between folders — like walking through different rooms in a house.  
- 📄 **`cp`**: Copy files or folders — like duplicating a document.  
- 📋 **`ls`**: **The most commonly used command** — lists all the files in the current directory. 
- 🆕 **`\n`**: New line of coding. (\n \n wld be 2 line etc.)
- ⬅️ **`\r`**: Moves cursor to the Beginning of the line ( not new line )
- 🗣️ **`\"`**: Double quotaion marks
- 🗣️ **`\'`**: Single quotaion marks
- 🔣 **`\\`**: backslash marks 
- 🗣️ **`\"`**: Double quotaion marks
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
- 📄 **`code hello.c`**: Creates a new file and opens the text editor — this is where you'll write your first program. 
- ⚙️ **`make hello`**: Compiles your code into machine-readable format — an executable file named `hello`. 
- ▶️ **`./hello`**: Runs your compiled program — watch your code come to life!  

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
⚠️ Note that every single character matters. If even one is off, the program will not run. `printf` is a function that outputs text — notice the quotes, semicolon, and `\n`, which adds a new line after `hello, world`. Formatting is key ⚠️

---

# ⚙️ Compiling and Running Your Program  
- 🖥️ **`make hello`**: Switch back to the terminal and run this command to compile your code.
- Notice we *omit* `.c`
- — `make` automatically looks for `hello.c` and turns it into an executable program called `hello`.  
- ✅ **No errors?** Great! That means your code compiled successfully — you’re ready to run it.  
- ❌ **Errors?** No worries — double-check your code to make sure it matches exactly. Even one typo can stop the process.  
- ▶️ **`./hello`**: Run your program with this command. 
- 📁 **File Explorer (left panel)**: Open it to see both `hello.c` (your readable source code) and `hello` (the compiled, executable file that the computer runs).
--- 
# 🐱‍💻 **Functions in C**  
- While we will provide much more guidance later, you can create your own function within C as follows:  
  ```c  
  void meow(void)  
  {  
      printf("meow\n");  
  }  
  ```  
- 🧱 This function can be used in the main function as follows:
  ```c  
  // Meow once
  #include <stdio.h>  
  
  int main(void)  
  {  
      printf("meow\n");  
  }
  
        // OR //
  
  // Meow 3x's
  #include <stdio.h>
  
  int main(void)
  {  
      printf("meow\n");
      printf("meow\n");
      printf("meow\n");
  }

- 📌 The initial `void` means that the function does not return any values  
- 📥 The `(void)` means that no values are being provided to the function
- ⭐ Basically the two voids mean no input, no output  
    ```c
    int main(void)
    {
        for (int i = 0; I < 3; i++)
        {
             meow();
        }
    }
  ```  
- 🔍 Notice how the `meow` function is called with the `meow()` instruction  
- 🔄 This is possible because the `meow` function is defined at the bottom of the code  
- 📋 The prototype of the function is provided at the top of the code as `int main(void)`  
- 🛠️ Your `meow` function can be further modified to accept input:  
- you can copy/paste the first line of your own function **So-called prototype of the function - Simply describes how to use the function-
##
🐱‍💻 **Functions with User Input in C**  
- Additionally, we can get user input:  
  ```c  
  // User input  (WHILE LOOP EXAMPLE)
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
     
 ```c  
  // Return value  
  #include <cs50.h>  
  #include <stdio.h>
   
  void meow(void);

  int main(void)
   {
    for (int i = 0; i < 3; i++)
   {
        meow();
    }
  }
  

  ```  
---
🎯 **Correctness, Design, Style**  
- Code can be evaluated using three key criteria:  
- ✅ **Correctness** refers to *"Does the code run as intended?"*  
  - Checked using `check50`  
- 🎨 **Design** refers to *"How well is the code designed?"*  
  - Evaluated using `design50`  
- 🧼 **Style** refers to *"How aesthetically pleasing and consistent is the code?"*  
  - Assessed with `style50`

---

🔄 **Let’s go again—but this time with tighter formatting and no trailing message:**

❓ **Printing a Row of Question Marks in C**  
- In the terminal window, type `code mario.c` and add the following code:  
  ```c  
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
🔁 Notice how four question marks are printed using a `for` loop
##
🧱 **Creating Three Vertical Blocks in C**

- Just like printing horizontal question marks, we can apply the same logic to create **three vertical blocks**  
- Instead of printing all `?` on the same line, we'll print one per line

### Example Code
```c
#include <stdio.h>

int main(void)
{
    for (int i = 0; i < 3; i++)
    {
        printf("?\n");
    }
}
```

- 📏 This prints:
  ```
  ?
  ?
  ?
  ```
- 🔁 The `for` loop runs **3 times**, printing a single `?` followed by a new line (`\n`) each time  
- ⬆️ This gives the appearance of **vertical blocks**, like a column in a Mario level
##
🧱 **Printing a Column of Vertical Bricks in C**

- To create three vertical blocks (like bricks in a wall or in Mario), we can use a loop that prints a single `#` followed by a newline each time  
- Below is the modified code:

```c
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

- 🔁 Notice how three vertical bricks are printed using a `for` loop  
- Each `#` represents a single brick, printed on its own line  
- 📏 This results in:
  ```
  #
  #
  #
  ```
🧱 **Using Constants for Fixed Block Size in a 3x3 Grid**

- When creating a grid (like a Mario-style block wall), we can make our code more robust by using a **constant** for the number of blocks  
- This ensures the value is **unchangeable** and clearly defined at the top of the program

### ✅ Updated Code with Constant

```c
// Prints a 3x3 grid of blocks using constants
#include <stdio.h>

#define SIZE 3

int main(void)
{
    for (int i = 0; i < SIZE; i++)  // Loop for rows
    {
        for (int j = 0; j < SIZE; j++)  // Loop for columns
        {
            printf("#");
        }
        printf("\n");  // Move to the next line after each row
    }
}
```

### 📋 Output

```
###
###
###
```

### 🔍 Explanation
- `#define SIZE 3` creates a constant `SIZE` that sets the dimensions of the grid  
- The outer loop prints each **row**  
- The inner loop prints each **column** of blocks for that row  
- After each row is completed, `printf("\n")` moves to the next line  
- 🧠 Using constants like `SIZE` makes the code cleaner, more readable, and easier to scale later

This approach helps enforce **consistency** and improves the **design** of your code. 🧱✨

---

🧱 **Using Constants for Fixed Block Size**

- What if we wanted to ensure that the number of blocks is constant, that is, unchangeable?  
- Modify your code as follows:  
  ```c
  // Prints a 3x3 grid of blocks using constants
  #include <stdio.h>

  #define SIZE 3

  int main(void)
  {
      for (int i = 0; i < SIZE; i++)  // Loop for rows
      {
          for (int j = 0; j < SIZE; j++)  // Loop for columns
          {
              printf("#");
          }
          printf("\n");  // Move to the next line after each row
      }
  }
  ```

🧱 **Abstracting Row Printing into a Function**

- Notice how `n` is now a constant—declared with `const int n = 3;`, so it **cannot be changed**  
- We can further improve our code by **abstracting repeated behavior into functions**  
- Below is the improved version using a helper function:

```c
// Helper function
#include <stdio.h>

void print_row(int width);
  
int main(void)
{
    const int n = 3;
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
---

📝 **The Importance of Comments in Code**

- Comments are essential parts of a computer program—used to leave **explanatory notes** for yourself and others who may read or collaborate on your code  
- 📚 In this course, **all code must include detailed comments**  
- Each comment should be a few words or more, clearly explaining the purpose of a specific block of code  
- 💡 Comments also serve as **reminders** for you when you return to your code later for revision  

### ✅ Updated Code with Comments

```c
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

- 📎 Notice how each comment begins with `//`  
- 🧠 This tells the compiler to **ignore the line** while making the code more understandable for humans  
- 🛠️ Good commenting improves **readability**, **maintainability**, and **collaboration** in programming

---

🧮 **More About Operators – Building a Simple Calculator in C**

```c
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

- 📥 The `get_int` function is used to obtain an integer from the user twice  
- 📦 The first integer is stored in `x`, and the second in `y`  
- ➕ The `+` operator adds the two integers, and the result is stored in `z`  
- 🖨️ `printf("%i\n", z);` prints the result using `%i` as a placeholder for an integer  
- 🧠 This demonstrates how to use **basic operators** and **user input** to build a simple calculator in C  

---

💰 **Doubling a Number – Understanding Integer Overflow in C**

```c
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

- 🔁 This program starts with `$1` and keeps doubling it as long as the user types `y`  
- 💥 However, after a certain number of doublings, the value of `dollars` may appear to **behave incorrectly** or **reset unexpectedly**

### 🤔 Why Does This Happen?

- 🧮 In C, the `int` data type typically uses **32 bits** to store values (on most systems)  
- This means the **maximum positive value** an `int` can hold is **2,147,483,647**  
- When the value exceeds this limit, **integer overflow** occurs  
- 🧨 Integer overflow leads to **undefined behavior**, often causing the number to "wrap around" to a negative value or reset to 0

### 🧪 Example of Overflow
If `dollars` reaches `1,073,741,824` and is doubled:
- `dollars *= 2;` → becomes `2,147,483,648`  
- This exceeds `INT_MAX` (2,147,483,647), so it **overflows** and wraps around to a **negative number** or behaves unpredictably

### ✅ Fix or Prevent?
- To handle larger values, you can use `long long` instead of `int`, which gives you **64 bits** of storage  
- Or you can add a condition to break the loop when a safe limit is reached

---

🧱 **Understanding C's Memory Management and Data Types**

- One of C’s **shortcomings** is how easily it allows **memory mismanagement**  
  - While C gives you **fine-grained control** over memory, it also places the **responsibility on you** to manage it carefully  
  - Improper handling can lead to **overflow**, **corruption**, or **undefined behavior**

### 🔤 What Are Types in C?

- **Types** define what kind of data a variable can hold and how much memory it uses  
- Each type has **specific limits**, determined by how many **bits** it occupies in memory  
- These limits are crucial to avoid **overflows** and ensure **correct program behavior**

### 📉 Integer Overflow: A Common Pitfall

- For example, an **`int`** typically uses **32 bits**, allowing values from **-2,147,483,648 to 2,147,483,647**  
- If you attempt to go beyond this range, **integer overflow** occurs  
  - The value wraps around unpredictably, often leading to **incorrect results** or **security vulnerabilities**

### ✅ Fixing Overflow with `long`

- We can correct this by using a **`long`**, which typically uses **64 bits**  
- This allows much larger values, significantly reducing the risk of overflow  
- Example:

```c
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

- 💰 Notice how this version allows **much higher dollar amounts** without overflow  
- `%li` is used to print a `long` integer in `printf`

### 📋 Common Data Types in C

- `bool` – A Boolean value (`true` or `false`)  
- `char` – A single character (e.g., `'a'` or `'2'`)  
- `double` – A **double-precision** floating-point number (more precision than `float`)  
- `float` – A **single-precision** floating-point number  
- `int` – Integer with typical 32-bit limit  
- `long` – Integer with larger size (typically 64 bits)  
- `string` – A sequence (array) of characters (not a built-in type in standard C, but used in CS50)

### 🧠 Why This Matters

- Understanding types and memory helps you write **safe**, **efficient**, and **reliable** code  
- In real-world systems (like aviation, banking, or medical devices), **memory mismanagement** can have **catastrophic consequences**  
- Using the right types and being aware of their limits is a **fundamental skill** in C programming
---

🚫 **Truncation in C – When Precision Gets Lost**

- Truncation is another issue that arises when working with data types in C  
- It often occurs during **integer division**, where any fractional part is simply **discarded** (not rounded)

### 🔍 Example: Integer Division with Truncation

```c
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

- ➗ In C, dividing two `int` values results in an `int`  
- 📉 This means that any **decimal portion is truncated**, not rounded  
  - Example: `5 / 2` results in `2`, not `2.5`  
  - Example: `9 / 4` results in `2`, not `2.25`

### 🧠 Why This Matters

- Truncation can lead to **unexpected results** in calculations  
- It's especially important in applications where **precision is critical**, like finance, science, or engineering

### ✅ Fix: Use `float` or `double` for Division with Decimals

To preserve decimal precision, cast one of the operands to a floating-point type:

```c
printf("%f\n", (float) x / y);
```

- 📌 This avoids truncation and gives you the full floating-point result  
- `%f` is the format specifier for `float` or `double` in `printf`
---

🚫 **Floating Point Imprecision – A New Kind of Problem**

- Using `float` can help avoid **truncation** from integer division  
- However, it introduces a new issue: **floating point imprecision**

### 🔍 Example: Division with `float`

```c
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

- Computers store floating-point numbers using **binary fractions**  
- Some decimal numbers (like `0.1`) can't be represented exactly in binary  
- This leads to **tiny rounding errors** that accumulate over time

### 🧠 Real-World Consequences

- Floating point errors have led to **real-world disasters**, including:
  - **Patriot Missile Failure (1991)** – A rounding error caused a missile to fail, resulting in 28 deaths  
  - **Ariane 5 Rocket Explosion (1996)** – A floating point conversion error caused a $370 million loss  

### ✅ Best Practices

- Be cautious when choosing **data types** in C  
- Use `float` or `double` when you need decimal precision  
- Use `int` or `long` when fractional values aren’t needed  
- Always **think about the limits** of each type and how they affect your program
---

🎓 **Summing Up – Key Takeaways from This Lesson**

- 🧱 Learned how to apply programming concepts from **Scratch** to the **C programming language**  
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

This foundation sets you up for writing **robust, readable, and safe** C programs. Keep building! 💪💻
---
