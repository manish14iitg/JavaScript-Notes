# JavaScript Data Types

JavaScript data types are categorized into two types:

## Primitive Data Types

### 1. Number
Numbers include both integers and floating-point values:
```js
8, 10, 1000000, 8.9, -9.5, 1/3
```

### 2. String
Strings can be defined using single quotes (`'`), double quotes (`"`), or backticks (`` ` ``):
```js
'Manish' OR "Manish" OR `Manish`
```
Backticks (`` ` ``) are used for multi-line strings and string interpolation.

#### String to Number Conversion
```js
'100' // This is a string
+'100' OR -'100' // Converts to number
+'Manish' // NaN (Not a Number)
+'100Manish' // NaN
parseInt('100Manish') // 100 (Converted to a number)

'' + 100 OR 100 + '' // '100' (String conversion)
```

### 3. Boolean
Booleans represent `true` or `false` values:
```js
true OR false
+true // 1
+false // 0
```

### 4. Undefined
A variable that has been declared but not assigned a value.

### 5. Null
`null` is an empty value:
```js
+null // 0
```
**Note:** `typeof null` returns **Object** (this is a known JavaScript quirk).

### 6. BigInt
Used for very large integers.

### 7. Symbol
Used to create unique identifiers.

---
This document provides an overview of JavaScript primitive data types.

