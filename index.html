// index.js

// 1. Get DOM elements
const canvas = document.getElementById('courtCanvas');
const ctx = canvas.getContext('2d');
const colorPicker = document.getElementById('colorPicker');
const textInput = document.getElementById('textInput');
const filenameInput = document.getElementById('filenameInput');

const drawBtn = document.getElementById('drawBtn');
const textBtn = document.getElementById('textBtn');
const saveBtn = document.getElementById('saveBtn');
const clearBtn = document.getElementById('clearBtn');

// 2. State variables
let isDrawing = false;
let currentTool = 'draw'; // Can be 'draw' or 'text'
let currentColor = '#000000';

// 3. Load the background image (assets/background.png)
const backgroundImage = new Image();
backgroundImage.src = 'assets/background.png';

// Draw the background once it loads
backgroundImage.onload = () => {
    drawBackground();
};

function drawBackground() {
    // Clear the canvas first
    ctx.clearRect(0, 0, canvas.width, canvas.height);
    // Draw the image to fit the canvas
    ctx.drawImage(backgroundImage, 0, 0, canvas.width, canvas.height);
}

// 4. Tool Selection
drawBtn.addEventListener('click', () => currentTool = 'draw');
textBtn.addEventListener('click', () => currentTool = 'text');
colorPicker.addEventListener('input', (e) => currentColor = e.target.value);

// 5. Drawing & Clicking Logic
canvas.addEventListener('mousedown', (e) => {
    const rect = canvas.getBoundingClientRect();
    const x = e.clientX - rect.left;
    const y = e.clientY - rect.top;

    if (currentTool === 'draw') {
        isDrawing = true;
        ctx.beginPath();
        ctx.moveTo(x, y);
    } else if (currentTool === 'text') {
        // Add text at the clicked location
        const text = textInput.value;
        if (text) {
            ctx.font = '20px Arial';
            ctx.fillStyle = currentColor;
            ctx.fillText(text, x, y);
        }
    }
});

canvas.addEventListener('mousemove', (e) => {
    if (!isDrawing || currentTool !== 'draw') return;

    const rect = canvas.getBoundingClientRect();
    const x = e.clientX - rect.left;
    const y = e.clientY - rect.top;

    ctx.lineTo(x, y);
    ctx.strokeStyle = currentColor;
    ctx.lineWidth = 3;
    ctx.lineCap = 'round';
    ctx.stroke();
});

canvas.addEventListener('mouseup', () => {
    if (isDrawing) {
        isDrawing = false;
        ctx.closePath();
    }
});

// Stop drawing if mouse leaves the canvas
canvas.addEventListener('mouseout', () => {
    isDrawing = false;
});

// 6. Clear Board
clearBtn.addEventListener('click', () => {
    drawBackground(); // Resetting just means redrawing the background over everything
});

// 7. Save File Logic
saveBtn.addEventListener('click', () => {
    // Get the filename from the input, default to 'basketball-play' if empty
    let fileName = filenameInput.value.trim();
    if (!fileName) {
        fileName = 'basketball-play';
    }

    // Convert canvas to a data URL (PNG format)
    const dataURL = canvas.toDataURL('image/png');

    // Create a temporary link element to trigger the download
    const link = document.createElement('a');
    link.download = `${fileName}.png`;
    link.href = dataURL;
    link.click();
});