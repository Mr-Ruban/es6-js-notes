# ✅ ES6+ JavaScript – Arrow Functions

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

### Arrow Function (with return)

const add = (a, b) => {
  return a + b;
};

### Arrow Function (implicit return)

const add = (a, b) => a + b;

### ✅ Rules and Characteristics
- Arrow functions do not have their own this

- Arrow functions cannot be used as constructors (new)

- No arguments object (use rest parameters if needed)

- Great for short, anonymous functions


## 📌 Use-Case Examples
### Array Mapping
const numbers = [1, 2, 3, 4];
const squares = numbers.map(num => num * num);
console.log(squares); // [1, 4, 9, 16]

### Filtering Data
const users = [
  { name: "Anantha", active: true },
  { name: "Aswini", active: false }
];

const activeUsers = users.filter(user => user.active);
console.log(activeUsers); // [{ name: "Anantha", active: true }]

### Sorting
const prices = [500, 100, 800, 200];
const sorted = prices.sort((a, b) => a - b);
console.log(sorted); // [100, 200, 500, 800]

### As Callbacks in Event Listeners
document.getElementById("btn").addEventListener("click", () => {
  console.log("Button clicked!");
});

