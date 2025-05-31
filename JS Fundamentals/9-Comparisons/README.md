# JavaScript Comparison Operators

## Summary

Comparison operators in JavaScript are used to compare values and return a **boolean** (`true` or `false`).

---

### ⚖️ Basic Comparison Operators

| Operator | Meaning           |
| -------- | ----------------- |
| `>`      | Greater than      |
| `<`      | Less than         |
| `>=`     | Greater or equal  |
| `<=`     | Less or equal     |
| `==`     | Loose equality    |
| `===`    | Strict equality   |
| `!=`     | Loose inequality  |
| `!==`    | Strict inequality |

---

### 📝 String Comparison

- Strings are compared **character by character** using **dictionary (lexicographical) order** based on Unicode values.

```javascript
"apple" < "banana"; // true
"Zoo" > "apple"; // false, because uppercase "Z" comes before lowercase "a"
```

---

### 🔄 Type Conversion in Comparisons

- When comparing **different types**, JavaScript automatically converts values to **numbers** (except with `===` and `!==` which do **not** perform type conversion).

```javascript
"5" == 5; // true (type conversion happens)
"5" === 5; // false (strict comparison, no conversion)
true == 1; // true
null == 0; // false
```

---

### ⚠️ Special Cases: `null` and `undefined`

- `null` and `undefined` are **loosely equal** to each other:

```javascript
null == undefined; // true
```

- But they are **not equal** to any other value:

```javascript
null == 0; // false
undefined == false; // false
```

- Using relational operators (`<`, `>`, `<=`, `>=`) with `null` or `undefined` can produce **unexpected results**:

```javascript
null > 0; // false
null == 0; // false
null >= 0; // true (converted to 0, then compared)
undefined > 0; // false
undefined < 0; // false
```

✅ **Best Practice**: Always check for `null` and `undefined` explicitly before using relational comparisons.

```javascript
if (value != null && value > 10) {
  // safe comparison
}
```

---

### ✅ Summary Tips

- Use `===` and `!==` for most comparisons to avoid unintended type coercion.
- Be cautious with `null` and `undefined` in comparisons.
- Know that string comparisons are case-sensitive and based on Unicode order.

---
