Live Project ::https://basic-calculation-of-array-js.vercel.app/


![Screenshot 2025-06-06 121119](https://github.com/user-attachments/assets/8ca1a257-9745-4273-99d8-36dfedca0656)

📁 File Structure:

project/
│
├── index.html      # HTML structure for the calculator UI
├── style.css       # Custom styles for the calculator
└── script.js       # JavaScript functionality for calculator operations

🔹 index.html
      Purpose:
        Defines the calculator's layout and loads necessary resources (Bootstrap, custom CSS, and JS).
 *  Key Components:
    - HTML5 document with Bootstrap CDN and favicon.
    - Main container: .container holds the calculator card.
    - Display input: <input id="display"> shows the current calculation.
    - Buttons: Grid of buttons (0–9, +, -, *, /, %, AC, DEL, =, etc.) for user interaction.
 *  Notes:
   - Form is used to hold the input box.
   - Button rows are structured using divs.
🔹 style.css
 *  Purpose:
     Styles the calculator for a modern and clean UI experience.
  - Key Features:
     Body: Light background (#d8e2dc) and full height.
    .calculator: Dark card layout with padding and rounded corners.

  - Input field:
- Center-aligned text.
- Large font for visibility.
- Shadows and rounded edges for better UI.

Buttons:
- Circular shape with shadows.
- Hover effects for interactivity.
- Consistent size and spacing.

Custom operator color (#55b386) handled inline in HTML.

🔹 script.js
Purpose:
Handles all calculator functionalities through vanilla JavaScript.

* Functional Flow:
- Event Listener:
- Adds click listener to every <button>.

* Operation Handling:
- =: Evaluates the expression using eval().
- AC: Clears the entire input.
- DEL: Removes the last character.
- Operators (+, -, *, /, %): Prevents duplicate operators at the end.
- Numbers & dot (.): Appends to the current input.

✅ Features:
-Responsive design using Bootstrap.
-Clear and Delete functionality.
-Live input handling.
-Prevents consecutive operator input (e.g., 5++2 becomes 5+2).
-Shadow and hover effects for better UX.

⚠️ Suggestions for Improvement:
Validation: Use try-catch to avoid eval() runtime errors.
Security: Consider replacing eval() with a safer math parser (like math.js).
Accessibility: Add aria-label attributes and keyboard support.

