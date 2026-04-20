# Language Translation Tool

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

A clean and responsive language translation web app built with HTML, CSS, and vanilla JavaScript. The project lets users type text, auto-detect the source language, choose a target language, and get instant translations directly in the browser.

## Live Demo

[View the deployed project](https://aman-2346.github.io/Language-translation-tool/)

## Features

- Real-time translation as the user types
- Auto-detect option for the source language
- 60+ language choices
- One-click language swap
- Character counter with a 5000 character limit
- Light and dark mode toggle
- Responsive layout for desktop and mobile screens
- Simple frontend-only setup with no build tools required

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- Ionicons for interface icons
- Google Translate web endpoint for translation requests

## Project Structure

```text
Language_Translation/
|-- index.html
|-- styles/
|   `-- style.css
|-- script/
|   |-- script.js
|   `-- languages.js
`-- images/
    |-- moon.png
    `-- sun.png
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/aman-2346/Language-translation-tool.git
cd Language-translation-tool
```

### 2. Run the project

This is a static frontend project, so you can run it with any local server.

Option 1: Use VS Code Live Server

- Open the folder in VS Code
- Install the Live Server extension if needed
- Right-click `index.html` and choose `Open with Live Server`

Option 2: Use Python

```bash
python -m http.server 5500
```

Then open `http://localhost:5500` in your browser.

## How to Use

1. Enter or paste text into the left text area.
2. Keep the source language on `Auto Detect` or choose a specific language.
3. Select the language you want to translate into.
4. Click the swap button to reverse the source and target languages.
5. Use the theme toggle in the bottom-right corner to switch between light and dark mode.

## How It Works

- Language options are loaded from `script/languages.js`
- The app listens for input changes in `script/script.js`
- On each input update, it sends a request to the Google Translate endpoint
- The translated output is shown in the right-side text area

## Notes

- An internet connection is required for translations to work
- The app currently depends on the Google Translate web endpoint, so behavior may change if that service changes
- File upload and download functionality is present in the code as commented sections, but it is not enabled in the current UI

## Future Improvements

- Add loading states and user-friendly error messages
- Debounce translation requests to reduce unnecessary API calls
- Add copy-to-clipboard support for translated text
- Save dark mode and selected languages in local storage
- Enable document upload and translated file download
- Add a custom domain or improve the deployment workflow

## Why This Project

This project is a strong example of a beginner-friendly but practical frontend application. It demonstrates DOM manipulation, API integration, responsive design, UI state handling, and clean project organization without relying on frameworks.

## Contributing

If you would like to improve the project, feel free to fork the repository, make your changes, and open a pull request.
