# Chapter 3: Conditions and Decision-Making

*Teaching your programs how to think, make choices and react to different situations.*

---

### 3.1 Making Choices in Real Life (and Code)

On certain days like when it is cloudy, you look out the window or check your weather app before going outside. You check:
* **If** it is raining or will rain, you take an umbrella.
* **Or (else)**, you don't take an umbrella and wear sunglasses since its sunny.

Our current TypeScript programs have been running normally from top to bottom, executing every single line in a straight robot line. But real-world software or applications don't work like that and need to make decisions. An app needs to check if a username or password is correct, if you clicked a button or if you deleted something.

These checks are made through **conditions**. Conditions allow our code to ask questions, then evaluate if it is `true` or `false` so it can choose the correct instruction to execute based on our answer.

---

### 3.2 Asking Questions: Comparison Operators

Writing conditions is simple, you only need to compare between two or more values. In TypeScript this trick is known as **comparison operators** that can ask questions like *"Is this number bigger than the other number?"* or *"Are these two things identical?"*.

Below we have a table containing the most common comparison operators you will use on a regular basis:

| Operator | What It Asks | Example | Result |
| :--- | :--- | :--- | :--- |
| **`>`** | Greater than | `10 > 5` | `true` |
| **`<`** | Less than | `3 < 8` | `true` |
| **`>=`** | Greater than or equal to | `18 >= 18` | `true` |
| **`<=`** | Less than or equal to | `4 <= 2` | `false` |
| **`===`** | Strictly equal to | `"admin" === "admin"` | `true` |
| **`!==`** | Not equal to | `5 !== 3` | `true` |

> **Important:** Keep in mind that we use **three equals signs (`===`)** to confirm if two things are exact equals in TypeScript. But we use a single equal sign (`=`) to *assign* values to variables!

---

### 3.3 The `if` Statement

The most fundamental decision making word in all of programming is the **`if` statement**. It allows the computer to run a block of code *only* if a specific situation or circumstance is `true`.

Let's look at a very simple example in TypeScript:

```typescript
const age = 30;

if (age > 19) {
  console.log("Congrats, you are an adult!");
}
```

**Output:**

```text
Congrats, you are an adult!
```

Here is how the logic of an `if` statement works:

1. **`if`** tells the computer a decision needs to be taken.
2. **`(age > 19)`** is the question inside parentheses. If this is `true`, the computer goes inside the statement.
3. **`{ ... }`** (curly braces) enclose the block of code or statement that should run only when the condition is true.

If `age` was set to `15`, `15 > 19` would be `false`, and the computer would just simply skip our message inside the curly braces then continue to the next line. In this case output would be blank! You can test it in your playground and see for yourself.

---

### 3.4 Handling the Alternative: The `else` Statement

We saw when the condition is `false` nothing happens, but what if you still want your program to do *something* instead of the *blank* we saw in the previous section?

That's where `if`'s companion, known as **`else`** statement comes in as your fallback plan:

```typescript
const hungry = "no";

if (hungry === "yes") {
  console.log("Let's eat a sandwich!");
} else {
  console.log("We don't need to eat now!");
}
```

**Output:**

```text
We don't need to eat now!
```

* If `hungry` is `yes`, the first block runs.
* If `hungry` is anything other than `yes`, the computer automatically drops down into the `else` block and runs that code instead.