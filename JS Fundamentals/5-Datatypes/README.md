# JavaScript Data Types

## Summary

JavaScript has **8 basic data types**, which include **7 primitive types** and **1 non-primitive type**.

### 🧩 Primitive Data Types

1. **`number`** – For all kinds of numbers (integers and floating-point). Limited by ±(2<sup>53</sup> - 1).
2. **`bigint`** – For integers of arbitrary length.
3. **`string`** – For textual data. Strings can contain zero or more characters.
4. **`boolean`** – Represents logical values: `true` or `false`.
5. **`null`** – Represents an unknown or empty value. Has one value: `null`.
6. **`undefined`** – Indicates a variable has been declared but not assigned. Has one value: `undefined`.
7. **`symbol`** – Used for creating unique identifiers.

### 🧱 Non-Primitive Data Type

- **`object`** – Used for more complex data structures like arrays, functions, and objects.

---

### 🔍 The `typeof` Operator

- Used to check the data type of a variable.
- Syntax:  
  ```js
  typeof x    // or typeof(x)
