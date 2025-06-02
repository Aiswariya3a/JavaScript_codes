## Loops in JavaScript

### Types of Loops

1. **`while`** – Checks the condition **before** each iteration.

   ```js
   while (condition) {
     // code
   }
   ```

2. **`do..while`** – Checks the condition **after** each iteration.

   ```js
   do {
     // code
   } while (condition);
   ```

3. **`for`** – Offers initialization, condition, and increment/decrement in one line. Condition is checked **before** each iteration.

   ```js
   for (let i = 0; i < 5; i++) {
     // code
   }
   ```

### Infinite Loops

Use `while (true)` for intentional infinite loops. Always include a `break` to stop it when needed.

```js
while (true) {
  if (shouldStop) break;
}
```

### `continue` and `break`

* **`break`** exits the loop immediately.
* **`continue`** skips to the next iteration.

### Labels with `break`/`continue`

Labels allow breaking out of or continuing outer loops from within nested loops.

```js
outer: for (let i = 0; i < 3; i++) {
  for (let j = 0; j < 3; j++) {
    if (j == 1) break outer;
  }
}
```

---