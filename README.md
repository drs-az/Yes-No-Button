# Yes / No Button Toy (Bluey Dance Mode Inspired)

A simple web toy that recreates the **Yes / No button** from Bluey’s *Dance Mode* episode.  
Click or tap the green or red circles on the toy image, and it will play voice clips saying **“Yes!”** or **“No!”**.  
Press **Yes three times in a row** to unlock **Dance Mode**! 🎉

---

## 🎮 Features
- Clickable **Yes** and **No** buttons mapped onto your toy image.
- Plays `yes.mp3` and `no.mp3` voice clips (overlapping playback supported).
- Fun animations: bounce on **Yes**, waggle on **No**.
- **Easter Egg: Dance Mode** → triggered by pressing Yes three times in a row.
- Dance Mode plays `dance mode.mp3`, shows a special **“DANCE MODE!”** message, and animates the toy with a bounce effect.
- Mobile-friendly with vibration feedback (on supported devices).
- Keyboard shortcuts: press **Y** or **N**.

---

## 📂 Files Needed
Place these files together in the same folder:
- `index.html` → main webpage
- `toy.jpg` → the image of your toy (update filename if different)
- `yes.mp3` / `yes.ogg` → audio clip for Yes
- `no.mp3` / `no.ogg` → audio clip for No
- `dance mode.mp3` → audio clip for Dance Mode Easter Egg
- `README.md` → this file

---

## 🚀 Usage
1. Open `index.html` in any modern browser.
2. Click/tap the green or red circle to hear “Yes” or “No.”
3. Try pressing the **Y** or **N** keys on your keyboard.
4. Press **Yes three times in a row** to trigger Dance Mode!

---

## ⚙️ Customization

### Button Placement
Hotspots are positioned with percentage values relative to the toy image:
```css
.hotspot.yes { top:12%; }
.hotspot.no  { top:30%; }
```

- **Lower the %** to move a button **higher** on the image.
- **Raise the %** to move a button **lower**.
- Adjust `width:40%` to make the clickable area bigger or smaller.

### Debug Mode
To see the clickable circles while adjusting, add this CSS:
```css
.hotspot {
  border: 2px dashed rgba(0,0,0,.4); /* temporary debug outline */
}
```

### Audio
Replace `yes.mp3`, `no.mp3`, and `dance mode.mp3` with your own voice clips or sounds.  
You can add `.ogg` versions for wider browser compatibility.

---

## 📱 Mobile Notes
- Works on iOS and Android browsers.
- Vibrates on press if the device supports the Vibration API.
- On some mobile browsers, the first tap may be required to “unlock” audio playback.

---

## 🕹️ Bonus Ideas
- Add visual effects (confetti, lights) during Dance Mode.
- Randomize voice clips by loading multiple versions for variety.
- Add styling (glow, light-up effects) when pressing a button.

---

## 📜 License
Free to use and modify for fun projects. Attribution to *Bluey* creators (Ludo Studio / BBC Studios) -- much ❤️.
