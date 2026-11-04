# Day 7 · Responsive design

_Module 4, UI/UX & Frontend Development, Lexicon IT-Proffs_

## What you will do today

You will make the entire site responsive using a _mobile-first_ approach, with breakpoints at 600 px and 900 px, and test it in DevTools device mode.

## Background

Responsive design means that the same page works on all screen sizes. **Mobile first** means writing CSS for the smallest screen first, then adding more with `@media (min-width: ...)` when there is enough space. You already have a solid foundation because you built the layout with flex and grid.

## How to work (the same as always)

1. **Fork** today's repository on GitHub (_Fork → Create fork_).
2. **Clone your fork:** _Code → HTTPS → copy the URL_. In the terminal (Ctrl+ö in VS Code): `git clone <url>`. Open the new folder in VS Code and start _Live Server_.
3. **Complete the assignment.** Save and check in the browser after each step. Make a commit after each completed step: `git add .` and `git commit -m "Describe what you did"`.
4. **Push** when you are done: `git push`.
5. **Submit in Microsoft Forms.**

If you get stuck, write down exactly where you got stuck and what you have tried, and bring it up first in the next guided session.

## The assignment step by step

### Step 1. Check the viewport tag

Both HTML files must include `<meta name="viewport" ...>`. Without it, none of today's work will function as intended.

### Step 2. Test in device mode

Open DevTools and click the device icon (Ctrl+Shift+M). Test at 360, 768, and 1280 px. Write down three things that are wrong or cramped.

### Step 3. Write mobile-first CSS

Make sure the base CSS (without media queries) looks good at a width of 360 px: one column with appropriate padding.

### Step 4. Breakpoint 1: 600 px

Add `@media (min-width: 600px) { ... }`: more `padding` in `main` and a larger hero heading.

### Step 5. Breakpoint 2: 900 px

Add `@media (min-width: 900px) { ... }`: an About Us section in two columns and a wider header.

### Step 6. Images and forms

Check that no images overflow and that form fields are neither too wide nor too narrow at any screen size.

### Step 7. Test on a real device

Open your page on a real phone (Live Server provides a network address, or use device mode if you cannot use a phone). Write down what you noticed.

## Checklist: how to know you are done

- [ ] The viewport meta tag is present in both files.
- [ ] The page works without horizontal scrolling at 360 px.
- [ ] There are at least two breakpoints using `min-width` (mobile first).
- [ ] The layout adapts sensibly between mobile, medium-sized screens, and desktop.
- [ ] You have tested in DevTools device mode at at least three widths.
- [ ] You have pushed to your fork and submitted the link.

## Tips if you get stuck

- Horizontal scrolling? An element has a fixed width. Find it with DevTools by hovering over the elements.
- A media query does not seem to apply? Check the braces and make sure it appears AFTER the base rules in the file.
- Breakpoints should be determined by when the _content_ no longer fits properly, rather than by specific devices.

## Submission

**Deadline: tomorrow at 09:00.** Submit everything in Microsoft Forms. No oral presentation is required.

In the form, provide:

1. A link to your fork of this repository.
2. A reflection: At what width did your page's layout first break, and how did you fix it?

## Want to do more? (optional)

- Add a third breakpoint at 1200 px for large screens.
- Use `clamp()` to make the hero heading scale fluidly without a media query.

## Responsive testing

- At 360px: The page became narrower and the content looked cramped. But not that much of a difference i would say.
- At 768px: The page got expanded and you can see two products from the meny list.
- At 1280px: The page got bigger and wider and easier for the user to navigate.

## Real device test

I tested the page on my phone in portrait and landscape mode.
The text was readable, the buttons were easy to tap, and the form fitted the screen. http://192.168.50.215:5500/index.html i used it to navigate trough my phone . i found it through the Live Server and i also wrote at the terminal "ipconfig".
