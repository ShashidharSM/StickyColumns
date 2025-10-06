# StickyColumns - A One Page Organizer

Organize sticky notes in columns. 100% local (no servers), React + CDN, single file.

Sticky Columns is a simple board to manage and plan your tasks; this is a standalone board I use to track my projects and tasks as a freelancer. Your data is saved locally, and resources are fetched from CDN, elminitaing any prior setup. 
Works best on a wide screen monitor - Responsive version coming soon.

## Features
- Add/rename/delete columns (max 10), drag to reorder
- Add/edit/delete notes, drag between columns
- Export/Import board JSON
- Dark mode (auto + toggle)

## Use
- Open `StickyColumns.html` in your browser.
- Data is stored in `localStorage` under `sticky-columns:v1`.
- Theme is stored in `localStorage` under `sticky-columns:theme`.

## Setup Instructions
### Quick Run (needs internet for the CDN scripts):
1) Save this file as index.html
2) Double-click to open in your browser

### Local/Offline Options:
#### Option A: Keep single-file workflow using local vendor scripts
   - Download these files next to index.html:
     - react.production.min.js (React 18 UMD)
     - react-dom.production.min.js (ReactDOM 18 UMD)
     - babel.min.js (babel-standalone)
   - Replace the three <script> tags at the top to point to the local copies.

#### Option B: "No Babel" build (faster, no CDN) – if you’re comfortable with a one-time build:
   - Create a folder and run:  npm create vite@latest sticky-columns -- --template react
     - Move the JSX into /src (e.g., App.jsx). Remove the Babel CDN from index.html.
     - Run:  npm install  &&  npm run build
     - Open dist/index.html in a browser (fully offline).

## Privacy
All data is stored in localStorage under key "sticky-columns:v1". Theme preference stored in "sticky-columns:theme".

## License
MIT © 2025 Shashi Sreedhara

