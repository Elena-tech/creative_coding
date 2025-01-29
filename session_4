# 🎭 **Session 4: Exploring Accessibility & Customization in Web Development** 🎭  

🚀 **Mission:** Bring It All Together – Create a Fully Accessible & Customizable Website!  
💡 **Theme:** **Enhance interactivity, personalize user experience, and ensure full accessibility compliance**.  

🔹 **Superpowers unlocked today:**  
✅ Adding **More Interactivity with JavaScript** ⚡  
✅ Customizing Websites for Different Users 🌍  
✅ Ensuring **WCAG Compliance & Best Practices** ♿  
✅ Using **Web Development Platforms (WordPress, Wix, Webflow, GitHub Pages)**  

---

## **📖 Lesson Breakdown**  

### **👀 Part 1: Why Customization Matters in Web Accessibility?**  
Not all users experience the web the same way! Customization allows users to **adapt a site to their needs** and provides:  
✅ **Better readability** (dark mode, larger text)  
✅ **Simplified navigation** (keyboard shortcuts, voice commands)  
✅ **Alternative input options** (screen readers, speech-to-text)  

---

## **🛠️ Lab Challenges: Make Websites More Interactive & Accessible!**  

### **🚀 Challenge 1: Add a Dark Mode Toggle 🌙**  
📌 **Task:** Create a **Dark Mode button** that switches between light and dark themes.  

🔹 **HTML:**  
```html
<button id="darkModeToggle">Enable Dark Mode</button>
```

🔹 **CSS:**  
```css
.dark-mode {
  background-color: #121212;
  color: white;
}
```

🔹 **JavaScript:**  
```js
document.getElementById("darkModeToggle").addEventListener("click", function() {
  document.body.classList.toggle("dark-mode");
  this.innerText = document.body.classList.contains("dark-mode") ? "Disable Dark Mode" : "Enable Dark Mode";
});
```

🎯 **Bonus:** Save the **user’s preference** using `localStorage`!  

---

### **🚀 Challenge 2: Create a Customizable Font Size Tool 🔤**  
📌 **Task:** Add a feature that **lets users adjust font size** for readability.  

🔹 **HTML:**  
```html
<label for="fontSize">Adjust Font Size:</label>
<input type="range" id="fontSize" min="12" max="32" value="16">
```

🔹 **JavaScript:**  
```js
document.getElementById("fontSize").addEventListener("input", function() {
  document.body.style.fontSize = this.value + "px";
});
```

🎯 **Bonus:** Allow users to **choose their own font** (e.g., dyslexia-friendly fonts).  

---

### **🚀 Challenge 3: Build an Accessible Navigation Menu** 🎯  
📌 **Task:** Design a **keyboard-accessible navigation bar**.  

🔹 **HTML:**  
```html
<nav>
  <ul id="menu">
    <li><a href="#">Home</a></li>
    <li><a href="#">About</a></li>
    <li><a href="#">Contact</a></li>
  </ul>
</nav>
```

🔹 **CSS (for better focus visibility):**  
```css
nav a:focus {
  outline: 3px solid yellow;
}
```

🔹 **JavaScript (Enable Keyboard Navigation):**  
```js
document.addEventListener("keydown", function(event) {
  if (event.key === "Tab") {
    document.activeElement.style.outline = "3px solid yellow";
  }
});
```

🎯 **Bonus:** Use `aria-expanded` attributes to make the menu **screen reader-friendly**!  

---

### **🚀 Challenge 4: Add Text-to-Speech for Better Accessibility** 🎤  
📌 **Task:** Implement **text-to-speech** so users can have text read aloud.  

🔹 **HTML:**  
```html
<p id="text">Web accessibility helps make the internet a more inclusive place.</p>
<button id="speakButton">Read Aloud</button>
```

🔹 **JavaScript:**  
```js
document.getElementById("speakButton").addEventListener("click", function() {
  let msg = new SpeechSynthesisUtterance(document.getElementById("text").innerText);
  window.speechSynthesis.speak(msg);
});
```

🎯 **Bonus:** Allow users to **choose different voices & speeds**!  

---

### **🚀 Challenge 5: Implement Form Validation with Live Error Messaging** 📑  
📌 **Task:** Prevent errors in forms and provide **real-time feedback**.  

🔹 **HTML:**  
```html
<form id="contactForm">
  <input type="text" id="name" placeholder="Your Name">
  <span id="nameError" class="error"></span>
  <button type="submit">Submit</button>
</form>
```

🔹 **JavaScript:**  
```js
document.getElementById("contactForm").addEventListener("submit", function(event) {
  let nameInput = document.getElementById("name");
  let errorMessage = document.getElementById("nameError");

  if (!nameInput.value.trim()) {
    event.preventDefault();
    errorMessage.innerText = "Please enter your name!";
  } else {
    errorMessage.innerText = "";
  }
});
```

🎯 **Bonus:** Use `aria-live="polite"` to make error messages accessible for **screen readers**.  

---

### **🚀 Challenge 6: Create a Personalized User Dashboard** 🏆  
📌 **Task:** Store **user preferences (theme, font, name)** and **display them on login**.  

🔹 **HTML:**  
```html
<input type="text" id="username" placeholder="Enter your name">
<button id="saveUser">Save</button>
<p id="welcomeMessage"></p>
```

🔹 **JavaScript:**  
```js
document.getElementById("saveUser").addEventListener("click", function() {
  let name = document.getElementById("username").value;
  localStorage.setItem("userName", name);
  document.getElementById("welcomeMessage").innerText = "Welcome, " + name + "!";
});

window.onload = function() {
  let savedName = localStorage.getItem("userName");
  if (savedName) {
    document.getElementById("welcomeMessage").innerText = "Welcome back, " + savedName + "!";
  }
};
```

🎯 **Bonus:** Add a **"Reset Preferences"** button to clear settings.  

---

## **💻 Exploring Website Building Platforms** 🌍  
🎯 **Task:** Research and explore different **website platforms**:  

🔹 **WordPress** – Customizable with plugins & themes.  
🔹 **Wix / Webflow** – Drag-and-drop builders.  
🔹 **GitHub Pages** – Free hosting for developers.  
🔹 **Squarespace** – Great for design-heavy sites.  

🎯 **Challenge:**  
- **Compare features** (Customization, Accessibility Tools, Cost, Ease of Use).  
- Try **building a quick landing page** using one of these platforms.  

---

## **🎒 Final Homework: Build Your Fully Accessible Website!**  
📌 **Task:** Apply **everything from the past 4 weeks** and create a **fully accessible, interactive, and customized website**!  

🎯 **Checklist for Your Final Website:**  
✅ **Accessible HTML** (semantic tags, headings, alt text)  
✅ **Keyboard-friendly navigation** (tab order, focus states)  
✅ **Readable design** (high contrast, adjustable font sizes)  
✅ **JavaScript interactivity** (dark mode, custom settings, text-to-speech)  
✅ **Form validation & error handling**  
✅ **Tested with accessibility tools (WAVE, Lighthouse, Screen Readers)**  

---

## **🎉 Final Challenge: Website Showcase & Accessibility Review!** 🎉  
🎯 **Task:** Present your website to the class & test each other’s sites for accessibility.  

🔹 **Feedback Criteria:**  
✅ Is it **fully navigable with a keyboard?**  
✅ Does it have **high contrast & readable text?**  
✅ Are **interactive features accessible?**  
✅ Did it pass **Lighthouse accessibility audits?**  

🏆 **Top 3 websites with the best accessibility features will win a prize!** 🎁  

---

## **🎓 Course Wrap-Up: What’s Next?**  
- Keep refining your **accessible design & development skills**.  
- Explore **more accessibility testing tools** (NVDA, Axe, VoiceOver).  
- Consider **certification in accessibility & inclusive design**.  

🚀 **Keep coding & making the web a better place for everyone!** 🌍♿🎉  
