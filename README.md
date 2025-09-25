<!-- ============================= -->
<!--       1. BANNER SECTION       -->
<!-- ============================= -->

![Banner](https://github.com/NDCSwift/Swift-Projects/blob/main/Screenshot%202025-09-25%20at%201.06.36%E2%80%AFPM.png?raw=true)

---

<!-- ============================= -->
<!--       2. INTRODUCTION         -->
<!-- ============================= -->

# 👋 Hi, I'm Noah Carpenter  
**Dream Big, Code Bigger — Building intuitive apps with Swift, SwiftUI, and Xcode.**

---

<!-- ============================= -->
<!--          3. ABOUT ME          -->
<!-- ============================= -->

## ✨ About Me  
Hello! I’m Noah Carpenter, an iOS developer and designer passionate about creating **engaging, intuitive, and polished mobile apps**.  
I love turning ideas into real, functional experiences that uplift, educate, and entertain.  
My work blends **clean design**, **robust engineering**, and a focus on **user delight**.  
I believe in coding as a craft and enjoy sharing my knowledge through teaching and YouTube tutorials.  

---

<!-- ============================= -->
<!--        4. MY PROJECTS         -->
<!-- ============================= -->

## 🚀 My Projects  

- **[WordSage](https://apps.apple.com/ca/app/wordsage/id6683296823)**  
  _Your daily vocabulary challenge with interactive games and motion-based controls._  
  🔗 [Live on App Store](https://apps.apple.com/ca/app/wordsage/id6683296823) • 💻 [GitHub Repo (Coming Soon)](#)

- **[Daily Devotion](https://apps.apple.com/ca/app/daily-devotions/id6744182819)**  
  _Beautifully curated scripture and reflections to inspire each day._  
  🔗 [Live on App Store](https://apps.apple.com/ca/app/daily-devotions/id6744182819) • 💻 [GitHub Repo (Coming Soon)](#)

- **[Tap Duel](https://apps.apple.com/us/app/tap-duel/id6746076055)**  
  _Face-to-face or online reflex battles with multiplayer support and custom visuals._  
  🔗 [Live on App Store](https://apps.apple.com/us/app/tap-duel/id6746076055) • 💻 [GitHub Repo (Coming Soon)](#)

---

<!-- ============================= -->
<!--       5. CONNECT WITH ME      -->
<!-- ============================= -->

## 🤝 Connect with Me  

[![YouTube](https://img.shields.io/badge/YouTube-FF0000?logo=youtube&logoColor=white)](https://www.youtube.com/@NoahDoesCoding97)  

---

<!-- ============================= -->
<!--        6. GITHUB STATS        -->
<!-- ============================= -->

## 📊 GitHub Stats  

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=EcatSenpai&show_icons=true&theme=tokyonight)

---

<!-- ============================= -->
<!--      7. YOUTUBE LATEST        -->
<!-- ============================= -->

## 🎬 Latest YouTube Videos  

<!-- 
This script fetches the latest uploads from your YouTube channel without using an API key. 
It works by embedding your channel’s RSS feed and parsing it with JS.
Note: Works best on GitHub Pages / personal site, GitHub README doesn’t execute JS — 
so provide a fallback (links) for README itself. 
-->

<!-- Fallback Links for README -->
- [Visit my YouTube Channel](https://www.youtube.com/@NoahDoesCoding97) for the latest videos!  



<div id="youtube-videos"></div>
<script>
  fetch("https://www.youtube.com/feeds/videos.xml?channel_id=UC0DtrK_aph5EzH_iC-9qYjg") 
    .then(res => res.text())
    .then(str => new window.DOMParser().parseFromString(str, "text/xml"))
    .then(data => {
      let container = document.getElementById("youtube-videos");
      let items = data.querySelectorAll("entry");
      items.forEach((el, i) => {
        if (i < 3) {
          let title = el.querySelector("title").textContent;
          let link = el.querySelector("link").getAttribute("href");
          let div = document.createElement("div");
          div.innerHTML = `<a href="${link}" target="_blank">🎥 ${title}</a>`;
          container.appendChild(div);
        }
      });
    });
</script>

