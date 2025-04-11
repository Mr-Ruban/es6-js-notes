✅ ES6+ JavaScript – Arrow Functions

## 🔹 What are Arrow Functions?

Arrow functions are a concise way to write functions in JavaScript introduced in ES6. They provide:

- Shorter syntax
- Lexical `this` binding (inherits `this` from the surrounding context)
- Cleaner and more readable code (especially for callbacks and one-liners)

---

## 🔧 Syntax

### Traditional Function

function add(a, b) {
  return a + b;
}

# Arrow Function (with return)

const add = (a, b) => {
  return a + b;
};

# Arrow Function (implicit return)

const add = (a, b) => a + b;

