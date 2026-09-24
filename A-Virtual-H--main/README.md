<div align="center">

# 🫂 Virtual Hug Card & Love Receipt Generator

<p align="center">
  <strong>An interactive, romantic, and playful web experience crafted for Hug Day, Valentine's, or any day to remind someone special that they are loved.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Mobile%20Responsive-2ed573?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Responsive" />
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" alt="License" />
</p>

<p align="center">
  <a href="#-features">Features</a> •
  <a href="#-quick-start">Quick Start</a> •
  <a href="#-url-personalization">Personalization</a> •
  <a href="#-project-structure">Project Structure</a> •
  <a href="#-tech-stack">Tech Stack</a> •
  <a href="#-author--credits">Author</a>
</p>

---

</div>

## 📖 Overview

The **Virtual Hug Card** is an interactive web experience that blends playful storytelling, dynamic audio, 3D micro-interactions, and a custom **on-screen Love Receipt generator**.

Users are greeted with a sweet request for a hug. If they attempt to decline, the "No" button playfully evades the cursor on desktop or triggers humorous pleading sequences. Once accepted, romantic music cues in, taking the user through a sensory **Hug Meter** squeeze interaction, confetti celebration, and an authentic **Thermal Love Receipt** certifying proof of unlimited affection.

---

## ✨ Features

### 🌹 Romantic Atmosphere & Design
* **Rose-Blush Velvet Palette:** Dreamy gradient background with a smooth 10s color cycle animation.
* **3D Glassmorphism Card Tilt:** Dynamic card tilt physics tracking cursor movement on desktop.
* **Curated Love Quotes Carousel:** Continuously cycles through heartfelt romantic quotes with smooth fade transitions.
* **Particle System & Emoji Cursor:** Drifting red roses, pink hearts, and sparkles with a playful cursor emoji trail.

### 🏃 Playful Interactive Storyline
* **Runaway "No" Button:** Detects fine-pointer devices and physically dodges cursor clicks.
* **Pleading Screens:** If clicked on touch devices, cascades into cute reaction screens (*"But... why? 😭"* & *"Pretty please? 🥺"*).
* **Mood-Adaptive Audio Engine:** Automatically triggers sad/funny audio (`song1.mp3`) on rejection and transitions to romantic music (`song2.mp3`) on acceptance.

### 💓 Sensory "Hug Meter"
* **Hold-to-Squeeze Interaction:** Simulates a real hug squeeze—the longer you hold, the tighter the embrace.
* **Dynamic Feedback:** Real-time progress updates (*"Squeezing... 🐻"*, *"Tighter... ❤️"*, *"Almost there... ✨"*).
* **Confetti & Haptic Feedback:** Triggers a 150-piece particle confetti explosion and mobile vibration (`navigator.vibrate`) upon completion.

### 🧾 On-Screen "Love Receipt" Generator
* **Authentic Thermal Receipt Aesthetic:** Features realistic sawtooth paper edge cuts (`clip-path`), monospaced typography (*Space Mono*), and a virtual printer slot animation.
* **Itemized Proof of Love:** Line items including *Extra Tight Warm Hug*, *Forehead & Cheek Kisses (Qty: ∞)*, *Late-Night Soft Cuddles*, and *Undivided Love & Devotion*.
* **Romantic Pricing:** 100% Lover VIP Discount, Total: `FREE FOREVER ❤️`.
* **Stylized Barcode & Legal Notice:** Authentic barcode graphic with code `I-L-O-V-E-Y-O-U-24/7` and a playful return policy.

### 💌 Instant URL Personalization
Customize recipient and sender names directly via URL parameters without modifying code:
```text
index.html?to=YourLove&from=Hxni
```

### ⚡ Offline-Ready & Reliable
* **Local Media Assets:** All 6 animation GIFs are stored locally within the project directory to prevent hotlinking bans, Cloudflare blocks, or broken external CDN links.

---

## 📂 Project Structure

```text
Virtual-Hug-Card/
│
├── index.html        # Main application (HTML, CSS styles, animations & scripts)
├── hug-ask.gif       # Ask hug animated illustration
├── cry.gif           # Crying rejection GIF
├── please.gif        # Pretty please reaction GIF
├── loading.gif       # Warmth calibration GIF
├── wait.gif          # Hug meter waiting GIF
├── hug-final.gif     # Final celebration hug GIF
├── song1.mp3         # Rejection audio track
├── song2.mp3         # Acceptance / romantic audio track
└── README.md         # Documentation
```

---

## 🚀 Quick Start

### 1. Clone or Download the Repository
```bash
git clone https://github.com/Hxni786/Virtual-Hug-Card.git
cd Virtual-Hug-Card
```

### 2. Run in Browser
No build tools, bundlers, or servers are required! Simply double-click `index.html` or open it with your favorite browser:
```bash
# On Windows (PowerShell)
Start-Process index.html

# Or with VS Code Live Server extension
```

---

## 🔗 URL Personalization

You can personalize the card when sending it to someone special by adding query parameters to the URL:

| Parameter | Description | Default Value | Example |
| :--- | :--- | :--- | :--- |
| `to` or `name` | Recipient name on the Love Receipt | `My Favorite Person` | `?to=Angel` |
| `from` | Sender name on the Love Receipt & Cashier | `Hxni ❤️` | `?from=Hxni` |

#### Example Shareable Link:
```text
https://your-domain.com/?to=Sweetheart&from=Hxni
```

---

## 🛠️ Customization Guide

* **Custom Audio:** Replace `song1.mp3` and `song2.mp3` with your favorite tracks (ensure filenames match or update paths in `index.html`).
* **Love Quotes:** Edit the `quotes` array in the `<script>` section of `index.html` to add your own personal notes or memories.
* **Color Palette:** Modify the CSS variables inside `:root` to customize the primary tones:
  ```css
  :root {
    --primary: #ff6b8b;       /* Main accent button color */
    --primary-dark: #d63061;  /* Heading and deep tone */
    --accent: #e84393;        /* Secondary highlight */
    --bg-gradient: ...;       /* Animated background gradient */
  }
  ```

---

## 🧰 Tech Stack

* **Markup:** Semantic [HTML5](https://developer.mozilla.org/en-US/docs/Web/HTML)
* **Styling:** Modern [CSS3](https://developer.mozilla.org/en-US/docs/Web/CSS) (Flexbox, CSS Variables, 3D Transforms, Clip-Path, Keyframe Animations)
* **Fonts:** [Google Fonts](https://fonts.google.com/) (*Fredoka*, *Quicksand*, *Space Mono*)
* **Icons:** [Font Awesome 6](https://fontawesome.com/)
* **Logic:** Vanilla JavaScript (ES6+, Canvas 2D API, Web Vibration API, Audio Element API)

---

## 🤝 Contributing

Contributions, feature ideas, and forks are welcome! Feel free to:
1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/RomanticFeature`)
3. Commit your Changes (`git commit -m 'Add some RomanticFeature'`)
4. Push to the Branch (`git push origin feature/RomanticFeature`)
5. Open a Pull Request

---

## 👨‍💻 Author & Credits

**Hxni**

<p align="left">
  <a href="https://www.instagram.com/the.cipher.stack/" target="_blank">
    <img src="https://img.shields.io/badge/Instagram-@the.cipher.stack-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram" />
  </a>
  <a href="https://github.com/Hxni786" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-Hxni786-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
</p>

---

<div align="center">
  <sub>Made with ❤️ for someone special. If you liked this project, don't forget to give it a ⭐!</sub>
</div>
