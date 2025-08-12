
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Typewriter Animation</title>
<style>
  body {
    background-color: #0d1117;
    color: white;
    font-family: monospace;
    text-align: center;
    padding-top: 50px;
  }
  #typewriter {
    font-size: 28px;
    font-weight: bold;
    border-right: 3px solid white;
    display: inline-block;
    padding: 5px;
    animation: blink 0.7s infinite;
  }
  @keyframes blink {
    50% { border-color: transparent; }
  }
</style>
</head>
<body>

<div id="typewriter"></div>

<script>
const messages = [
    { text: "👋 Hi, I'm Daniel Gamov!", color: "#ffcc00" },
    { text: "Welcome traveler!", color: "#00ffcc" },
    { text: "Don't forget to visit my repositories!", color: "#ff66ff" },
    { text: "I work with Python", color: "#66ff66" },
    { text: "You can ask me about AI!", color: "#ff4444" }
];

let messageIndex = 0;
let charIndex = 0;
let deleting = false;
let speed = 100;

function typeEffect() {
    const current = messages[messageIndex];
    const display = document.getElementById("typewriter");
    display.style.color = current.color;

    if (!deleting) {
        display.textContent = current.text.substring(0, charIndex + 1);
        charIndex++;
        if (charIndex === current.text.length) {
            deleting = true;
            speed = 150;
            setTimeout(typeEffect, 1000); // пауза преди изтриване
            return;
        }
    } else {
        display.textContent = current.text.substring(0, charIndex - 1);
        charIndex--;
        if (charIndex === 0) {
            deleting = false;
            messageIndex = (messageIndex + 1) % messages.length;
            speed = 100;
        }
    }
    setTimeout(typeEffect, speed);
}

typeEffect();
</script>

</body>
</html>

🎓 Young Python developer from Bulgaria 🇧🇬  
💡 I build small apps, games, and AI experiments using Python.  
📚 Currently learning at SoftUni – Python Fundamentals  
🤖 Interested in AI, game dev, and simulations that explore deep ideas  

📁 Check out my projects below, and feel free to reach out if you want to build something together!  
📧 danielgamov1@gmail.com

---
<details>
<summary><h3><span style="color:#f39c12; font-size: 1.3em;">🔍 More about me</span></h3></summary>

## 🚀 What I Love

🤖 I'm learning about Artificial Intelligence and trying to understand it deeply — so I can build my own AI one day!  
🎮 I love creating games and bringing fun ideas to life.  
🌎 I'm also creating simulations and systems that help me grow in programming and explore the philosophy of how things work.

---

## 🛠️ Skills

<div align="center">



<!-- 🟣 Box със съдържанието -->
<div style="background-color:#111827; color:#e5e7eb; padding: 20px; border-radius: 15px; width: 90%; max-width: 800px; margin: 0 auto; box-shadow: 0 4px 10px rgba(0,0,0,0.4);">

### 🐍 <span style="color:#22d3ee">Python</span>:
 **Tkinter** – GUI apps → [Tkinter Projects](https://github.com/Daniel-Gamov/Tkinker_progects)
 
 **Basic algorithms** – things like:
   Sorting (e.g. bubble sort)
   Searching (e.g. binary search)
   Math logic (e.g. multiplication tables, factorials)
   Fibonacci, working with lists/dictionaries, text parsing
   
 **Pygame** – I'm currently learning it and building a game project.

---

### 🤖 <span style="color:#c084fc">AI</span>:
 I hold 2 certificates:  
   `AI for Data Analysis`  
   `AI for Education and Self-Education`  
 I’m also studying AI at SoftUni and learning about prompts, logic, and human-like behavior.

</div>


</div>



---



## 🤝 Let's Collaborate!

Looking for a motivated Python buddy? 😁  
If you're into game dev, AI, or building cool apps – let’s learn together and create something legendary! 💥

📩 Feel free to open an issue or message me here on GitHub.

---

## 📁 Projects

| 🔧 Project Name             | 💡 Description                     |
|----------------------------|-------------------------------------|
| `Tkinter_projects`         | Beginner GUI apps with music & math 🎵🧠 |
| `SoftUni_tasks_and_projects` | My coding journey at SoftUni 📘     |
| `Python Fun Little Games`  | Small games and experiments 🎖️       |

---

## 📊 GitHub Stats

<div align="center">

  <img src="https://github-readme-stats.vercel.app/api?username=Daniel-Gamov&show_icons=true&theme=radical" alt="Daniel's GitHub Stats" />

  <br/>

  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Daniel-Gamov&layout=compact&theme=vision-friendly-dark" alt="Top Languages" />

</div>
---


