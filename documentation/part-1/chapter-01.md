# Part 1: PROGRAMMING FROM SCRATCH

## Chapter 1: What is Programming?

Your first steps in the world of programming. No experience needed.

### Chapter Objectives

By the end of this chapter you will be able to:

- Explain what programming is.
- Understand what code and programming languages are.
- Understand how computers follow instructions.
- Recognize TypeScript as a programming language.
- Open and use the TypeScript Playground.
- Write and execute their first TypeScript instructions.
- Use console.log() to display information.
- Perform basic mathematical operations using TypeScript.
- Recognize and fix simple syntax errors.

Nothing to install.

---

### 1.1 What is programming?

Imagine you wish to make a burger.

You don't think how many steps are involved. You take two slices of bread, between them you add mayonnaise, cheese, hamburger, some salad, maybe something extra and done!

But when you try to explain it to someone new you have to tell them in steps:

1. Take two slices of bread
2. Place one slice on a plate.
3. Put mayonnaise.
4. Put cheese.
5. Put hamburger.
6. Put salad.
7. Add extra things.
8. Put the second slice of bread.

This is what exactly one would describe programming is, you just tell all the exact steps for the computer to do.

So, programming is the method of writing the instructions for the computer to perform. If you miss a step then the computer will make the mistake.

Some examples of tasks:

- Calculate numbers.
- Create art.
- Play music.
- Play games.
- Using the internet.

Every software you ever used was created through programming that required specific instructions.

---

### 1.2 What is code?

Computers don't understand our human language and they have their own language.

That language is known as a programming language.

Some of the most popular programming languages are:

* TypeScript
* JavaScript
* Python
* C++
* Rust

Each of these languages has their own rules to follow and comes along with syntax.

Syntax simply means the combination rules, principles and structural patterns to combine symbols to create well formed code.

For example, lets look at a TypeScript example:

```typescript
console.log("Hello, World!");
```

This is a simple piece of code instructing the computer to display the text **Hello, World!** on the screen or console.
Don't worry about the extra stuff written, we'll go through them soon.

Congrats! We just saw our first line of code.

---

### 1.3 Meet TypeScript

TypeScript is a programming language developed and maintained by Microsoft.

It can be used to build applications, websites, tools and much more.

It was built on top of JavaScript and adds the static typing feature. Don't worry about this, we will explore this later.

For now, just know TypeScript is the language we will use to talk to computers and learn how to write it.

---

### 1.4 Your First Programming Environment

Normally, tutorials make you install all sorts of complicated tools and software before writing a single line of code.

We will not do that for now. Let's start writing code using the official **TypeScript Playground**.

> Write, edit, and execute TypeScript directly in your browser at [typescriptlang.org](https://www.typescriptlang.org/play).  
> *No account or software installation required for basic use.*

When you go to the site and open it, you will find an editor with some example TypeScript code. We will write our first programs here.

---

### 1.5 Writing Your First Code

Open the TypeScript Playground, delete the example code and just write:

```typescript
console.log("Hello, World!");
```

The playground will automatically compile and show your TypeScript on the right side through JavaScript output (we don't need to understand what that is for our book) but let's click on **Run** above.

This time you will see the clean output:

```text
Hello, World!
```

Congratulations! We have just written and executed our first TypeScript program.

---

### 1.6 Understanding the Instruction

Let's examine what we wrote:

```typescript
console.log("Hello, World!");

```

There are three important elements:

| Element | Meaning |
| --- | --- |
| `console` | A keyword that provides access to the console |
| `log()` | A method of displaying information |
| `"Hello, World!"` | The text we want to display |

You don't have to worry about memorizing all this stuff. Just for now let's understand:

> `console.log()` displays information.

---

### 1.7 Displaying Different Messages

Try replacing the message with multiple instructions on your own or use the examples available below:

```typescript
console.log("My name is John.");
console.log("I am learning TypeScript.");
console.log("This is my first programming language!");
```

The output we should see:

```text
My name is John.
I am learning TypeScript.
This is my first programming language!
```

Did you notice? No matter how many instructions, the computer executes them strictly **in order**: first instruction, second instruction, third instruction.

---

### 1.8 Making the Computer Do Mathematics

Programming is not only about displaying text messages. Computers are very powerful and can even do calculations.

Let's try:

```typescript
console.log(10 + 2);
```

**Output:**

```text
12
```

You can also do the four basic mathematical operations (and a few extras too):

```typescript
console.log(10 + 2);  // Addition
console.log(10 - 2);  // Subtraction
console.log(10 * 2);  // Multiplication
console.log(10 / 2);  // Division
```

**Output:**

```text
12
8
20
5
```

Here are some mathematical symbols you'll use regularly:

| Symbol | Operation |
| --- | --- |
| `+` | Addition |
| `-` | Subtraction |
| `*` | Multiplication |
| `/` | Division |
| `**` | Exponentiation |
| `%` | Remainder |

Try some practice on your own by changing the numbers around and seeing the results in your TS Playground!

---

### 1.9 Guided Exercises

Now for some practice. These exercises will help you to become comfortable writing and modifying code safely.

**Exercise 1:** Display your first name using `console.log()`.

<details>
<summary><b>Hint</b> (Click to reveal)</summary>

```typescript
console.log("Your name");
```
</details>

**Exercise 2:** Display the message: `I am learning TypeScript.`

<details>
<summary><b>Hint</b> (Click to reveal)</summary>

```typescript
console.log("The Text");
```
</details>

**Exercise 3:** Calculate `25 + 75`.

<details>
<summary><b>Hint</b> (Click to reveal)</summary>

```typescript
console.log(firstNumber + secondNumber);
```
</details>

**Exercise 4:** Calculate `150 - 45`.

<details>
<summary><b>Hint</b> (Click to reveal)</summary>

```typescript
console.log(firstNumber - secondNumber);
```
</details>

**Exercise 5:** Calculate `12` multiplied by `8`.

<details>
<summary><b>Hint</b> (Click to reveal)</summary>

```typescript
console.log(firstNumber * secondNumber);
```
</details>

---

### 1.10 Independent Challenges

Let's try some exercises but this time without step-by-step instructions.

**Challenge 1: Your Personal Introduction**

Write a program that displays:

* Your name.
* Your country.
* Your favourite hobby.
* Why you're learning programming.

*(Hint: Each item should appear on a separate line using its own `console.log()` statement).*

**Challenge 2: Shopping Calculator**

Imagine you've purchased:

* 3 coffees costing €2 each.
* 2 sandwiches costing €5 each.
* 1 dessert costing €4.

Write TypeScript instructions to calculate the total cost in a single calculation. Your program should display the final amount.
*(Hint: You can look at 1.8 for some help).*

**Challenge 3: Fix the Broken Program**

The following code contains errors:

```typescript
console.log("Hello, world!);
console.log(10 + );
console.log("I am learning TypeScript);
```

Find and correct all three syntax mistakes.
*(Hint: The TypeScript Playground might provide some hints).*

---

### 1.11 Practical Mini-Project: Build Your First Calculator

Now its time to build a simple calculator that will display results of many mathematical operations.

Your calculator program should:

1. Display a welcome message.
2. Display two numbers.
3. Calculate their sum.
4. Calculate their difference.
5. Calculate their product.
6. Calculate their division result.

For this first project, use the numbers **10** and **20**.

**Let me give you a headstart:**

```typescript
console.log("Welcome to my calculator!");
console.log("First number: 10");
console.log("Second number: 20");

// Add your calculations below.
```

Try to do the project on your own and if you have too trouble you can look at the solutions below!