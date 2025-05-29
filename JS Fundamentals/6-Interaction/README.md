# Browser Interaction in JavaScript

## Summary

JavaScript provides three **browser-specific modal functions** to interact with users:

### 🛎️ Interaction Methods

1. **`alert(message)`**
   - Displays a message to the user.
   - No return value.

2. **`prompt(message, default)`**
   - Shows a dialog asking for user input.
   - Returns the entered text, or `null` if the user cancels.

3. **`confirm(message)`**
   - Shows a dialog asking for confirmation (OK/Cancel).
   - Returns `true` if OK is pressed, `false` if Cancel or Esc is pressed.

---

### ⏸️ Modal Behavior

- These dialogs are **modal**:  
  They pause script execution and prevent interaction with the rest of the page until the dialog is dismissed.

---

### ⚠️ Limitations

- The **position** of these dialog boxes is controlled by the browser (usually centered).
- The **appearance** (style, font, buttons) is also browser-dependent and **cannot be customized**.

> 📝 While these methods are useful for simple tasks, custom dialogs built with HTML/CSS/JS offer more flexibility and a better user experience.

---

### Example

```javascript
alert("Welcome!");

let name = prompt("What is your name?", "Guest");
if (name !== null) {
  alert("Hello, " + name + "!");
}

let isConfirmed = confirm("Do you want to continue?");
if (isConfirmed) {
  alert("You chose to continue.");
} else {
  alert("You canceled the action.");
}
