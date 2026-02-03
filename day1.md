# 📔 Coding Diary: Day 1 - HTML Structures & Data

## What I Learned
**Objective:** Moving beyond basic text tags to build accessible, meaningful page structures and handle user input.

* **Semantic HTML:** Learned the importance of using specific tags like `<nav>`, `<article>`, `<aside>`, and `<section>` instead of generic `<div>` tags to improve accessibility and SEO.
* **Forms & Inputs:** Explored different input types (Text, Password, Checkbox, Radio) and how to group them using `<fieldset>` and `<legend>`.
* **Media Elements:** Learned how to properly embed Images (`<img>`), Audio, Video, and SVGs to make the page interactive.
* **Hyperlinks:** Mastered the critical difference between **Absolute links** (full URLs like `https://google.com`) and **Relative paths** (local files like `./about.html`).

> **Diary Task:** Built a "Registration Page" featuring a name field, a country dropdown menu, and a bio text area.

---

## Problems Faced
* **Broken Image Paths:** My profile picture rendered as a broken icon. I was confused about how to reference a file located in a folder "above" my current file (`../`).
* **Unwanted Form Refresh:** Every time I clicked "Submit," the page reloaded instantly, clearing all the data I had just typed before I could see the result.
* **Invalid Nesting:** I placed a `<div>` block inside a `<p>` tag. The browser tried to fix it automatically, which caused my layout to look broken and disjointed.

---

## How I Solved Them
1.  **Fixing Paths:** I reorganized my files, moving images to a dedicated `assets/images/` folder. I updated the code to `src="./assets/images/pic.jpg"` and started using VS Code's autocomplete to ensure the path was valid.
2.  **Preventing Default Submit:** I learned that `<form>` tags have a default behavior to send data and reload. To stop this while testing, I added `onsubmit="return false"` to the form tag.
3.  **W3C Validation:** I used the [W3C HTML Validator](https://validator.w3.org/) tool to debug the layout. It flagged the nesting error immediately. I replaced the inner `<div>` with a `<span>` (an inline element), which is valid inside a paragraph.

---
**Next Goal:** Start styling this structure using basic CSS!
