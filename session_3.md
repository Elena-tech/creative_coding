# 🎨 **Session 3: Accessible Web Development – Building for Everyone!** 🎨  

🚀 **Mission:** Make the Web a More Inclusive Place!  
💡 **Theme:** Combine **HTML, CSS, and JavaScript** to build **accessible, user-friendly websites**.  

🔹 **Superpowers unlocked today:**  
✅ Using **Accessibility Testing Tools** 🕵️‍♂️  
✅ Writing **Semantic HTML** for better structure 📜  
✅ Improving **Readability & Contrast with CSS** 🎨  
✅ Adding **Dynamic Interactions with JavaScript** ⚡  
✅ Implementing **ARIA Attributes & Form Enhancements** ♿  

---

## **📖 Lesson Breakdown**  

### **👀 Part 1: Why Accessibility Matters?**  
**Accessibility** makes the web usable for **everyone**, including people with disabilities. It’s not just about compliance; it’s about **inclusivity and usability**!  

🎯 **Why should we care?**  
- 1 billion+ people globally have disabilities ♿  
- Improves **SEO & usability** (Google loves accessible sites!)  
- Legal requirements (WCAG, ADA, UK GOV Accessibility Guidelines)  
- A **better experience** for everyone!  

---

## **🛠️ Lab Challenges: Hands-on Accessibility Testing & Fixes!**  

### **🚀 Challenge 1: Using Accessibility Testing Tools** 🕵️‍♂️  
📌 **Task:** Evaluate a real website’s accessibility using Chrome’s **Wave Extension**  

🔹 **Steps:**  
1️⃣ Download **Wave Accessibility Tool** for Chrome: [Get it here](https://wave.webaim.org/extension/)  
2️⃣ Open **a website of your choice** (e.g., BBC, Instagram, a news site)  
3️⃣ Click the **Wave icon** to analyze the page’s **HTML structure & contrast**  
4️⃣ **Assess:**  
   ✅ Does the page use proper **heading tags**?  
   ✅ Is the **contrast high enough** for readability?  
   ✅ Does it have **ARIA labels** and **alt text** for images?  
5️⃣ Write **3-5 key takeaways**:  
   - What **does the site do well**?  
   - What **could be improved**?  
   - What **WCAG rating** does it have?  

🎯 **Bonus:** Use **DevTools (`F12` → Lighthouse)** to run an **Accessibility Audit**!  

---

### **🚀 Challenge 2: Making HTML More Accessible** 📜  
📌 **Task:** **Improve a basic webpage’s accessibility** using proper HTML elements.  

🔹 **Starter Code:**  
Use [this CodePen starter](https://codepen.io/) or create a new **HTML file**.  

#### **2A: Add 'alt' Text for Images** 🖼️  
- Locate the `<img>` tag.  
- Add meaningful **alt text** describing the image.  

#### **2B: Use Semantic HTML** 🏗️  
- Replace `<div>` tags with meaningful elements:  
   ✅ `<header>` for the top section  
   ✅ `<nav>` for menus  
   ✅ `<main>` for content  
   ✅ `<section>` for different parts  
   ✅ `<footer>` for the bottom  

#### **2C: Ensure Logical Headings** 🔠  
- Replace generic `<div>` headings with:  
   ✅ `<h1>` for the main title  
   ✅ `<h2>` for sub-sections  
   ✅ **No skipping levels!** (`h1 → h3` is bad)  

#### **2D: Replace Vague Link Text** 🔗  
❌ Bad: `<a href="about.html">Click here</a>`  
✅ Better: `<a href="about.html">Learn more about our team</a>`  

#### **2E: Add Labels to Forms** ✍️  
- Add `<label>` to form inputs for better usability.  

#### **2F: Implement an ARIA Attribute** ♿  
- Add `aria-label="Submit your form"` to the **Submit button**.  

🎯 **Bonus:** Validate your HTML with the **[W3C HTML Validator](https://validator.w3.org/)**!  

---

### **🚀 Challenge 3: Making CSS More Accessible** 🎨  
📌 **Task:** Improve styles for **better contrast, readability, and focus states.**  

🔹 **Open `styles.css` and modify the following:**  

#### **3A: Improve Contrast & Readability** 🌓  
- Find the `body` selector and:  
   ✅ Increase **text contrast** (dark text on light background or vice versa)  
   ✅ Increase **font size & line spacing** for readability  

#### **3B: Link CSS Styles to HTML**  
- Add **ID & class attributes** in HTML to apply CSS styles correctly.  

#### **3C: Style a New Button**  
- Add a button in HTML (`<button class="styled-button">Click Me</button>`)  
- Create a `.styled-button` style in **CSS** (custom colors, padding, borders).  

#### **3D: Add a Hover Effect** 🎭  
- Use `:hover` to make the button **change color on hover**.  

🎯 **Bonus:** Add **focus states** (`:focus`) for **keyboard users**!  

---

### **🚀 Challenge 4: JavaScript & Accessibility** ⚡  
📌 **Task:** Improve usability with JavaScript!  

#### **4A: Add Elements Dynamically**  
- Create a **button** that, when clicked, **adds a paragraph** dynamically.  

```js
document.getElementById("addText").addEventListener("click", function() {
  let newPara = document.createElement("p");
  newPara.innerText = "This is a new paragraph!";
  document.body.appendChild(newPara);
});
```

#### **4B: Remove Elements** 🗑️  
- Add a **button** that removes the **last paragraph** created.  

```js
document.getElementById("removeText").addEventListener("click", function() {
  let paragraphs = document.querySelectorAll("p");
  if (paragraphs.length > 0) {
    paragraphs[paragraphs.length - 1].remove();
  }
});
```

#### **4C: Toggle Visibility** 👀  
- Add a **"Show/Hide Section"** button.  

```js
document.getElementById("toggleSection").addEventListener("click", function() {
  let section = document.getElementById("hiddenSection");
  if (section.style.display === "none") {
    section.style.display = "block";
    this.innerText = "Hide Section";
  } else {
    section.style.display = "none";
    this.innerText = "Show Section";
  }
});
```

#### **4D: Change Heading Text on Click** 🔠  
```js
document.getElementById("changeHeading").addEventListener("click", function() {
  document.getElementById("mainHeading").innerText = "Accessibility is Awesome!";
});
```

#### **4E: Change Background Color Dynamically** 🎨  
```js
document.getElementById("changeColor").addEventListener("click", function() {
  document.body.style.backgroundColor = "#f0db4f"; // Yellow
});
```

#### **4F: Form Validation** ✅  
```js
document.getElementById("form").addEventListener("submit", function(event) {
  event.preventDefault();
  let input = document.getElementById("name").value;
  if (!input) {
    alert("Please enter your name!");
  } else {
    alert("Thanks, " + input + "!");
  }
});
```

🎯 **Bonus:** Add an **ARIA live region** to notify screen reader users of form errors!  

---

### **🚀 Optional Challenge: Peckham Bakery Menu Generator** 🍞🥐  
📌 **Task:** Use **arrays & loops** to create a **menu list dynamically.**  

```js
let menuItems = ["Croissant", "Baguette", "Pain au Chocolat", "Sourdough"];
let menuContainer = document.getElementById("menu");

menuItems.forEach(item => {
  let div = document.createElement("div");
  div.innerHTML = `<h3>${item}</h3><p>A delicious ${item} fresh from the oven!</p>`;
  menuContainer.appendChild(div);
});
```

---

## **🎒 Homework & Next Steps**  
✅ **Finish your accessibility fixes & test with Lighthouse**  
✅ **Bring a completed accessible webpage next week**  
✅ **Test your website using a screen reader (ChromeVox, NVDA, or VoiceOver)**  

📢 **Next Session:** **Full Project – Create a fully accessible interactive website!** 🚀  

🎉 **Keep coding, keep learning, and build for everyone!** ♿💻🚀
