# Mellow
Mellow helps you give one thing your attention, then take a real break. Start a 25-minute focus session, keep a small list for today, and watch your progress grow — all in a quiet, responsive interface.

#What’s inside
•Three gentle timers: 25-minute focus, 5-minute short break, and 15-minute long break.
•A simple daily rhythm: Four focus rounds make up the suggested daily goal; breaks are offered between rounds.
•Today’s task list: Add, complete, and remove tasks without losing your train of thought.
•A little progress view: See completed sessions, focus minutes, and progress toward four sessions.
•Optional chime: A subtle two-note sound at the end of a timer. Off by default.
•Private by design: Tasks and today’s progress stay in your browser’s local storage.
•Responsive and lightweight: Works on desktop and mobile with no build step or third-party JavaScript.

#Get started
Run it locally1.Download or clone this repository.
2.Open index.html in a modern browser.
3.Press Start focus. That’s it.To serve it locally instead, 
run:python3 -m http.server 8000
Then visit http://localhost:8000.

#Publish with GitHub Pages
1.Create a GitHub repository and add these files.
2.Open Settings → Pages.
3.Under Build and deployment, select Deploy from a branch.
4.Choose your default branch and the /(root) folder, then save.

GitHub Pages will publish the app at your repository’s Pages URL. No build command or framework configuration is required.

#Project structure
mellow-focus/
├── assets/
│   ├── cover.svg       # Repository cover artwork
│   └── favicon.svg     # Browser tab icon
├── app.js              # Timer, task list, and local persistence
├── index.html          # Accessible app structure
├── styles.css          # Responsive visual design
├── .nojekyll           # Keep GitHub Pages deployment simple
├── .gitignore
├── LICENSE
└── README.md


#Privacy and browser support
Mellow does not send data to a server. Tasks, session count, focus minutes, and sound preference are stored in localStorage on the device and browser where you use the app. The daily list and counters reset when the local calendar date changes. Clearing browser storage also clears Mellow’s saved data.The app uses modern browser features including localStorage, SVG, and the Web Audio API for the optional chime. If audio is unavailable or blocked, the timer still works normally. The optional typefaces load from Google Fonts; system fallbacks are included.


#Customize

Change the timer lengths in the DURATIONS constant at the top of app.js. The main colors and type stacks are CSS custom properties at the top of styles.css.

#Contributing

Issues and pull requests are welcome. For larger changes, open an issue first so we can keep the app intentionally small and focused.

#License
Mellow is released under the MIT License.




