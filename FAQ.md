# Frequently Asked Questions (FAQ)

Here are some common questions about the Awesome Kartikey Paint Clone project.

**Q1: How do I change the brush size?**

A: Use the slider located next to the brush icon in the top toolbar. You can drag the slider or manually see the size update in the numerical display next to it. The size ranges from 1 to 50 pixels.

**Q2: How do I change the brush color?**

A: Click the color input box (displaying a hex color code) located next to the brush icon. A color picker will appear, allowing you to select a new color for your brush.

**Q3: How does the "Bucket" (Background Color) tool work?**

A: The bucket tool sets the background color of the canvas. Click the color input box next to the `fa-fill-drip` icon to choose a color. When selected, the entire canvas background will change to this color, and any subsequent "Clear Canvas" or "Eraser" actions will use this color. Note that it redraws the canvas, applying the new background _behind_ existing strokes that are restored.

**Q4: How does the Eraser work? Does it truly erase?**

A: The eraser simulates erasing by drawing with the _current background color_ (`bucketColor`). When you select the eraser, the brush color is temporarily set to the background color, and the brush size is set to the maximum (50px). It doesn't remove pixels but rather paints over them.

**Q5: What does the "Save Local Storage" button do?**

A: This button (`fa-download` icon) saves the sequence of drawing actions (lines, colors, sizes) you've made onto your browser's local storage. This allows you to close the browser and potentially restore your drawing later using the "Load Local Storage" button. It does _not_ save an image file.

**Q6: What does the "Load Local Storage" button do?**

A: This button (`fa-upload` icon) attempts to retrieve the drawing data saved previously using the "Save Local Storage" button. If data is found, it clears the current canvas and redraws the saved drawing.

**Q7: What happens if I click "Clear Local Storage"?**

A: This button (`fa-trash-alt` icon) permanently removes any drawing data previously saved to your browser's local storage for this application. This action cannot be undone.

**Q8: Can I save my drawing as an image file?**

A: Yes! Click the "Save Image File" button (`fa-save` icon). This will trigger a download of the current canvas content as a JPEG image file named `paint-example.jpeg`.

**Q9: Why does the application show a message on my mobile phone?**

A: The application's layout and controls are optimized for larger screens (like desktops or tablets). On screens narrower than 800px, it displays a message suggesting using a larger screen for the best experience, as the controls might be cramped or unusable otherwise.

**Q10: Can I undo my last stroke?**

A: No, the current implementation does not support undoing individual strokes. The only way to revert changes is to use the "Clear Canvas" button, which removes everything, or reload a previously saved state using "Load Local Storage".

**Q11: What external libraries does this project use?**

A: It uses `jscolor.js` for the color picker functionality and Font Awesome for the icons in the toolbar.

**Q12: Is this a collaborative painting tool?**

A: No, this is a single-user application. All drawing and saving happen locally in your browser.
