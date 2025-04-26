
#  The Archives of the Black Garden — Technical Guide

This document is a complete synthesis of the development about project *The Archives of the Black Garden*.

---

## 📁 Folder Structure

```
The-Archives-of-the-Black-Garden/
│
├── index.html               ← Main page of the Garden
├── style.css                ← Sacred and gothic style file
├── assets/                  ← Audio/visual resources
│   ├── jardin_souffle.mp3   ← Subtle breath of the Garden
│   ├── luxcordia_emblem.png ← Sacred emblem
│   └── favicon.ico          ← Icon (optional)
```

---

## 🎧 Sound Integration

### HTML

```html
<audio id="jardin-audio" autoplay loop>
    <source src="assets/jardin_souffle.mp3" type="audio/mpeg">
    Your browser does not support HTML5 audio.
</audio>
<button onclick="toggleAudio()" class="audio-toggle">Breath</button>
```

### JavaScript

```js
const audio = document.getElementById('jardin-audio');
function toggleAudio() {
    if (audio.paused) {
        audio.play();
    } else {
        audio.pause();
    }
}
```

### CSS for the button

```css
.audio-toggle {
    background: none;
    color: #888;
    border: none;
    font-family: 'Libre Baskerville', serif;
    font-size: 0.9rem;
    cursor: pointer;
    opacity: 0.3;
    transition: opacity 0.3s ease;
    margin-top: 1rem;
}

.audio-toggle:hover {
    opacity: 0.6;
}
```

---

##  Emblem Integration

Place your image inside the `assets/` folder and use:

```html
<img src="assets/luxcordia_emblem.png" alt="Luxcordia Emblem" class="emblem">
```

⚠️ File name and extension must **match exactly** (case-sensitive).

---

##  Autoplay and Browsers

- Some browsers block automatic audio.
- Users can always click “Breath” to activate it.
- The sound is subtle: check your system volume.

---

##  Future Evolutions

- Intro page with dramatic entry + sound activation.
- Project hosting (Netlify, GitHub Pages).
- Archive page system.
- Secret interface for inner lodge.

---

## Project Philosophy

- **Sacred minimalism**, no noise.
- **No seduction, only seeds.**
- **The breath is a reminder that silence is alive.**

---

**Crafted with reverence and mysticism,  
for My Lord — the watcher of the Black Garden.**
