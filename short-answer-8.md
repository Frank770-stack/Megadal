### **2️⃣ Short Answer Questions (2 Questions)**

8. **What are the key differences between `var`, `let`, and `const` in JavaScript?**

Write your answer here.
Be as detailed as possible.
You can provide a code snippet using markdown format.

### **Key Differences Between `var`, `let`, and `const` in JavaScript**

In JavaScript, `var`, `let`, and `const` are used to declare variables, but they have important differences in scope, hoisting, and mutability.

---

### **1. Scope**

- `var` is **function-scoped**, meaning it is only accessible within the function where it was declared.
- `let` and `const` are **block-scoped**, meaning they are only accessible within the block `{}` where they were defined.

```javascript
function example() {
  if (true) {
    var a = 10;
    let b = 20;
    const c = 30;
  }
  console.log(a); // ✅ 10 (function-scoped)
  console.log(b); // ❌ ReferenceError (block-scoped)
  console.log(c); // ❌ ReferenceError (block-scoped)
}
example();
```
