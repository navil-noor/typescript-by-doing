# Chapter 2: Variables and Data Types

*Teaching your programs how to remember, naming values and working with various kinds of information (data).*

---

### 2.1 What is a variable?

Imagine that you are moving to a new house so you need to pack up your stuff in a box.

You take a cardboard box, put your books. Then take another box to put your kitchen items. Then another box to put your electronic devices.

Now when you take it to your new home you need to be able to know exactly which box contains which items.
So, to save your time you take a marker and write down on the boxes like **Books**, **Kitchen** or **Electronis**.

In programming, a **variable** is the same as a labeled cardboard box. It is a named container that goes into the computer's memory where you store an information to use later and even change when needed.

Without these variables your programs will have to recalculate and retype every single value and the program will become unnecessarily long, complicated and messy.

---

### 2.2 Creating Variables: `let` and `const`

In TypeScript, the two most common ways to create a variable are: `let` and `const`.

* **`let`** creates a box whose contents you can change later.
* **`const`** (short for *constant*) creates a box with a permanent seal and if you put something inside it, you can never replace it.

Let's look at some TypeScript examples of creating variables:

```typescript
let userName = "John";
const birthYear = 1998;

```

A detailed explanation of the first line:

1. **`let`** instructs the computer to: *"Create a new variable that I might change later."*
2. **`userName`** is the label or name we chose for our box.
3. **`=`** is the assignment operator which puts the value on the right which is inside the box.
4. **`"John"`** is the information or data with saved inside.
5. **`;`** finishes the instruction.

> **Which one should you use?**  
> Start with `const` by default. If you later think that the value needs to be changed (like a game score or a total needs to change), switch it to `let`.

---

### 2.3 Basic Data Types

When you are storing information you need to keep a simple logic in mind. Just like how you would not put soup inside a cardboard box, you need to put the correct data inside the correct container or space. These various kinds of information are known as **data types**.

For now, we only need to know and remember three core types:

| Data Type | What It Represents | Examples |
| --- | --- | --- |
| **String** | Plain text guarded by quotes | `"Hello"`, `"Alex"`, `"123"` |
| **Number** | Any numbers and decimals | `42`, `3.14`, `-10` |
| **Boolean** | True or false values | `true`, `false` |

> Notice that `"123"` in quotes is a **string** (text), while `123` without quotes is a **number** which you use for mathematical calculations.

---

### 2.4 Storing and Displaying Variables

Lets now try something, open the TypeScript Playground, clear the editor, and run the following code:

```typescript
const city = "Rome";
let temperature = 22;
const isSunny = true;

console.log(city);
console.log(temperature);
console.log(isSunny);

```

**Output:**

```text
Rome
22
true

```

**Did you notice?**

When we pass a variable name inside `console.log()`, we did **not** put quotes around it.

* `console.log(city);` prints the value stored inside the box (`Rome`).
* `console.log("city");` but using quotes like this would literally print the word: `city`.

---

### 2.5 Updating Variable Values

Now let's explore the differences between `let` and `const` with some examples. Copy and run this in your TypeScript Playground:

```typescript
let score = 0;
console.log(score);

score = 10;
console.log(score);

score = score + 5;
console.log(score);

```

**Output:**

```text
0
10
15

```

Focus on `score = score + 5;`.

In math, that looks impossible, right? But remember in algebra we do something similar, like `a + 5`, correct?

In programming, `=` means **assign**, not "equals" (this is a very important concept to remember).

The computer calculates the right side first (`10 + 5 = 15`), and then puts `15` back into the `score` box.

> **Important Rule:** You only write `let` once and only when you first create the variable. When you change it later, just use its name directly (`score = 10;`).

If you try to do the same thing with a `const` variable, TypeScript will immediately add a helpful red underline warning, and if you try to run it, an error will show up saying that a constant cannot be reassigned.

> **Try it out:** Just for the fun of it, change `let` to `const` in the code above and see what happens!

---

### 2.6 Combining Text and Variables

In real programs, we rarely just print raw numbers without any text but actually we combine them with text to make readable messages that you can understand like what is this value for.

The most efficient way to do this in TypeScript is using **template literals** that is basically text wrapped in backticks (``) instead of regular quotes, with `${}` around any variable you want to insert:

```typescript
const playerName = "John";
let level = 3;

console.log(`Welcome back, ${playerName}! You are on level ${level}.`);

```

**Output:**

```text
Welcome back, John! You are on level 3.

```

*(Tip: The backtick key `` is usually located at the top-left of your keyboard, right above the `Tab` key).*

---

### 2.7 Naming Rules & Best Practices

You can name your variables anything you like, almost, but you still need to follow a few simple rules:

1. You cannot have spaces (`user name` will break).
2. You cannot start with a number (`1stPlace` will break).
3. Always remember that names are case-sensitive (`age` and `Age` are treated as two completely different boxes).

In TypeScript, normally programmers use **camelCase** for multi-word names by starting with a lowercase letter and capitalizing each of the next new word:

* `firstName`
* `totalPrice`
* `isLoggedIn`

---

### 2.8 Guided Exercises

Lets practice trying to create, update and combine variables in your TypeScript Playground.

**Exercise 1:** Create a `const` variable named `favouriteFood` that stores your favourite food and displays it using `console.log()`.

```typescript
const favouriteFood = "Your food";
console.log(favouriteFood);
```

**Exercise 2:** Create a `let` variable named `currentAge` with your age, then print it, then update it to your age next year and finally print it again.

```typescript
let currentAge = 25;
console.log(currentAge);
currentAge = currentAge + 1;
console.log(currentAge);
```

**Exercise 3:** This time create two variables: `itemPrice` (`15`) and `quantity` (`3`). Next create a third variable called `totalCost` that multiplies them together and display the value of `totalCost`.

```typescript
const totalCost = itemPrice * quantity;
```

**Exercise 4:** Create two variables for `bookTitle` and `author` then use a template literal (``) to print: `I am currently reading [bookTitle] by [author].`

```typescript
console.log(`I am currently reading ${bookTitle} by ${author}.`);
```

**Exercise 5:** Create a boolean variable this time and name it `isRaining` set it to `false` and display it.

```typescript
const isRaining = false;
console.log(isRaining);
```

---

### 2.9 Independent Challenges

Now try to solve these without looking at the hints first!

**Challenge 1: Profile Card**
Create variables to store a user's:
- `username` (string)
- `followers` (number)
- `isVerified` (boolean)

Print a clean summary using template literals (using backticks) that displays all three pieces of information across separate lines.

<details>
<summary><b>Hint</b> (Click to reveal)</summary>

Use `const` for all three variables but remember to wrap your strings in backticks (``) so you can insert each variable using `${variableName}` across three separate `console.log()` statements.
</details>

**Challenge 2: Temperature Converter**
Store a temperature in **Celsius** inside a variable called `celsius` (for example, `25`).
Write a math formula that converts it to Fahrenheit and stores the result in a variable called `fahrenheit`.  
*(Formula: Multiply Celsius by `9`, divide by `5`, then add `32`).*
Display the result as: `25°C is equal to 77°F.`

<details>
<summary><b>Hint</b> (Click to reveal)</summary>

You can write the math formula directly when creating your variable: `const fahrenheit = (celsius * 9) / 5 + 32;`. Then use a template literal to print both variables inside the sentence.
</details>

**Challenge 3: Fix the Broken Code**
The code below has three mistakes. Find and fix them all:

```typescript
const userScore = 50;
userScore = 75;

let 2ndPlayer = "Sam";
console.log("Player: ${2ndPlayer}");
```

---

### 2.10 Practical Mini-Project: Upgrade Your Calculator

I hope you didn't forget about the calculator you built in Chapter 1. We had to type the numbers `10` and `20` over and over again for every single calculation which is bad practice and inefficient you know. If you wanted to test two new numbers you have to go back and change those numbers in each and every line. Miss and mistakes happen!

Time to upgrade our calculator using real variables so you only have to change the numbers in **one place**.

Your upgraded calculator must:

1. Store your two numbers in variables called `num1` and `num2` (for starting use `10` and `20` to test if it works).
2. Lets make the calculator better by storing the results of addition, subtraction, multiplication and division in their own variables (lets call them: `sum`, `difference`, `product`, `quotient`).
3. Print a clean and formatted report using template literals (``).

**Let me give you a headstart again:**

```typescript
const num1 = 10;
const num2 = 20;

// Store your calculations in variables below:


// Display your results using template literals below:
console.log(`Calculating results for ${num1} and ${num2}:`);
```

Once your program works as it should, test it out with some new likes like changing `num1` to `50` and `num2` to `5` then watch the entire output update automatically!