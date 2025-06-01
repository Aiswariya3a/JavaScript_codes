# 📘 JavaScript Learning Tracker

Welcome to my daily JavaScript learning journey! This README helps keep track of the topics I’ve covered each day.

---

## ✅ Day 1 – JavaScript Basics

### 📌 Topics Covered

- **`<script>` Tag**
  - Embedding JavaScript in HTML using the `<script>` tag.
  - External scripts with `src` attribute.

- **JavaScript Code Structure**
  - JavaScript statements are syntax constructs that perform actions.
  - You can write multiple statements in your script.
  - Statements are **usually** separated by semicolons (`;`), but in many cases, JavaScript automatically inserts semicolons where line breaks occur (called *automatic semicolon insertion*).
  - However, there are exceptions where line breaks don’t count as semicolons.
  - It's recommended to **always use semicolons** to avoid unexpected behavior.

- **Modern Mode – `"use strict"`**
  - Introduced with ECMAScript 5 (ES5) in 2009.
  - `"use strict"` is a special directive that enables modern, stricter parsing and error handling.
  - It must be placed at the top of the script or at the beginning of a function.
  - Helps catch errors and disables outdated or error-prone features.
  - Once enabled, it cannot be turned off within the script.

- **Variables in JavaScript**
  - `let`, `const`, and `var` declarations.
  - Naming conventions and best practices.

- **Data Types in JavaScript**
  - 7 primitive types: `number`, `bigint`, `string`, `boolean`, `null`, `undefined`, `symbol`
  - 1 non-primitive type: `object`
  - Usage of `typeof` operator.

- **User Interaction**
  - `alert(message)` – Shows a simple message.
  - `prompt(message, default)` – Asks the user for input.
  - `confirm(message)` – Requests confirmation from the user.

---

## ✅ Day 2 – Type Conversion

### 📌 Topics Covered

- **String Conversion**
  - Happens when outputting values.
  - Explicit conversion using `String(value)`.

- **Numeric Conversion**
  - Occurs in mathematical operations.
  - Explicit conversion using `Number(value)`.
  - Common conversion rules:
    - `undefined` → `NaN`
    - `null` → `0`
    - `true` / `false` → `1` / `0`
    - `" "` (space string) → trimmed and parsed
    - `""` → `0`

- **Boolean Conversion**
  - Occurs in logical contexts.
  - Explicit conversion using `Boolean(value)`.
  - Falsy values: `0`, `null`, `undefined`, `NaN`, `""`
  - All other values are truthy.

- **Common Pitfalls**
  - `undefined` becomes `NaN` (not `0`)
  - `"0"` and `" "` are truthy values

---

## ✅ Day 3 – Basic Operations & Comparisons

### 📌 Topics Covered

- **Basic Math Operations**
  - Addition (`+`), subtraction (`-`), multiplication (`*`), division (`/`), remainder (`%`), exponentiation (`**`)

- **String Concatenation**
  - `+` operator concatenates strings:
    ```js
    "Hello" + " world" // "Hello world"
    ```
  - Mixed types trigger string conversion:
    ```js
    "1" + 2 // "12"
    ```

- **Unary `+`**
  - Converts non-numbers to numbers:
    ```js
    +true // 1
    +""   // 0
    ```

- **Operator Precedence**
  - Parentheses `()` override order.
  - unary > Exponentiation `**` > multiplication/division > addition/subtraction > assignment

- **Assignment & Shorthand Operators**
  - Simple: `x = value`
  - Compound: `x += 1`, `x *= 2`, etc.

- **Increment & Decrement**
  - `++x` / `x++` (prefix/postfix increment)
  - `--x` / `x--` (prefix/postfix decrement)

- **Bitwise Operators**
  - `&`, `|`, `^`, `~`, `<<`, `>>`, `>>>`
  - Used for low-level operations on 32-bit binary numbers.

- **Comma Operator**
  - Evaluates multiple expressions, returns the last one:
    ```js
    let x = (1 + 2, 3 + 4); // x = 7
    ```

- **Comparison Operators**
  - `<`, `>`, `<=`, `>=`, `==`, `!=`, `===`, `!==`
  - Lexicographical comparison for strings.
  - Mixed types get converted (except strict equality).
  - `null == undefined` is true.
  - Be cautious with `null` or `undefined` in comparisons.

---
## ✅ Day 4 – Conditional Branching, Logical Operators & Nullish Coalescing

### 📌 Topics Covered

* **Conditional Branching: `if`, `else`, `else if`**

  * `if (condition)` executes a block if the condition is truthy.
  * `else` runs when the condition is falsy.
  * `else if` checks additional conditions.
  * Always use curly braces `{}` for better readability.

* **Boolean Conversion in Conditions**

  * Falsy values: `0`, `""`, `null`, `undefined`, `NaN`
  * All other values are truthy.
  * Conditions can use direct expressions or pre-evaluated booleans.

* **Conditional (Ternary) Operator `?`**

  * Short form of if–else:

    ```js
    let result = condition ? value1 : value2;
    ```
  * Can be nested for multiple conditions, though less readable.
  * Best used for value assignment, not code execution.

* **Logical Operators: `||`, `&&`, `!`**

  * `||` returns the first truthy value or the last one.
  * `&&` returns the first falsy value or the last one if all are truthy.
  * `!` negates a boolean.
  * Used for control flow and short-circuit evaluation.

* **Nullish Coalescing Operator `??`**

  * Returns the first defined value (not `null` or `undefined`):

    ```js
    let height = userHeight ?? 100;
    ```
  * Does **not** treat `0`, `false`, or `""` as undefined.
  * Has precedence of 3; MUST use parentheses when combining with `||` or `&&`.
  ---

## 📅 Progress Log

| Day | Topics Covered                                                                 |
|-----|---------------------------------------------------------------------------------|
| 1   | Script tag, Code structure, use strict, Variables, Data types, Interaction     |
| 2   | Type Conversion                                                                |
| 3   | Basic Operations, String Concatenation, Unary +, Operator Precedence,          |
|     | Assignment, Shorthand Operators, Inc/Dec, Bitwise, Comma, Comparisons          |
| 4   | Conditional Branching, Logical Operators, Nullish Coalescing Operator `??` |

---

