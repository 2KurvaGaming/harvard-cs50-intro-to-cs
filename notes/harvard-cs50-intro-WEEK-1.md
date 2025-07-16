# 👨‍🏫 Harvard CS50 Foundations Notes 📓

⭐ This section will be for important notes as I go through the Harvard CS50's Foundations course.
##
## 🏫 SECTION: WEEK 1 - Language C

## LECTURE/ VERBAL 
### 🧑‍💻 KEY LESSONS🚀
**📘 Visual Studio Code for CS50** Coding playground —  where the magic begins✨
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
- 🖥️ **IDE (Integrated Development Environment)**: On the left side is the file explorer where you can find your files. In the middle is the text editor where you write and edit your programs. At the bottom is the terminal window where you can interact with the system using commands.  
- 🖱️ **Terminal Window (CLI)**: This is where you type commands to communicate directly with the computer in the cloud. It’s powerful, fast, and essential for developers.  
- 📁 **`cd`**: Use this to move between folders — like walking through different rooms in a house.  
- 📄 **`cp`**: Copy files or folders — like making a duplicate of a document.  
- 📋 **`ls`**: List all the files in your current folder — like checking what’s inside a drawer.  
- 📁 **`mkdir`**: Create a brand-new folder — your own custom storage space.  
- 🔄 **`mv`**: Move or rename files — like picking up a file and placing it somewhere else or giving it a new name.  
- 🗑️ **`rm`**: Delete files — use with care, there's no undo button!  
- 🗑️📁 **`rmdir`**: Delete entire folders — again, double-check before hitting enter!
---
### 📋 Exploring the Terminal  
- 📋 **`ls`**: **The most commonly used command** — lists all the files in the current directory. 
- 🖥️ **Preconfigured IDE**: Because this IDE is set up with all the necessary software, you should use it to complete all assignments for this course.
---
# 👋 Hello World

### 💻 Writing, Compiling, and Running Your First Program  
- 📄 **`code hello.c`**: Opens the text editor to create your first C file — this is where you'll write your code.  
- ⚙️ **`make hello`**: Compiles your code into machine-readable format — turning your ideas into something the computer understands.  
- ▶️ **`./hello`**: Runs your compiled program — watch your code come to life!  

```bash
code hello.c
make hello
./hello
```
### 💻 Building Your First C Program  
- 📄 **`code hello.c`**: Creates a new file and opens the text editor — this is where you'll write your first program.  
- ⚙️ **`make hello`**: Compiles your C code into an executable file named `hello`.  
- ▶️ **`./hello`**: Runs the compiled program — your first step into the world of C programming!  

```bash
code hello.c
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
- 🖥️ **`make hello`**: Switch back to the terminal and run this command to compile your code. Notice we *omit* `.c` — `make` automatically looks for `hello.c` and turns it into an executable program called `hello`.  
- ✅ **No errors?** Great! That means your code compiled successfully — you’re ready to run it.  
- ❌ **Errors?** No worries — double-check your code to make sure it matches exactly. Even one typo can stop the process.  
- ▶️ **`./hello`**: Run your program with this command. Watch as it prints `hello, world` to the screen!  
- 📁 **File Explorer (left panel)**: Open it to see both `hello.c` (your readable source code) and `hello` (the compiled, executable file that the computer runs).
