# 🎉 **Session 2: Introduction to JavaScript – Code Like a Superhero!** 🎉  

🚀 **Mission:** Make Websites Dynamic & Accessible!  
💡 **Theme:** JavaScript is the **magic** behind interactive websites! Today, we’ll learn how to **store data, make decisions, create loops, interact with web pages**, and **build fun projects**!  

🔹 **Superpowers unlocked:**  
✅ Variables & Data Types 🏆  
✅ Basic Math Operations 🔢  
✅ Conditional Statements 🧐  
✅ Arrays & Loops 🔄  
✅ DOM Manipulation 🎨  
✅ Interactive Web Elements ✨  

---

## **📖 Lesson Breakdown**  

### **👀 Part 1: What is JavaScript?**  
🔹 JavaScript makes websites **dynamic**! Unlike HTML & CSS (which structure and style a webpage), **JS brings it to life** with animations, interactions, and logic!  

🎯 **Why does it matter?**  
- Makes websites **responsive** & **interactive**  
- Helps with **form validation** and user-friendly experiences  
- Powers **games, animations, and apps**  
- Improves **accessibility** for users with different needs  

---

## **🛠️ Lab Challenges: Hands-on JavaScript!**  

### **🚀 Challenge 1: Superhero Variables** 🦸‍♀️🦸‍♂️  
📌 **Task:** Create a JavaScript file (`script.js`) and declare variables for:  
- Your **favorite superhero** 🦸  
- The number of **pizzas** you can eat 🍕  
- The **best movie** you’ve seen 🎬  

```js
let superhero = "Wonder Woman";
let pizzasEaten = 5;
let bestMovie = "Inception";

console.log("Superhero: " + superhero);
console.log("Pizzas I can eat: " + pizzasEaten);
console.log("Best Movie: " + bestMovie);
```

🎯 **Bonus:** Add a **fun fact** variable about yourself!  

---

### **🚀 Challenge 2: Math Game – Buy All the Snacks!** 🍩☕🍪  
📌 **Task:** Solve some math problems in JavaScript.  

#### **2a: Addition – Breakfast Cost 💰**  
```js
let coffeePrice = 3.5;
let croissantPrice = 2.5;
console.log("Total cost: $" + (coffeePrice + croissantPrice));
```

#### **2b: Subtraction – Money Left After a Donut 🍩**  
```js
let wallet = 10;
let donutPrice = 1.5;
console.log("Money left: $" + (wallet - donutPrice));
```

#### **2c: Multiplication – How Many Ice Creams Can You Buy? 🍦**  
```js
let iceCreamPrice = 2;
let totalMoney = 20;
console.log("Ice creams I can buy: " + (totalMoney / iceCreamPrice));
```

#### **2d: Division – Sharing is Caring! 🍬**  
```js
let candies = 24;
let friends = 4;
console.log("Each friend gets: " + (candies / friends) + " candies");
```

🎯 **Bonus:** Make the console log a **fun message**!  

---

### **🚀 Challenge 3: Jacket or No Jacket? (Conditional Statements)** 🧥❄️☀️  
📌 **Task:** Write a script that checks if the temperature **requires a jacket**!  

```js
let temperature = 15; // Try changing this value
if (temperature < 20) {
  console.log("It's jacket weather! 🧥");
} else {
  console.log("No jacket needed! ☀️");
}
```

🎯 **Bonus:** Use `prompt()` to let **users enter the temperature**!  

---

### **🚀 Challenge 4: Travel Bucket List (Arrays & Loops)** ✈️🌍  
📌 **Task:** Store your **dream travel destinations** in an array and **log them one by one**!  

```js
let destinations = ["Bali", "Iceland", "Japan", "Italy"];
for (let i = 0; i < destinations.length; i++) {
  console.log("I want to visit: " + destinations[i]);
}
```

🎯 **Bonus:** Make a **random travel picker**!  

```js
let randomDestination = destinations[Math.floor(Math.random() * destinations.length)];
console.log("You should visit: " + randomDestination + "! 🌍");
```

---

### **🚀 Challenge 5: Click to Change the Background! (Basic DOM Manipulation)** 🎨  
📌 **Task:** Create a **button** that changes the **background color** of the page when clicked!  

🔹 **HTML:**  
```html
<button id="colorButton">Change Background Color</button>
```

🔹 **JavaScript:**  
```js
document.getElementById("colorButton").addEventListener("click", function() {
  document.body.style.backgroundColor = "lightblue";
});
```

🎯 **Bonus:** Make the **background color change randomly**!  

---

### **🚀 Challenge 6: Form Validation (Prevent Empty Fields!)** 📄  
📌 **Task:** Create a form where users enter their **favorite book & email**. If they forget to fill it out, show an **error message**!  

🔹 **HTML:**  
```html
<form id="bookForm">
  <input type="text" id="book" placeholder="Favorite Book">
  <input type="email" id="email" placeholder="Email">
  <button type="submit">Submit</button>
  <p id="errorMessage" style="color:red;"></p>
</form>
```

🔹 **JavaScript:**  
```js
document.getElementById("bookForm").addEventListener("submit", function(event) {
  event.preventDefault();
  let book = document.getElementById("book").value;
  let email = document.getElementById("email").value;
  let errorMessage = document.getElementById("errorMessage");

  if (!book || !email) {
    errorMessage.innerText = "Please fill out both fields!";
  } else {
    errorMessage.innerText = "";
    alert("Thank you for sharing your favorite book!");
  }
});
```

🎯 **Bonus:** Add a **character counter** for the book input field!  

---

### **🚀 Challenge 7: The Ultimate To-Do List!** ✅  
📌 **Task:** Build a simple **to-do list** that allows users to **add, complete, and remove tasks**.  

🔹 **HTML:**  
```html
<div>
  <input type="text" id="taskInput" placeholder="Add a task">
  <button id="addTaskButton">Add Task</button>
  <ul id="taskList"></ul>
</div>
```

🔹 **JavaScript:**  
```js
document.getElementById("addTaskButton").addEventListener("click", function() {
  let taskInput = document.getElementById("taskInput");
  let taskList = document.getElementById("taskList");

  if (taskInput.value) {
    let li = document.createElement("li");
    li.innerText = taskInput.value;

    let completeButton = document.createElement("button");
    completeButton.innerText = "Complete";
    completeButton.addEventListener("click", function() {
      li.style.textDecoration = "line-through";
    });

    let removeButton = document.createElement("button");
    removeButton.innerText = "Remove";
    removeButton.addEventListener("click", function() {
      taskList.removeChild(li);
    });

    li.appendChild(completeButton);
    li.appendChild(removeButton);
    taskList.appendChild(li);
    taskInput.value = "";
  }
});
```

🎯 **Bonus:** Add **drag-and-drop** to reorder tasks!  

---

## **🎒 Homework & Next Steps**  
✅ **Complete your JavaScript challenges** and test them in the browser.  
✅ **Explore DevTools (`F12` → Console) and debug your code**.  
✅ **Bring your completed To-Do List app** for a **showcase session** next week!  

📢 **Next Session:** **We’ll combine HTML, CSS & JavaScript to build an interactive website!** 🚀  

🎉 **Keep coding, keep learning, and have fun!** 🚀💻
