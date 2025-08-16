# Awesome Kartikey Paint Clone

A simple, web-based paint application clone built with HTML, CSS, and vanilla JavaScript. Allows users to draw, erase, change colors and brush sizes, save/load drawings to local storage, and download the final artwork.



## Features

- **Brush Tool:** Draw lines with adjustable size and color.
- **Color Picker:** Choose custom colors for the brush and background using `jscolor.js`.
- **Brush Size Slider:** Dynamically change the brush thickness.
- **Bucket Fill:** Change the canvas background color.
- **Eraser:** Erase parts of the drawing (effectively paints with the background color).
- **Clear Canvas:** Reset the entire canvas to the background color.
- **Local Storage Persistence:**
  - Save the current drawing state to the browser's local storage.
  - Load the previously saved drawing from local storage.
  - Clear the saved drawing from local storage.
- **Download Image:** Save the current canvas drawing as a JPEG image file.
- **Active Tool Display:** Shows the currently selected tool (Brush/Eraser) or status messages.
- **Responsive Handling:** Displays a message prompting users to use a larger screen on mobile devices.

## Tech Stack

- **Frontend:** HTML5, CSS3, Vanilla JavaScript
- **APIs:** HTML Canvas API, Web Storage API (Local Storage)
- **Libraries:**
  - [jscolor.js](http://jscolor.com/): For the color picker UI.
  - [Font Awesome](https://fontawesome.com/): For icons.

## Setup Instructions

No complex build process is required. Simply clone the repository and open the `index.html` file in your web browser.

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/awesome-kartikey/paint-clone.git
    ```
2.  **Navigate to the directory:**
    ```bash
    cd paint-clone
    ```
3.  **Open the HTML file:**
    - Open `index.html` directly in your preferred web browser (e.g., Chrome, Firefox, Edge).

## Usage

1.  **Open `index.html`** in your browser.
2.  **Select a Tool:**
    - **Brush:** Click the brush icon or just start drawing. Use the color picker next to it to change the brush color and the slider/input to change the brush size.
    - **Bucket:** Click the paint bucket icon and use its color picker to change the canvas background color.
    - **Eraser:** Click the eraser icon. The brush size automatically maximizes for erasing.
3.  **Draw:** Click and drag the mouse on the canvas area to draw or erase.
4.  **Clear:** Click the undo icon (`fa-undo-alt`) to clear the entire canvas.
5.  **Save/Load:**
    - Click the download icon (`fa-download`) to save your drawing progress to local storage.
    - Click the upload icon (`fa-upload`) to load your previously saved drawing.
    - Click the trash icon (`fa-trash-alt`) to remove the saved drawing from local storage.
6.  **Download:** Click the save icon (`fa-save`) to download the current canvas as a `paint-example.jpeg` file.
