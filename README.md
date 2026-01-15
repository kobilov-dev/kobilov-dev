<div align="center">
  <img height="200" src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif" />
</div>

<h2 align="center" style="color:#ff8c00;">Frontend Development • Clean Code • Modern UI</h2>

---

## 👋 Hi, I'm Shokirjon (kobilov-dev)

I'm a **Frontend Developer** focused on building modern, clean, and user-friendly interfaces.  
I enjoy turning ideas into **interactive web experiences** and continuously improving my skills.

---

## 🎯 Current Focus
- Frontend Development
- Clean & structured code
- UI implementation and responsiveness
- Working with modern frameworks and tools

---

## 🛠️ Tech Stack

<div align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" height="40" />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" height="40" />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/sass/sass-original.svg" height="40" />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="40" />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" height="40" />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/angular/angular-original.svg" height="40" />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" height="40" />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/androidstudio/androidstudio-original.svg" height="40" />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" height="40" />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" height="40" />
</div>

---

## 🚀 Featured Projects
Here you’ll find:
- Frontend projects and UI implementations  
- Practice projects and experiments  
- Clean and structured repositories  

---

## 🎮 Mini Project – Color Click Game

Below is a **simple interactive browser game** showcasing frontend skills: HTML, SCSS/CSS, and JavaScript.  
Click the correct color before the timer runs out and score points!

<div align="center">

```html
<style>
#game-container { text-align:center; margin:20px auto; }
.color-box { width:100px; height:100px; display:inline-block; margin:10px; cursor:pointer; border-radius:8px; transition: transform 0.1s; }
.color-box:hover { transform: scale(1.1); }
#score { font-size: 18px; margin-top: 10px; }
</style>

<div id="game-container">
  <div id="box1" class="color-box"></div>
  <div id="box2" class="color-box"></div>
  <div id="box3" class="color-box"></div>
  <p id="score">Score: 0</p>
</div>

<script>
const boxes = [document.getElementById('box1'), document.getElementById('box2'), document.getElementById('box3')];
let correctIndex = 0;
let score = 0;

function randomColor() {
  return '#' + Math.floor(Math.random()*16777215).toString(16);
}

function setColors() {
  correctIndex = Math.floor(Math.random()*boxes.length);
  boxes.forEach((box, i) => box.style.background = randomColor());
  boxes[correctIndex].style.background = 'orange';
}

boxes.forEach((box, i) => box.addEventListener('click', () => {
  if(i===correctIndex) { score++; } else { score--; }
  document.getElementById('score').innerText = 'Score: ' + score;
  setColors();
}));

setColors();
</script>




