# JavaScript Type Conversions

## Summary

JavaScript automatically or explicitly converts values between different types. The **three most commonly used type conversions** are:

---

### 🔤 String Conversion

- Happens when outputting values (e.g., `alert`, `console.log`).
- Explicit conversion: `String(value)`
- Primitive values convert in a straightforward manner.

---

### ➕ Numeric Conversion

- Happens in mathematical operations.
- Explicit conversion: `Number(value)`
- Conversion rules:

| Value          | Converts To |
|----------------|-------------|
| `undefined`    | `NaN`       |
| `null`         | `0`         |
| `true` / `false` | `1` / `0` |
| `""` (empty string) | `0`   |
| `" 123 "`      | `123` (whitespace is trimmed) |
| Invalid string | `NaN`       |

---

### 🔁 Boolean Conversion

- Happens in logical operations and condition checks.
- Explicit conversion: `Boolean(value)`
- Conversion rules:

| Value                      | Converts To |
|----------------------------|-------------|
| `0`, `null`, `undefined`, `NaN`, `""` | `false` |
| Any other value            | `true`      |

---

### ⚠️ Common Pitfalls

- `undefined` becomes `NaN` when converted to a number, **not** `0`.
- Strings like `"0"` and `" "` (space-only) are **true**, not false.

---
