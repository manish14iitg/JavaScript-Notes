Here's the complete, ready-to-copy markdown file with your JavaScript variables guide, enhanced with emojis and clear formatting:

```markdown
# JavaScript Variables Guide 📝

Learn about `let`, `const`, and `var` in JavaScript with examples! 🚀

---

## `let` Keyword 🆕
```javascript
let username = "Manish";          // Declare + Initialize
let intro = "My name is Manish Kumar";
let firstName = "Manish";
let lastName = "Kumar";
let userIntro = "My Name is " + firstName + " " + lastName; // String concatenation
```

### Key Behaviors 🔑
- **Hoisting**: 
  ```javascript
  let a;          // ✅ a = undefined (but cannot be accessed before declaration)
  let b = a + 5;  // ❌ ReferenceError (a is in TDZ)
  a = 10;
  ```
  - `console.log(b)` → `NaN` (Not a Number)
  - `console.log(a)` → `10`

- **Scope**: Block-scoped (`{ }`)

---

## `const` Keyword 🔒
```javascript
const name = "Manish";  // Must initialize during declaration
```
### Rules ⚠️
- ❌ Cannot reassign values
- ✅ Block-scoped (like `let`)
- Example:
  ```javascript
  const PI = 3.14;
  PI = 3.14159; // ❌ TypeError (Assignment to constant)
  ```

---

## `var` Keyword 🏷️ (Legacy)
```javascript
var age = 25;  // Function-scoped
```
### Quirks 🤔
- **Hoisting**:
  ```javascript
  console.log(x); // undefined (not an error!)
  var x = 10;
  ```
- ❌ No block scope (leaks outside `{ }`)

---

## Comparison Table 📊

| Feature        | `let`         | `const`       | `var`          |
|---------------|--------------|--------------|----------------|
| Scope         | Block        | Block        | Function       |
| Reassignable? | ✅ Yes       | ❌ No        | ✅ Yes         |
| Hoisting      | TDZ (Error)  | TDZ (Error)  | ✅ (undefined) |
| Modern Use?   | Preferred    | Preferred    | Avoid          |

> **Tip**: Always prefer `const` by default, use `let` when rebinding is needed, and avoid `var` in modern code. 🎯

---

## Temporal Dead Zone (TDZ) ⚡
- Accessing `let`/`const` before declaration throws an error:
  ```javascript
  console.log(y); // ❌ ReferenceError (TDZ)
  let y = 20;
  ```

---

Happy Coding! 💻✨
