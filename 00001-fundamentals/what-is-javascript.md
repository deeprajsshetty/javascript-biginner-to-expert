# What is JavaScript?

JavaScript (JS) is a **high-level, interpreted programming language** that is one of the core technologies of the World Wide Web, alongside HTML and CSS.

- Created by **Brendan Eich** in 1995 at Netscape.
- Initially developed in **10 days** and named _Mocha_, then _LiveScript_, and finally **JavaScript**.
- Standardized under **ECMAScript (ES)** by **ECMA International**.

---

## ✨ Key Features

- **Interpreted & Just-in-Time Compiled** – Runs directly in browsers using JavaScript Engines (like V8 in Chrome).
- **Dynamic Typing** – Variables can hold values of any type.
- **Weakly Typed** – Type coercion is allowed (e.g., `5 + "5" = "55"`).
- **Prototype-Based OOP** – Uses prototypes instead of classical inheritance.
- **First-Class Functions** – Functions are treated as values.
- **Asynchronous by Nature** – Supports callbacks, promises, and async/await.

---

## 🌍 Where is JavaScript Used?

- **Web Development**
  - Frontend: DOM Manipulation, Events, UI
  - Backend: Node.js
- **Mobile Apps**: React Native, Ionic
- **Desktop Apps**: Electron.js
- **Game Development**
- **IoT & AI Applications**

---

## ⚡ Example: Hello World

```javascript
console.log('Hello, JavaScript!');
```

```Output
Hello, JavaScript!
```

## ⚡ Diagram: JS Ecosystem

   [ HTML ]   [ CSS ]   [ JavaScript ]
      |          |           |
      |----------|-----------|
                 ↓
         Web Applications

## 📚 References
- [MDN – JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [ECMAScript Specification](https://tc39.es/ecma262/)
- [JavaScript.info](https://javascript.info/)


```markdown
# How JavaScript is Executed?

JavaScript is executed in **JavaScript Engines** embedded inside browsers (e.g., V8 in Chrome, SpiderMonkey in Firefox).

---

## 🚀 Steps of Execution
1. **Parsing** – JS code is parsed into an Abstract Syntax Tree (AST).
2. **Compilation** – Modern engines use **JIT (Just-in-Time Compilation)**.
3. **Execution** – The engine executes machine code.
4. **Garbage Collection** – Automatic memory management.

---

## 📊 Diagram: JS Engine Workflow

Parser → AST → Interpreter → Bytecode → Optimizer → Machine Code

---

```markdown
# Dynamic vs Weakly Typed in JavaScript

---

## Dynamic Typing
JavaScript is **dynamically typed**, meaning variable types are decided at runtime.

```javascript
let x = 42;     // number
x = "Hello JS"; // string

## Weak Typing
JavaScript is weakly typed, meaning type coercion happens automatically.  JS converts types when needed.

```javascript
console.log(5 + "5");   // "55"  (number → string)
console.log("5" * 2);   // 10    (string → number)

## ⚠️ Implications
Pros: Flexibility, faster prototyping
Cons: Unexpected bugs due to coercion

---

```markdown
# JavaScript Host Environment

JavaScript does not run alone – it requires a **host environment** like a **browser** or **Node.js**.

---

## 🌍 Browser Environment
- Provides APIs: `document`, `window`, `fetch`, `localStorage`
- Enables DOM Manipulation and Events

Example:
```javascript
document.getElementById("demo").innerText = "Hello, Browser!";

## 🖥️ Node.js Environment
- Provides APIs: fs, http, os, process
- Enables server-side programming

```Node
const fs = require("fs");
fs.writeFileSync("hello.txt", "Hello Node.js");

📊 Diagram: JS Host Environment

      +----------------------+
      |  JavaScript Engine   |
      +----------------------+
      |  Host APIs           |
      |  (Browser / Node.js) |
      +----------------------+
