# 👨‍🏫 Harvard CS50 Foundations Notes 📓

⭐ This section will be for important notes as I go through the Harvard CS50's Foundations course.

##

## 🏫 SECTION: WEEK 0 SCRATCH

## -LECTURE VERBAL-

##
👌 LLM - probability/statistics - implimented through neural networks. Biology 0 neruins transmit electrial signals
zeos and ones each circle reps neron 
    -## 🧠 Pseudocode

📘 This process of converting instructions into code is called **pseudocode**.

✅ The ability to create pseudocode is **central to success** in both this class and in computer programming.

📝 **What is Pseudocode?**  
Pseudocode is a human-readable version of your code.  
For example, here’s how we might write pseudocode for searching a phone book:

Here is an example of a simple algorithm written in pseudocode:

```
1  Pick up phone book
2  Open to middle of phone book
3  Look at page
4  If person is on page
5      Call person
6  Else if person is earlier in book
7      Open to middle of left half of book
8      Go back to line 3
9  Else if person is later in book
10     Open to middle of right half of book
11     Go back to line 3
12 Else
13     Quit
```

## 🚨 Why Pseudocode Matters

🔑 **Pseudocoding is an essential skill for at least two reasons:**

1. 🧭 It allows you to **think through the logic** of your problem in advance — before writing actual code.
2. 📘 It helps you **communicate your logic clearly** to others who may want to understand your decisions and code.

## 🔧 Key Components of Pseudocode

🔍 Notice that pseudocode includes the following building blocks — the **fundamentals of programming**:

- **🛠 Functions**  
  Lines that begin with verbs like *pick up*, *open*, and *look at* — these represent actions.
  
- **❓ Conditionals**  
  Phrases like `if`, `else if` — these allow your code to make decisions.
  
- **🧮 Boolean Expressions**  
  Statements like *"person is earlier in the book"* — these evaluate to `true` or `false`.
  
- **🔁 Loops**  
  Instructions like *"go back to line 3"* — these allow you to repeat steps.

🌟 These building blocks form the foundation of programming.  


🧩 In Scratch (discussed below), we will use each of these basic building blocks.

# 🔮 What’s Ahead

📆 This week, you’ll dive into **Scratch**, a visual programming language designed to make learning to code fun and accessible.

🧠 Then, in the coming weeks, you’ll take your first steps into the world of **C**, a powerful and foundational programming language. Here's a sneak peek:

---

```markdown

#include <stdio.h>

int main(void)
{
  printf("hello, world\n");
}
```

## 🧱 Why Start with C?

🎯 Learning C will:
- 🧠 Sharpen your understanding of how computers work
- 💪 Prepare you for learning other languages like **Python**, **JavaScript**, and more
- 🛠️ Give you insight into the底层 (lower-level) mechanics of programming

## 🧩 What Comes Next?

🧬 As the course progresses, you’ll explore:
- 🔍 Algorithms – the logic behind solving complex problems
- 🧮 Data structures – how to organize and manage data efficiently
- 🚀 Performance optimization – making your code faster and smarter

## 🤯 Why Is C So Tricky?

❗ One of the biggest challenges in learning C is the **punctuation and syntax** — things like semicolons, curly braces, and pointer notation.

🧯 But don’t worry — we’re going to **set all that aside for now** and focus purely on the **ideas** behind programming using **Scratch**.

# 🎨 Scratch

🎓 **Scratch** is a visual programming language developed by MIT.

🧩 It uses the **same essential coding building blocks** we covered earlier in this lecture — like:

- 🛠️ Functions  
- ❓ Conditionals  
- 🔁 Loops  
- 🧮 Variables  

🌈 The big advantage?  
With Scratch, you can **focus on the logic and structure** of your programs without worrying about syntax details like:

- ❌ Curly braces `{}`  
- ❌ Semicolons `;`  
- ❌ Parentheses `()`  

🕹️ Scratch operates on a coordinate system

# 🎯 Meow and Abstraction

🧱 Along with pseudocoding, **abstraction** is a core skill and concept in computer programming.

## 🧩 What is Abstraction?

🧠 **Abstraction** means:
> Simplifying a complex problem by breaking it down into smaller, more manageable pieces.

### 🍽️ Real-World Example

Imagine you’re hosting a **big dinner** for your friends.  
The idea of cooking the entire meal might feel totally overwhelming! 😱

But what if you break it down?

- 🧅 Chop the vegetables  
- 🍳 Cook the sauce  
- 🍖 Prepare the main dish  
- 🍰 Bake the dessert  

Each step is **smaller and easier to handle** — and together, they make up the whole meal! 🍴

## 🔍 Abstraction in Programming

🛠️ Just like in cooking, **abstraction helps us manage complexity in code**.

In programming — and even in **Scratch** — you’ll see abstraction in action:

- 📦 Grouping related code into functions or blocks  
- 🧩 Reusing pieces of logic without repeating code  
- 🧹 Keeping your code clean, modular, and easy to understand  

🧠 Think of it like this:  
Abstraction lets you **focus on the big picture** while hiding the messy details behind a simplified interface.

🐱 And yes — even a simple "meow" block in Scratch is an example of abstraction! 🐾

🔎 Notice how even a few conversational responses require many lines of code.  
Now imagine handling **thousands or tens of thousands** of possible interactions — that’s a *lot* of code!

## 🧠 Modern AI: Training, Not Programming

🧠 Instead of hardcoding every interaction, AI developers **train large language models (LLMs)** using massive datasets.

📈 These models:
- 🔍 Analyze patterns in huge blocks of text
- 🤔 Predict what word or phrase is most likely to come next
- 🔄 Learn from context, not strict rules

## 💡 Why Use AI?

⚡ AI-based tools are incredibly useful in many areas of life and work:
- Writing
- Research
- Coding
- Problem-solving

### ✅ What is CS50.ai?

🤖 **CS50.ai** is an AI assistant designed to:
- 🆘 Help you when you're stuck
- 💡 Offer hints and guidance
- 🧠 Encourage your learning

# 🤖 Artificial Intelligence

🧠 Let's explore how we can use the programming building blocks to start building our own **artificial intelligence**.

## 🗣️ A Simple Example

Here’s a snippet of what **traditional rule-based AI** might look like in pseudocode:

```
If student says hello
    Say hello
Else if student says goodbye
    Say goodbye 
Else if student asks how you are
    Say well
Else if student asks why 111 in binary is 7 in decimal
    ...
```

🔎 Notice how even a few conversational responses require many lines of code.  
Now imagine handling **thousands or tens of thousands** of possible interactions — that’s a *lot* of code!

## 🧠 Modern AI: Training, Not Programming

🧠 Instead of hardcoding every interaction, AI developers **train large language models (LLMs)** using massive datasets.

📈 These models:
- 🔍 Analyze patterns in huge blocks of text
- 🤔 Predict what word or phrase is most likely to come next
- 🔄 Learn from context, not strict rules

## 💡 Why Use AI?

⚡ AI-based tools are incredibly useful in many areas of life and work:
- Writing
- Research
- Coding
- Problem-solving

🤖 **CS50.ai** is an AI assistant designed to:
- 🆘 Help you when you're stuck
- 💡 Offer hints and guidance
- 🧠 Encourage your learning

##
# 🚧 Roadblocks 

