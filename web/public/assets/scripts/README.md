[&larr; Up one folder](../README.md)
<hr>

# Website scripts

The code that makes the page do things. Plain JavaScript, no frameworks, so
the page loads fast and works offline once visited.

| File | What it does |
|---|---|
| [app.js](app.js) | Site-wide behaviour: the light/dark theme switch (remembered for next time), the mobile menu, the keyboard-friendly feature tabs, and registering the offline support. |
| [pads.js](pads.js) | The playable 16-pad demo: loads the demo kit on first touch, plays it with velocity depending on where you hit, lets the closed hi-hat cut the open one, and drives the level meters from the real output. Keyboard keys play the pads too. |
