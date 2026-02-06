# MMAC Card WebAR Demo (Browser-based)

This is a **browser-only** AR demo that mimics your "App Clip style" flow:
- Open link -> camera opens
- When the card is detected -> floating panel appears
- Buttons: Call + WhatsApp

## The one thing you must generate: targets.mind
MindAR image tracking needs a `.mind` file built from your marker image.

Use the official MindAR compiler tool:
https://hiukim.github.io/mind-ar-js-doc/tools/compile/

Steps:
1) Open the compiler page
2) Upload your **back-side card image** (use the best, sharpest image)
3) Click Start
4) Download the output file (usually `targets.mind`)
5) Rename it to `targets.mind` (if needed) and replace the file in this folder.

## Hosting (IMPORTANT)
Camera access requires HTTPS.
Easiest:
- Put this folder on GitHub
- Enable GitHub Pages
- Open the Pages URL on iPhone Safari

Local testing:
- Use VS Code "Live Server" + HTTPS OR any local https server.

## Customize
Open `index.html` and change:
- PHONE_E164 = "+97156xxxxxxx"
