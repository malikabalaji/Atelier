<div align="center">

# 🪡 Atelier

### *yours, restyled.*

**You own more outfits than you think. Atelier finds them.**

Photograph your clothes. Pick one piece you love. Watch a styling engine build complete looks from your own closet, in seconds, entirely in your browser.

![HTML](https://img.shields.io/badge/pure-HTML%20%2B%20vanilla%20JS-E34F26?style=flat-square&logo=html5&logoColor=white)
![Zero Dependencies](https://img.shields.io/badge/dependencies-zero-8B7355?style=flat-square)
![One File](https://img.shields.io/badge/entire%20app-one%20file-1C1A17?style=flat-square)
![Privacy](https://img.shields.io/badge/your%20data-never%20leaves%20your%20device-2E7D32?style=flat-square)

</div>

---

## The problem

Everyone has a closet full of clothes and the daily feeling of *"I have nothing to wear."* The truth is you have plenty. You just can't see the combinations.

## The idea

Atelier is a personal wardrobe studio that fits in a single HTML file:

📸 **Snap it.** Upload photos or use your camera, right in the browser. Atelier reads each garment's colour palette automatically and flags whether it's a quiet neutral or a statement piece.

🏷️ **Tag it.** One tap to confirm the category and formality. The app even guesses the category for you from the photo's shape.

✨ **Style it.** Choose any piece as your anchor. The engine composes up to four complete outfits around it, balancing colour, matching formality, and making sure only one statement piece speaks at a time.

Each look arrives with a name (*The Mainstay*, *Off-Duty*, *After Hours*), a match score, and a plain-English explanation of why it works.

## Why it's interesting under the hood

This is not a wrapper around an API. Everything runs client-side:

| What | How |
|---|---|
| 🎨 Colour intelligence | Canvas pixel sampling extracts the dominant palette, tone, and saturation of every garment |
| 🧠 Category guessing | Lightweight heuristics infer the garment type before you even tap |
| ⚖️ Outfit scoring | Every candidate piece is scored on formality distance, statement balance, neutral bonuses, and tonal harmony |
| 📷 Live camera | MediaDevices API with square crop and shutter flash, built into the page |
| 🔒 Total privacy | localStorage only. No accounts, no servers, no tracking. Close the tab and your closet is still there. Only for you. |

All of it in **~900 lines of hand-written HTML, CSS, and JavaScript**. No framework. No build step. Nothing to install.

## Try it in 10 seconds

```bash
git clone https://github.com/malikabalaji/Atelier.git
cd Atelier
open atelier-outfit-builder.html
```

That's it. For camera capture, serve it locally:

```bash
python3 -m http.server 8000
# visit http://localhost:8000/atelier-outfit-builder.html
```

## Designed like a fashion product, not a to-do app

Editorial serif typography, a warm gallery-white canvas, soft motion, and copy that sounds like a stylist rather than a settings menu. Because if an app is about looking good, it should look good.

---

<div align="center">

*An empty rail is just a beginning.*

**⭐ Star this repo if you'd wear it.**

</div>
