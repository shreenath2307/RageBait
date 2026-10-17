# The World's Worst Profile Page

## Features

- **Inverted cursor**: Move the mouse left and the cursor goes right. Clicks land where the fake cursor is, not where your real mouse is. This stays on for the whole site.
- **Neon green login page**: A dark terminal-style screen with neon green text.
- **Name rejection**: Type your name (at least 5 letters) and press Enter. The page says *"Ew. Not that name please. That's my ex's name. Enter another name."*
- **Banned keyboard**: For the second name your real keyboard stops working. You have to type **habibi** on an on-screen keyboard.
- **Scrambled virtual keyboard**: The letters are shuffled, and so are backspace and enter. Combined with the inverted cursor, this is where the pain is.
- **Fake loading screen**: Counts down from 1,00,000 with a progress bar that barely moves. Scrolling is locked.
- **The insult**: After 10 seconds the page says *"How long are you gonna wait, IDIOT. JUST SCROLL DOWN."*
- **The screech**: When you scroll down, a loud screeching noise starts. The browser generates it, so there's no audio file.
- **Maths to make it stop**: A shaking pop-up asks for **HCF(a, b) × LCM(a, b)**. The noise only stops when you get it right. Each wrong answer makes it louder and higher.
- **Pastel profile page**: The reward at the end shows Habibi's profile, with your first name crossed out as "formerly ___".

---

## How to run

1. Put `index.html` (and this README) in a folder.
2. Open the folder in VS Code.
3. Either:
   - right-click `index.html` and choose **Open with Live Server** (needs the Live Server extension), or
   - double-click `index.html` to open it in your browser.

You don't need to install anything. It's a single file of plain HTML, CSS and JavaScript.

## Demo tips

- **Turn your volume down before the screech.** It's meant to be loud, and it's very loud in headphones.
- **Answer to the maths problem:** HCF × LCM of two numbers always equals the two numbers multiplied together. For HCF(12, 18) × LCM(12, 18), the answer is 12 × 18 = **216**.
- The fonts load from Google Fonts, so you need internet for the nicer fonts. Without it the page still works.
- If the screech doesn't play, click once anywhere on the page. Browsers block sound until the user has clicked something.

## Tweaks

- **Flip the cursor up and down too:** in the `<script>` near the top, change `const INVERT_Y = false;` to `true`.
- **Change the forced name:** search for `'habibi'` in the script and replace it.
- **Change the wait time:** search for `10000` (milliseconds) in the `login()` function.

## Built with

- HTML, CSS and JavaScript only. No frameworks.
- Web Audio API for the screech.
- Fonts: Fraunces, DM Sans, JetBrains Mono.
