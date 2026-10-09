# 📋 Online Survey App

A simple online survey application built with **React**. A bank of 12 questions is available, and each user is asked to answer **5 random questions**.

## Features
- Question bank of 12 questions
- 5 random questions per attempt (Fisher-Yates shuffle)
- One question at a time with a progress bar
- "Next" is enabled only after an option is selected
- Summary of all answers at the end
- Responses saved in the browser (`localStorage`)
- "Take Again" gives a new set of random questions

## Tech Stack
- React 18 (loaded via CDN)
- Babel Standalone (JSX in the browser)
- HTML + CSS

## How to Run
No installation needed.

1. Download or clone this repository
2. Open `index.html` in a browser (double-click), or use the VS Code **Live Server** extension

> Internet connection is required because React is loaded from a CDN.

## Project Structure
```
survey-app/
├── index.html   # React app (components, question bank, styles)
├── README.md
└── .gitignore
```

## How It Works
1. `questionBank` holds all 12 questions with their options
2. `pickRandomQuestions()` shuffles the bank and takes the first 5
3. React state (`useState`) controls the screen: `start` → `question` → `result`
4. On submit, answers are shown and stored in `localStorage`

## Live Demo
Add your GitHub Pages link here after deploying:
`https://YOUR-USERNAME.github.io/survey-app/`
