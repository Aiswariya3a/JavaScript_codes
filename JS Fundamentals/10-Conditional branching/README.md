## Conditional Branching in JavaScript: `if` and `?`

JavaScript allows decision-making using two main constructs: the `if` statement and the conditional (`?`) operator.

### `if` Statement

The `if` statement checks a condition and executes code if the condition is true.

```js
if (condition) {
  // code block
}
```

Use curly braces `{}` even for single statements to maintain readability.

### Boolean Conversion

JavaScript automatically converts values in conditions to boolean:

* Falsy values: `0`, `""`, `null`, `undefined`, `NaN`
* All other values are true

```js
if (0) { ... } // won't execute
if (1) { ... } // will execute
```

### `else` and `else if`

* `else` runs if the `if` condition is false.
* `else if` lets you check multiple conditions sequentially.

```js
if (x < 10) {
  // ...
} else if (x < 20) {
  // ...
} else {
  // ...
}
```

### Conditional (`?`) Operator

Also called the ternary operator, this provides a concise way to assign values based on conditions.

```js
let result = condition ? value1 : value2;
```

Example:

```js
let accessAllowed = (age > 18) ? true : false;
```

If the condition is complex, use parentheses for readability.

### Nested `?` Operators

Multiple conditions can be chained:

```js
let message = (age < 3) ? 'Hi, baby!' :
              (age < 18) ? 'Hello!' :
              (age < 100) ? 'Greetings!' :
              'What an unusual age!';
```

This is equivalent to multiple `if...else` blocks.

### Misuse of `?` for Side Effects

Avoid using `?` for executing different code branches (like `alert(...)`). Use `if` instead for clarity:

```js
// Not recommended
(condition) ? doSomething() : doSomethingElse();

// Preferred
if (condition) {
  doSomething();
} else {
  doSomethingElse();
}
```

Use the `?` operator to **return** values based on conditions, not for general control flow.

---
