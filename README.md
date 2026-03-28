# Basketball Playbook 🏀

A lightweight, browser-based digital whiteboard for basketball coaches and players. Easily draw up plays, add player positions, and save your strategies as image files.

## Features

* **Draw Plays:** Freehand drawing tool to map out player movement and ball passes.
* **Add Text:** Click anywhere on the court to drop text (great for labeling PG, SG, screens, etc.).
* **Color Picker:** Change the color of your markers and text on the fly.
* **Clear Board:** Instantly wipe the whiteboard clean to start a new play.
* **Custom Export:** Name your play and export the canvas directly as a `.PNG` file.

## Project Structure

Make sure your files are organized like this for the background image to load correctly:

```text
skitmc-basketball/
├── assets/
│   └── background.png    <-- Your basketball court image
├── index.html            <-- The main layout and UI
├── index.js              <-- The canvas drawing and saving logic
└── README.md