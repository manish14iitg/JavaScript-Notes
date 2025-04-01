# JavaScript Dialog Boxes 🗨️

Interactive dialog boxes for user interaction in JavaScript. Supports:
- Alert boxes ⚠️
- Confirm dialogs ❓  
- Prompt dialogs ✏️

## Table of Contents
1. [Alert Box](#alert-box-)
2. [Confirm Dialog](#confirm-dialog-)
3. [Prompt Dialog](#prompt-dialog-)
4. [Best Practices](#best-practices-)

---

## Alert Box ⚠️
Displays a message with an OK button.

```javascript
alert("This is an alert message!");
Features:

Blocking (pauses execution until dismissed)

No return value

Browser-native styling

## Confirm Dialog ❓
Asks for confirmation with OK/Cancel buttons.


const userConfirmed = confirm("Do you want to proceed?");
if (userConfirmed) {
  console.log("User clicked OK");
} else {
  console.log("User clicked Cancel");
}
Returns:

true if OK clicked

false if Cancel clicked

## Prompt Dialog ✏️
Collects user input with text field.

javascript
Copy
const userName = prompt("Please enter your name:", "John Doe");
if (userName !== null) {
  console.log(`Hello, ${userName}!`);
}
Parameters:

Message (required)

Default value (optional)

Returns:

Entered string or null if canceled
