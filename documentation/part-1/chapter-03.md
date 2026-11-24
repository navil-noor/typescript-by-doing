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