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